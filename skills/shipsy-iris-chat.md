---
name: iris-chat
description: Interact with Shipsy's website AI assistant via the irisChat operation.
api: openapi/shipsy-openapi.json
operations:
  - irisChat
---

## Steps
1. **POST** to `https://www.shipsy.ai/api/iris` with a JSON body containing a `messages` array as defined in the OpenAPI spec.
2. Receive a JSON response with a `response` field containing the assistant's reply.

### Request example
```json
{
  "messages": [
    {"role": "user", "content": "What is AgentFleet?"}
  ]
}
```

### Response example
```json
{
  "response": "AgentFleet is ..."
}
```