---
name: Screen a wallet address for risk (KYT)
description: Run zkMe Know-Your-Transaction checks on an on-chain address — labels, activity overview and a risk score — before allowing a transfer.
api: openapi/zkme-openapi.yml
operations: [getKytStatus, getAddressOverview, getRiskScore, getTransactionsInvestigation]
---

# Screen a wallet address for risk (KYT)

Use this skill to assess whether an on-chain wallet address is safe to interact
with, using zkMe's KYT surface.

## Steps
1. Optionally call `getKytStatus` (POST `.../kyt/status`) with `mchNo`, `apiKey`
   to confirm `support_api` and that the target `coin` is in `support_coin`.
2. Call `getAddressOverview` (POST `.../kyt/address/overview`) with `mchNo`,
   `apiKey`, `coin`, `address` to read balance, `txs_count`, first/last seen and
   totals.
3. Call `getRiskScore` (POST `.../kyt/risk/score`) with the same fields (plus an
   optional `txid`) and read `score`, `risk_level`, `risk_detail` and
   `hacking_event`. Gate the transaction on your risk threshold.
4. For a deeper look, call `getTransactionsInvestigation` (POST
   `.../kyt/transactions/investigation`) with `start_timestamp`,
   `end_timestamp`, `type` and `page`.

## Conventions
- Auth: `mchNo` + `apiKey` in the JSON body. See `authentication/zkme-authentication.yml`.
- KYT success code is `200` (not `80000000`). See `errors/zkme-problem-types.yml`.
- Rate limit: 10 calls/second/key.
