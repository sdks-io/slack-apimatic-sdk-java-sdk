
# Admin Conversations Invite Error Schema Exception

Schema for error response from admin.conversations.invite

*This model accepts additional fields of type Object.*

## Structure

`AdminConversationsInviteErrorSchemaException`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Error` | [`AdminConversationsInviteErrorEnum`](../../doc/models/admin-conversations-invite-error-enum.md) | Required | - | AdminConversationsInviteErrorEnum getError() | setError(AdminConversationsInviteErrorEnum error) |
| `Ok` | `String` | Required, Constant | **Value**: `"False"` | String getOk() | setOk(String ok) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "error": "channel_not_found",
  "ok": "False",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

