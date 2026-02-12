
# Apps Permissions Resources List Error Schema Exception

Schema for error response from apps.permissions.resources.list method

*This model accepts additional fields of type Object.*

## Structure

`AppsPermissionsResourcesListErrorSchemaException`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Callstack` | `String` | Optional | Note: PHP callstack is only visible in dev/qa | String getCallstack() | setCallstack(String callstack) |
| `Error` | [`AppsPermissionsResourcesListErrorEnum`](../../doc/models/apps-permissions-resources-list-error-enum.md) | Required | - | AppsPermissionsResourcesListErrorEnum getError() | setError(AppsPermissionsResourcesListErrorEnum error) |
| `Ok` | `String` | Required, Constant | **Value**: `"False"` | String getOk() | setOk(String ok) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "error": "invalid_cursor",
  "ok": "False",
  "callstack": "callstack8",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

