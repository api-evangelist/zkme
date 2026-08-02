---
name: Check a user's zkKYC status
description: Verify whether a wallet/account has passed zkMe zkKYC and inspect the individual verifier values (sanction, age, citizenship, location, uniqueness).
api: openapi/zkme-openapi.yml
operations: [queryKycInfoByAddress, getUsersList]
---

# Check a user's zkKYC status

Use this skill to confirm a user has completed zkMe zkKYC before granting them
access to a gated action, and to read which specific proofs they passed.

## Prerequisites
- `mchNo` (AppID) and `apiKey` from the zkMe dashboard.
- The `programNo` configured for your integration.

## Steps
1. Call `queryKycInfoByAddress` (POST `https://agw.zk.me/zkseradmin/openapi/queryKycInfoByAddress`)
   with body fields `mchNo`, `apiKey`, `programNo`, `account` (the user's wallet
   address, email, or identifier) and `chainId` (e.g. `"1"` for Ethereum,
   `"solana"` for Solana).
2. Confirm the response `code` is `80000000` (success). Read `kycStatus` and the
   `verifierValues` booleans: `sanction`, `age`, `citizenship`, `location`,
   `unique`. Only treat the user as verified when `kycStatus` indicates passed
   and the verifier values you require are `true`.
3. To reconcile many users, page through `getUsersList` (POST
   `.../kyc/getUsersList`) 50 users per page using `page`; wait until
   `clientUserIdentifier` is populated (it is empty until "KYC Passed").

## Conventions
- Auth: `mchNo` + `apiKey` are sent in the JSON body (not a header). See
  `authentication/zkme-authentication.yml`.
- Errors: any `code` other than `80000000` is a business error; read `msg`. See
  `errors/zkme-problem-types.yml`.
- Rate limit: 10 calls/second/key. See `rate-limits/zkme-rate-limits.yml`.
- No idempotency key; these are read-only queries and safe to retry.
