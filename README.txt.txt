# CurrencyConvertAPIProject

## Project Overview
This project implements a simple currency conversion API wrapper using AMDorenCurrencyAPI.

You can convert any amount from one currency to another using this API.

## How to Test

### Using cURL:
Change the "from", "to", or "amount" values to test different currencies:

Example command:
curl -X POST -H "Content-Type: application/json" -H "appId: biizep" -H "appKey: dibogezrelsss1ivbqcu" -d "{\"from\":\"USD\",\"to\":\"INR\",\"amount\":10}" "https://ind-thomas.dev.hyperverge.co/v1/test/CurrencyConvertAPI"

- Run this command in command prompt
- from: Source currency code (3 letters, e.g., USD)
- to: Target currency code (3 letters, e.g., INR)
- amount: Amount to convert

### Response
**Success Response Example:**
{
  "statusCode": 200,
  "data": {
    "status": "success",
    "metaData": {},
    "result": {
      "from": "USD",
      "to": "INR",
      "amount": 10,
      "converted": 830.25
    }
  }
}

**Error Response Example:**
{
  "statusCode": 400,
  "message": "Input Validation Error: Headers: requires property \"api_key\"",
  "status": "failure"
}

## Notes:
- Update "appId" and "appKey" with your credentials.
- You can change currency codes or amount in the JSON payload for testing.
 

App Credentials

appId: biizep

appKey: dibogezrelsss1ivbqcu

Always keep these credentials safe. Replace them in your cURL requests or module headers.
