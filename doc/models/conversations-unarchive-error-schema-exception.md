
# Conversations Unarchive Error Schema Exception

Schema for error response from conversations.unarchive method

*This model accepts additional fields of type Object.*

## Structure

`ConversationsUnarchiveErrorSchemaException`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Callstack` | `String` | Optional | Note: PHP callstack is only visible in dev/qa | String getCallstack() | setCallstack(String callstack) |
| `Error` | [`ConversationsUnarchiveErrorEnum`](../../doc/models/conversations-unarchive-error-enum.md) | Required | - | ConversationsUnarchiveErrorEnum getError() | setError(ConversationsUnarchiveErrorEnum error) |
| `Needed` | `String` | Optional | - | String getNeeded() | setNeeded(String needed) |
| `Ok` | `String` | Required, Constant | **Value**: `"False"` | String getOk() | setOk(String ok) |
| `Provided` | `String` | Optional | - | String getProvided() | setProvided(String provided) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "error": "invalid_form_data",
  "ok": "False",
  "callstack": "callstack2",
  "needed": "needed6",
  "provided": "provided2",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

