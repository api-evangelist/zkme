---
name: Check a business zkKYB verification status
description: Poll the zkMe zkKYB verification stage for a business entity you referenced by externalID.
api: openapi/zkme-openapi.yml
operations: [getAccessToken, getBusinessStatus]
---

# Check a business zkKYB verification status

Use this skill to track a business entity's progress through zkMe zkKYB.

## Steps
1. Mint an access token: call `getAccessToken` (POST
   `https://nest-api.zk.me/api/token/get`) with `apiKey`, `appId`,
   `apiModePermission`, `lv`. The token is valid for 30 minutes.
2. Call `getBusinessStatus` (POST
   `https://agw.zk.me/kybpopup/api/kyb/getBusinessStatus`) with `mchNo`,
   `accessToken`, `programNo`, and your `externalID` for the entity.
3. Confirm `code` is `80000000`, then read `data.statusCode`:
   1 Started, 2 Info Submitted, 3 Under Review, 4 Resubmission Required,
   5 Passed, 6 Failed — and `data.statusDesc` for the human-readable stage.
   Re-poll while the status is 1-4; treat 5 as verified.

## Conventions
- Auth: `mchNo` + short-lived `accessToken` in the JSON body. Re-mint the token
  every 30 minutes. See `authentication/zkme-authentication.yml`.
- Errors: any `code` other than `80000000` is a business error; read `msg`.
- Rate limit: 10 calls/second/key.
