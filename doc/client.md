
# Client Class Documentation

The following parameters are configurable for the API Client:

| Parameter | Type | Description |
|  --- | --- | --- |
| environment | [`Environment`](../README.md#environments) | The API environment. <br> **Default: `Environment.PRODUCTION`** |
| httpClientConfig | [`Consumer<HttpClientConfiguration.Builder>`](../doc/http-client-configuration-builder.md) | Set up Http Client Configuration instance. |
| loggingConfig | [`Consumer<ApiLoggingConfiguration.Builder>`](../doc/api-logging-configuration-builder.md) | Set up Logging Configuration instance. |
| authorizationCodeAuth | [`AuthorizationCodeAuth`](auth/oauth-2-authorization-code-grant.md) | The Credentials Setter for OAuth 2 Authorization Code Grant |

The API client can be initialized as follows:

```java
import com.slack.Environment;
import com.slack.SlackWebApiClient;
import com.slack.authentication.AuthorizationCodeAuthModel;
import com.slack.exceptions.ApiException;
import com.slack.http.response.ApiResponse;
import com.slack.models.OauthScope;
import com.slack.models.OauthToken;
import java.io.IOException;
import java.util.Arrays;
import org.slf4j.event.Level;

public class Program {
    public static void main(String[] args) {
        SlackWebApiClient client = new SlackWebApiClient.Builder()
            .loggingConfig(builder -> builder
                    .level(Level.DEBUG)
                    .requestConfig(logConfigBuilder -> logConfigBuilder.body(true))
                    .responseConfig(logConfigBuilder -> logConfigBuilder.headers(true)))
            .httpClientConfig(configBuilder -> configBuilder
                    .timeout(0))
            .authorizationCodeAuth(new AuthorizationCodeAuthModel.Builder(
                    "OAuthClientId",
                    "OAuthClientSecret",
                    "OAuthRedirectUri"
                )
                .oauthScopes(Arrays.asList(
                        OauthScope.ADMIN,
                        OauthScope.ADMIN_APPSREAD
                    ))
                .build())
            .environment(Environment.PRODUCTION)
            .build();

    }
}
```

## Slack Web APIClient Class

The gateway for the SDK. This class acts as a factory for the Apis and also holds the configuration of the SDK.

### Apis

| Name | Description | Return Type |
|  --- | --- | --- |
| `getAdminAppsApi()` | Provides access to AdminApps controller. | `AdminAppsApi` |
| `getAdminAppsApprovedApi()` | Provides access to AdminAppsApproved controller. | `AdminAppsApprovedApi` |
| `getAdminAppsRequestsApi()` | Provides access to AdminAppsRequests controller. | `AdminAppsRequestsApi` |
| `getAdminAppsRestrictedApi()` | Provides access to AdminAppsRestricted controller. | `AdminAppsRestrictedApi` |
| `getAdminConversationsApi()` | Provides access to AdminConversations controller. | `AdminConversationsApi` |
| `getAdminConversationsEkmApi()` | Provides access to AdminConversationsEkm controller. | `AdminConversationsEkmApi` |
| `getAdminConversationsRestrictAccessApi()` | Provides access to AdminConversationsRestrictAccess controller. | `AdminConversationsRestrictAccessApi` |
| `getAdminEmojiApi()` | Provides access to AdminEmoji controller. | `AdminEmojiApi` |
| `getAdminInviteRequestsApi()` | Provides access to AdminInviteRequests controller. | `AdminInviteRequestsApi` |
| `getAdminInviteRequestsApprovedApi()` | Provides access to AdminInviteRequestsApproved controller. | `AdminInviteRequestsApprovedApi` |
| `getAdminInviteRequestsDeniedApi()` | Provides access to AdminInviteRequestsDenied controller. | `AdminInviteRequestsDeniedApi` |
| `getAdminTeamsAdminsApi()` | Provides access to AdminTeamsAdmins controller. | `AdminTeamsAdminsApi` |
| `getAdminTeamsApi()` | Provides access to AdminTeams controller. | `AdminTeamsApi` |
| `getAdminTeamsOwnersApi()` | Provides access to AdminTeamsOwners controller. | `AdminTeamsOwnersApi` |
| `getAdminTeamsSettingsApi()` | Provides access to AdminTeamsSettings controller. | `AdminTeamsSettingsApi` |
| `getAdminUsergroupsApi()` | Provides access to AdminUsergroups controller. | `AdminUsergroupsApi` |
| `getAdminUsersApi()` | Provides access to AdminUsers controller. | `AdminUsersApi` |
| `getAdminUsersSessionApi()` | Provides access to AdminUsersSession controller. | `AdminUsersSessionApi` |
| `getApi()` | Provides access to Api controller. | `Api` |
| `getAppsEventAuthorizationsApi()` | Provides access to AppsEventAuthorizations controller. | `AppsEventAuthorizationsApi` |
| `getAppsPermissionsApi()` | Provides access to AppsPermissions controller. | `AppsPermissionsApi` |
| `getAppsPermissionsResourcesApi()` | Provides access to AppsPermissionsResources controller. | `AppsPermissionsResourcesApi` |
| `getAppsPermissionsScopesApi()` | Provides access to AppsPermissionsScopes controller. | `AppsPermissionsScopesApi` |
| `getAppsPermissionsUsersApi()` | Provides access to AppsPermissionsUsers controller. | `AppsPermissionsUsersApi` |
| `getAppsApi()` | Provides access to Apps controller. | `AppsApi` |
| `getAuthApi()` | Provides access to Auth controller. | `AuthApi` |
| `getBotsApi()` | Provides access to Bots controller. | `BotsApi` |
| `getCallsApi()` | Provides access to Calls controller. | `CallsApi` |
| `getCallsParticipantsApi()` | Provides access to CallsParticipants controller. | `CallsParticipantsApi` |
| `getChatApi()` | Provides access to Chat controller. | `ChatApi` |
| `getChatScheduledMessagesApi()` | Provides access to ChatScheduledMessages controller. | `ChatScheduledMessagesApi` |
| `getConversationsApi()` | Provides access to Conversations controller. | `ConversationsApi` |
| `getDialogApi()` | Provides access to Dialog controller. | `DialogApi` |
| `getDndApi()` | Provides access to Dnd controller. | `DndApi` |
| `getEmojiApi()` | Provides access to Emoji controller. | `EmojiApi` |
| `getFilesCommentsApi()` | Provides access to FilesComments controller. | `FilesCommentsApi` |
| `getFilesApi()` | Provides access to Files controller. | `FilesApi` |
| `getFilesRemoteApi()` | Provides access to FilesRemote controller. | `FilesRemoteApi` |
| `getMigrationApi()` | Provides access to Migration controller. | `MigrationApi` |
| `getOauthApi()` | Provides access to Oauth controller. | `OauthApi` |
| `getOauthV2Api()` | Provides access to OauthV2 controller. | `OauthV2Api` |
| `getPinsApi()` | Provides access to Pins controller. | `PinsApi` |
| `getReactionsApi()` | Provides access to Reactions controller. | `ReactionsApi` |
| `getRemindersApi()` | Provides access to Reminders controller. | `RemindersApi` |
| `getRtmApi()` | Provides access to Rtm controller. | `RtmApi` |
| `getSearchApi()` | Provides access to Search controller. | `SearchApi` |
| `getStarsApi()` | Provides access to Stars controller. | `StarsApi` |
| `getTeamApi()` | Provides access to Team controller. | `TeamApi` |
| `getTeamProfileApi()` | Provides access to TeamProfile controller. | `TeamProfileApi` |
| `getUsergroupsApi()` | Provides access to Usergroups controller. | `UsergroupsApi` |
| `getUsergroupsUsersApi()` | Provides access to UsergroupsUsers controller. | `UsergroupsUsersApi` |
| `getUsersApi()` | Provides access to Users controller. | `UsersApi` |
| `getUsersProfileApi()` | Provides access to UsersProfile controller. | `UsersProfileApi` |
| `getViewsApi()` | Provides access to Views controller. | `ViewsApi` |
| `getWorkflowsApi()` | Provides access to Workflows controller. | `WorkflowsApi` |
| `getOauthAuthorizationApi()` | Provides access to OauthAuthorization controller. | `OauthAuthorizationApi` |

### Methods

| Name | Description | Return Type |
|  --- | --- | --- |
| `shutdown()` | Shutdown the underlying HttpClient instance. | `void` |
| `getEnvironment()` | Current API environment. | `Environment` |
| `getHttpClient()` | The HTTP Client instance to use for making HTTP requests. | `HttpClient` |
| `getHttpClientConfig()` | Http Client Configuration instance. | [`ReadonlyHttpClientConfiguration`](../doc/http-client-configuration.md) |
| `getLoggingConfig()` | Logging Configuration instance. | [`ReadonlyLoggingConfiguration`](../doc/api-logging-configuration.md) |
| `getAuthorizationCodeAuth()` | The credentials to use with AuthorizationCodeAuth. | [`AuthorizationCodeAuth`](auth/oauth-2-authorization-code-grant.md) |
| `getBaseUri(Server server)` | Get base URI by current environment | `String` |
| `getBaseUri()` | Get base URI by current environment | `String` |

