
# Usergroups Update Error Schema Exception

Schema for error response from usergroups.update method

*This model accepts additional fields of type Object.*

## Structure

`UsergroupsUpdateErrorSchemaException`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Callstack` | `String` | Optional | Note: PHP callstack is only visible in dev/qa | String getCallstack() | setCallstack(String callstack) |
| `Error` | [`UsergroupsUpdateErrorEnum`](../../doc/models/usergroups-update-error-enum.md) | Required | - | UsergroupsUpdateErrorEnum getError() | setError(UsergroupsUpdateErrorEnum error) |
| `Ok` | `String` | Required, Constant | **Value**: `"False"` | String getOk() | setOk(String ok) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "error": "token_revoked",
  "ok": "False",
  "callstack": "callstack2",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

