
# Admin Conversations Create Error Schema Exception

Schema for error response from admin.conversations.create

*This model accepts additional fields of type Object.*

## Structure

`AdminConversationsCreateErrorSchemaException`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Error` | [`AdminConversationsCreateErrorEnum`](../../doc/models/admin-conversations-create-error-enum.md) | Required | - | AdminConversationsCreateErrorEnum getError() | setError(AdminConversationsCreateErrorEnum error) |
| `Ok` | `String` | Required, Constant | **Value**: `"False"` | String getOk() | setOk(String ok) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "error": "could_not_create_channel",
  "ok": "False",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

