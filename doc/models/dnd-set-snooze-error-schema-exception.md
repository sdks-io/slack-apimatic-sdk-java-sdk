
# Dnd Set Snooze Error Schema Exception

Schema for error response from dnd.setSnooze method

*This model accepts additional fields of type Object.*

## Structure

`DndSetSnoozeErrorSchemaException`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Callstack` | `String` | Optional | Note: PHP callstack is only visible in dev/qa | String getCallstack() | setCallstack(String callstack) |
| `Error` | [`DndSetSnoozeErrorEnum`](../../doc/models/dnd-set-snooze-error-enum.md) | Required | - | DndSetSnoozeErrorEnum getError() | setError(DndSetSnoozeErrorEnum error) |
| `Ok` | `String` | Required, Constant | **Value**: `"False"` | String getOk() | setOk(String ok) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "error": "invalid_json",
  "ok": "False",
  "callstack": "callstack0",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

