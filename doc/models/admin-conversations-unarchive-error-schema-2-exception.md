
# Admin Conversations Unarchive Error Schema 2 Exception

Schema for error response from admin.conversations.rename

*This model accepts additional fields of type Object.*

## Structure

`AdminConversationsUnarchiveErrorSchema2Exception`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Error` | [`AdminConversationsRenameErrorEnum`](../../doc/models/admin-conversations-rename-error-enum.md) | Required | - | AdminConversationsRenameErrorEnum getError() | setError(AdminConversationsRenameErrorEnum error) |
| `Ok` | `String` | Required, Constant | **Value**: `"False"` | String getOk() | setOk(String ok) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "error": "name_taken",
  "ok": "False",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

