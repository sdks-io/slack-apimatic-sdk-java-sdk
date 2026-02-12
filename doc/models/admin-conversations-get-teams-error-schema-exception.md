
# Admin Conversations Get Teams Error Schema Exception

Schema for error response from admin.conversations.getTeams

*This model accepts additional fields of type Object.*

## Structure

`AdminConversationsGetTeamsErrorSchemaException`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Error` | [`AdminConversationsGetTeamsErrorEnum`](../../doc/models/admin-conversations-get-teams-error-enum.md) | Required | - | AdminConversationsGetTeamsErrorEnum getError() | setError(AdminConversationsGetTeamsErrorEnum error) |
| `Ok` | `String` | Required, Constant | **Value**: `"False"` | String getOk() | setOk(String ok) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "error": "channel_type_not_supported",
  "ok": "False",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

