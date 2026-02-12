
# Usergroups Users List Error Schema Exception

Schema for error response from usergroups.users.list method

*This model accepts additional fields of type Object.*

## Structure

`UsergroupsUsersListErrorSchemaException`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Callstack` | `String` | Optional | Note: PHP callstack is only visible in dev/qa | String getCallstack() | setCallstack(String callstack) |
| `Error` | [`UsergroupsEnableErrorEnum`](../../doc/models/usergroups-enable-error-enum.md) | Required | - | UsergroupsEnableErrorEnum getError() | setError(UsergroupsEnableErrorEnum error) |
| `Ok` | `String` | Required, Constant | **Value**: `"False"` | String getOk() | setOk(String ok) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "error": "invalid_post_type",
  "ok": "False",
  "callstack": "callstack8",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

