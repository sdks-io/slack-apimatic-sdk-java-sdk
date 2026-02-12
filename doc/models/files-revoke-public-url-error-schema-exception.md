
# Files Revoke Public Url Error Schema Exception

Schema for error response from files.revokePublicURL method

*This model accepts additional fields of type Object.*

## Structure

`FilesRevokePublicUrlErrorSchemaException`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Callstack` | `String` | Optional | Note: PHP callstack is only visible in dev/qa | String getCallstack() | setCallstack(String callstack) |
| `Error` | [`FilesRevokePublicUrlErrorEnum`](../../doc/models/files-revoke-public-url-error-enum.md) | Required | - | FilesRevokePublicUrlErrorEnum getError() | setError(FilesRevokePublicUrlErrorEnum error) |
| `Ok` | `String` | Required, Constant | **Value**: `"False"` | String getOk() | setOk(String ok) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "error": "team_added_to_org",
  "ok": "False",
  "callstack": "callstack0",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

