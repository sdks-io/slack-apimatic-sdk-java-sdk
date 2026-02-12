
# Conversations Set Purpose Error Schema Exception

Schema for error response from conversations.setPurpose method

*This model accepts additional fields of type Object.*

## Structure

`ConversationsSetPurposeErrorSchemaException`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Callstack` | `String` | Optional | Note: PHP callstack is only visible in dev/qa | String getCallstack() | setCallstack(String callstack) |
| `Error` | [`ConversationsSetPurposeErrorEnum`](../../doc/models/conversations-set-purpose-error-enum.md) | Required | - | ConversationsSetPurposeErrorEnum getError() | setError(ConversationsSetPurposeErrorEnum error) |
| `Needed` | `String` | Optional | - | String getNeeded() | setNeeded(String needed) |
| `Ok` | `String` | Required, Constant | **Value**: `"False"` | String getOk() | setOk(String ok) |
| `Provided` | `String` | Optional | - | String getProvided() | setProvided(String provided) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "error": "request_timeout",
  "ok": "False",
  "callstack": "callstack0",
  "needed": "needed4",
  "provided": "provided0",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

