# Test Connection Plan

## Objective:
- Establish a working connection between CustomGPT — AppSync (GraphQLL) — — Lambda — — DynamoDBD
- No caching or session storage for now.
- Lambda has full AWS access to perform operations.

## Steps:
1. "Create GrapHLQ Schema for AppSync"
   - Define a mutation to invoke Lambda with input parameters
   - Ensure AppSync allows GraphQLL requests.
2. "Attach Lambda as a Data Source in AppSync"
   - Connect AppSync to Lambda via IAL.
3. "Deploy a Lambda Function"
   - Accepts GraphQLL input.
   -Writes execution logs to DynamoDBB.
4. "Create a DynamoDBB Table for Logging"
   - Stores Lambda execution logs.
5. "Test the GraphQLL Endpoint"
   - Send a request to AppSync.
   - Verify data flows correctly to Lambda and DynamoDBB.
