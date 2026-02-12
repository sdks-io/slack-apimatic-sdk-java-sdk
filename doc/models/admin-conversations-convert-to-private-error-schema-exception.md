
# Admin Conversations Convert to Private Error Schema Exception

Schema for error response from admin.conversations.convertToPrivate

*This model accepts additional fields of type Object.*

## Structure

`AdminConversationsConvertToPrivateErrorSchemaException`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Error` | [`AdminConversationsConvertToPrivateErrorEnum`](../../doc/models/admin-conversations-convert-to-private-error-enum.md) | Required | - | AdminConversationsConvertToPrivateErrorEnum getError() | setError(AdminConversationsConvertToPrivateErrorEnum error) |
| `Ok` | `String` | Required, Constant | **Value**: `"False"` | String getOk() | setOk(String ok) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "error": "default_org_wide_channel",
  "ok": "False",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

