
# Admin Conversations Set Conversation Prefs Error Schema Exception

Schema for error response from admin.conversations.setConversationPrefs

*This model accepts additional fields of type Object.*

## Structure

`AdminConversationsSetConversationPrefsErrorSchemaException`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Error` | [`AdminConversationsSetConversationPrefsErrorEnum`](../../doc/models/admin-conversations-set-conversation-prefs-error-enum.md) | Required | - | AdminConversationsSetConversationPrefsErrorEnum getError() | setError(AdminConversationsSetConversationPrefsErrorEnum error) |
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

