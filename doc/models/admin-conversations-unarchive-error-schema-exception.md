
# Admin Conversations Unarchive Error Schema Exception

Schema for error response from admin.conversations.getConversationPrefs

*This model accepts additional fields of type Object.*

## Structure

`AdminConversationsUnarchiveErrorSchemaException`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Error` | [`AdminConversationsGetConversationPrefsErrorEnum`](../../doc/models/admin-conversations-get-conversation-prefs-error-enum.md) | Required | - | AdminConversationsGetConversationPrefsErrorEnum getError() | setError(AdminConversationsGetConversationPrefsErrorEnum error) |
| `Ok` | `String` | Required, Constant | **Value**: `"False"` | String getOk() | setOk(String ok) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "error": "missing_scope",
  "ok": "False",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

