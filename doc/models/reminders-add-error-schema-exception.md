
# Reminders Add Error Schema Exception

Schema for error response from reminders.add method

*This model accepts additional fields of type Object.*

## Structure

`RemindersAddErrorSchemaException`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Callstack` | `String` | Optional | Note: PHP callstack is only visible in dev/qa | String getCallstack() | setCallstack(String callstack) |
| `Error` | [`RemindersAddErrorEnum`](../../doc/models/reminders-add-error-enum.md) | Required | - | RemindersAddErrorEnum getError() | setError(RemindersAddErrorEnum error) |
| `Ok` | `String` | Required, Constant | **Value**: `"False"` | String getOk() | setOk(String ok) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "error": "no_permission",
  "ok": "False",
  "callstack": "callstack8",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

