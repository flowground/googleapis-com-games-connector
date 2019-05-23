# ![LOGO](logo.png) Google Play Game Services **flow**ground Connector

## Description

A generated **flow**ground connector for the Google Play Game Services API (version v1).

Generated from: https://api.apis.guru/v2/specs/googleapis.com/games/v1/swagger.json<br/>
Generated at: 2019-05-23T12:13:24+03:00

## API Description

The API for Google Play Game Services.

## Authorization

Supported authorization schemes:
- OAuth2

For OAuth 2.0 you need to specify OAuth Client credentials as environment variables in the connector repository:
* `OAUTH_CLIENT_ID` - your OAuth client id
* `OAUTH_CLIENT_SECRET` - your OAuth client secret

## Actions

### Lists all the achievement definitions for your application.

*Tags:* `achievementDefinitions`

#### Input Parameters
* `language` - _optional_ - The preferred language to use for strings returned by this method.
* `maxResults` - _optional_ - The maximum number of achievement resources to return in the response, used for paging. For any response, the actual number of achievement resources returned may be less than the specified maxResults.
* `pageToken` - _optional_ - The token returned by the previous request.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Updates multiple achievements for the currently authenticated player.

*Tags:* `achievements`

#### Input Parameters
* `builtinGameId` - _optional_ - Override used only by built-in games in Play Games application.
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Increments the steps of the achievement with the given ID for the currently authenticated player.

*Tags:* `achievements`

#### Input Parameters
* `achievementId` - _required_ - The ID of the achievement used by this method.
* `requestId` - _optional_ - A randomly generated numeric ID for each request specified by the caller. This number is used at the server to ensure that the request is handled correctly across retries.
* `stepsToIncrement` - _required_ - The number of steps to increment.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Sets the state of the achievement with the given ID to REVEALED for the currently authenticated player.

*Tags:* `achievements`

#### Input Parameters
* `achievementId` - _required_ - The ID of the achievement used by this method.
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Sets the steps for the currently authenticated player towards unlocking an achievement. If the steps parameter is less than the current number of steps that the player already gained for the achievement, the achievement is not modified.

*Tags:* `achievements`

#### Input Parameters
* `achievementId` - _required_ - The ID of the achievement used by this method.
* `steps` - _required_ - The minimum value to set the steps to.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Unlocks this achievement for the currently authenticated player.

*Tags:* `achievements`

#### Input Parameters
* `achievementId` - _required_ - The ID of the achievement used by this method.
* `builtinGameId` - _optional_ - Override used only by built-in games in Play Games application.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Indicate that the the currently authenticated user is playing your application.

*Tags:* `applications`

#### Input Parameters
* `builtinGameId` - _optional_ - Override used only by built-in games in Play Games application.
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Retrieves the metadata of the application with the given ID. If the requested application is not available for the specified platformType, the returned response will not include any instance data.

*Tags:* `applications`

#### Input Parameters
* `applicationId` - _required_ - The application ID from the Google Play developer console.
* `language` - _optional_ - The preferred language to use for strings returned by this method.
* `platformType` - _optional_ - Restrict application details returned to the specific platform.
    Possible values: ANDROID, IOS, WEB_APP.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Verifies the auth token provided with this request is for the application with the specified ID, and returns the ID of the player it was granted for.

*Tags:* `applications`

#### Input Parameters
* `applicationId` - _required_ - The application ID from the Google Play developer console.
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Returns a list of the event definitions in this application.

*Tags:* `events`

#### Input Parameters
* `language` - _optional_ - The preferred language to use for strings returned by this method.
* `maxResults` - _optional_ - The maximum number of event definitions to return in the response, used for paging. For any response, the actual number of event definitions to return may be less than the specified maxResults.
* `pageToken` - _optional_ - The token returned by the previous request.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Returns a list showing the current progress on events in this application for the currently authenticated user.

*Tags:* `events`

#### Input Parameters
* `language` - _optional_ - The preferred language to use for strings returned by this method.
* `maxResults` - _optional_ - The maximum number of events to return in the response, used for paging. For any response, the actual number of events to return may be less than the specified maxResults.
* `pageToken` - _optional_ - The token returned by the previous request.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Records a batch of changes to the number of times events have occurred for the currently authenticated user of this application.

*Tags:* `events`

#### Input Parameters
* `language` - _optional_ - The preferred language to use for strings returned by this method.
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Lists all the leaderboard metadata for your application.

*Tags:* `leaderboards`

#### Input Parameters
* `language` - _optional_ - The preferred language to use for strings returned by this method.
* `maxResults` - _optional_ - The maximum number of leaderboards to return in the response. For any response, the actual number of leaderboards returned may be less than the specified maxResults.
* `pageToken` - _optional_ - The token returned by the previous request.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Submits multiple scores to leaderboards.

*Tags:* `scores`

#### Input Parameters
* `language` - _optional_ - The preferred language to use for strings returned by this method.
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Retrieves the metadata of the leaderboard with the given ID.

*Tags:* `leaderboards`

#### Input Parameters
* `language` - _optional_ - The preferred language to use for strings returned by this method.
* `leaderboardId` - _required_ - The ID of the leaderboard.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Submits a score to the specified leaderboard.

*Tags:* `scores`

#### Input Parameters
* `language` - _optional_ - The preferred language to use for strings returned by this method.
* `leaderboardId` - _required_ - The ID of the leaderboard.
* `score` - _required_ - The score you're submitting. The submitted score is ignored if it is worse than a previously submitted score, where worse depends on the leaderboard sort order. The meaning of the score value depends on the leaderboard format type. For fixed-point, the score represents the raw value. For time, the score represents elapsed time in milliseconds. For currency, the score represents a value in micro units.
* `scoreTag` - _optional_ - Additional information about the score you're submitting. Values must contain no more than 64 URI-safe characters as defined by section 2.3 of RFC 3986.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Lists the scores in a leaderboard, starting from the top.

*Tags:* `scores`

#### Input Parameters
* `collection` - _required_ - The collection of scores you're requesting.
    Possible values: PUBLIC, SOCIAL, SOCIAL_1P.
* `language` - _optional_ - The preferred language to use for strings returned by this method.
* `leaderboardId` - _required_ - The ID of the leaderboard.
* `maxResults` - _optional_ - The maximum number of leaderboard scores to return in the response. For any response, the actual number of leaderboard scores returned may be less than the specified maxResults.
* `pageToken` - _optional_ - The token returned by the previous request.
* `timeSpan` - _required_ - The time span for the scores and ranks you're requesting.
    Possible values: ALL_TIME, DAILY, WEEKLY.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Lists the scores in a leaderboard around (and including) a player's score.

*Tags:* `scores`

#### Input Parameters
* `collection` - _required_ - The collection of scores you're requesting.
    Possible values: PUBLIC, SOCIAL, SOCIAL_1P.
* `language` - _optional_ - The preferred language to use for strings returned by this method.
* `leaderboardId` - _required_ - The ID of the leaderboard.
* `maxResults` - _optional_ - The maximum number of leaderboard scores to return in the response. For any response, the actual number of leaderboard scores returned may be less than the specified maxResults.
* `pageToken` - _optional_ - The token returned by the previous request.
* `resultsAbove` - _optional_ - The preferred number of scores to return above the player's score. More scores may be returned if the player is at the bottom of the leaderboard; fewer may be returned if the player is at the top. Must be less than or equal to maxResults.
* `returnTopIfAbsent` - _optional_ - True if the top scores should be returned when the player is not in the leaderboard. Defaults to true.
* `timeSpan` - _required_ - The time span for the scores and ranks you're requesting.
    Possible values: ALL_TIME, DAILY, WEEKLY.

### Return the metagame configuration data for the calling application.

*Tags:* `metagame`

#### Input Parameters
* `alt` - _optional_ - Data format for the response.
    Possible values: json.
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Get the collection of players for the currently authenticated user.

*Tags:* `players`

#### Input Parameters
* `collection` - _required_ - Collection of players being retrieved
    Possible values: connected, playedWith, played_with, visible.
* `language` - _optional_ - The preferred language to use for strings returned by this method.
* `maxResults` - _optional_ - The maximum number of player resources to return in the response, used for paging. For any response, the actual number of player resources returned may be less than the specified maxResults.
* `pageToken` - _optional_ - The token returned by the previous request.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Retrieves the Player resource with the given ID. To retrieve the player for the currently authenticated user, set playerId to me.

*Tags:* `players`

#### Input Parameters
* `language` - _optional_ - The preferred language to use for strings returned by this method.
* `playerId` - _required_ - A player ID. A value of me may be used in place of the authenticated player's ID.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Lists the progress for all your application's achievements for the currently authenticated player.

*Tags:* `achievements`

#### Input Parameters
* `language` - _optional_ - The preferred language to use for strings returned by this method.
* `maxResults` - _optional_ - The maximum number of achievement resources to return in the response, used for paging. For any response, the actual number of achievement resources returned may be less than the specified maxResults.
* `pageToken` - _optional_ - The token returned by the previous request.
* `playerId` - _required_ - A player ID. A value of me may be used in place of the authenticated player's ID.
* `state` - _optional_ - Tells the server to return only achievements with the specified state. If this parameter isn't specified, all achievements are returned.
    Possible values: ALL, HIDDEN, REVEALED, UNLOCKED.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### List play data aggregated per category for the player corresponding to playerId.

*Tags:* `metagame`

#### Input Parameters
* `collection` - _required_ - The collection of categories for which data will be returned.
    Possible values: all.
* `language` - _optional_ - The preferred language to use for strings returned by this method.
* `maxResults` - _optional_ - The maximum number of category resources to return in the response, used for paging. For any response, the actual number of category resources returned may be less than the specified maxResults.
* `pageToken` - _optional_ - The token returned by the previous request.
* `playerId` - _required_ - A player ID. A value of me may be used in place of the authenticated player's ID.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Get high scores, and optionally ranks, in leaderboards for the currently authenticated player. For a specific time span, leaderboardId can be set to ALL to retrieve data for all leaderboards in a given time span.<br/>
> NOTE: You cannot ask for 'ALL' leaderboards and 'ALL' timeSpans in the same request; only one parameter may be set to 'ALL'.

*Tags:* `scores`

#### Input Parameters
* `includeRankType` - _optional_ - The types of ranks to return. If the parameter is omitted, no ranks will be returned.
    Possible values: ALL, PUBLIC, SOCIAL.
* `language` - _optional_ - The preferred language to use for strings returned by this method.
* `leaderboardId` - _required_ - The ID of the leaderboard. Can be set to 'ALL' to retrieve data for all leaderboards for this application.
* `maxResults` - _optional_ - The maximum number of leaderboard scores to return in the response. For any response, the actual number of leaderboard scores returned may be less than the specified maxResults.
* `pageToken` - _optional_ - The token returned by the previous request.
* `playerId` - _required_ - A player ID. A value of me may be used in place of the authenticated player's ID.
* `timeSpan` - _required_ - The time span for the scores and ranks you're requesting.
    Possible values: ALL, ALL_TIME, DAILY, WEEKLY.

### Get a list of quests for your application and the currently authenticated player.

*Tags:* `quests`

#### Input Parameters
* `language` - _optional_ - The preferred language to use for strings returned by this method.
* `maxResults` - _optional_ - The maximum number of quest resources to return in the response, used for paging. For any response, the actual number of quest resources returned may be less than the specified maxResults. Acceptable values are 1 to 50, inclusive. (Default: 50).
* `pageToken` - _optional_ - The token returned by the previous request.
* `playerId` - _required_ - A player ID. A value of me may be used in place of the authenticated player's ID.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Retrieves a list of snapshots created by your application for the player corresponding to the player ID.

*Tags:* `snapshots`

#### Input Parameters
* `language` - _optional_ - The preferred language to use for strings returned by this method.
* `maxResults` - _optional_ - The maximum number of snapshot resources to return in the response, used for paging. For any response, the actual number of snapshot resources returned may be less than the specified maxResults.
* `pageToken` - _optional_ - The token returned by the previous request.
* `playerId` - _required_ - A player ID. A value of me may be used in place of the authenticated player's ID.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Registers a push token for the current user and application.

*Tags:* `pushtokens`

#### Input Parameters
* `alt` - _optional_ - Data format for the response.
    Possible values: json.
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Removes a push token for the current user and application. Removing a non-existent push token will report success.

*Tags:* `pushtokens`

#### Input Parameters
* `alt` - _optional_ - Data format for the response.
    Possible values: json.
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Indicates that the currently authorized user will participate in the quest.

*Tags:* `quests`

#### Input Parameters
* `language` - _optional_ - The preferred language to use for strings returned by this method.
* `questId` - _required_ - The ID of the quest.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Report that a reward for the milestone corresponding to milestoneId for the quest corresponding to questId has been claimed by the currently authorized user.

*Tags:* `questMilestones`

#### Input Parameters
* `milestoneId` - _required_ - The ID of the milestone.
* `questId` - _required_ - The ID of the quest.
* `requestId` - _required_ - A numeric ID to ensure that the request is handled correctly across retries. Your client application must generate this ID randomly.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Checks whether the games client is out of date.

*Tags:* `revisions`

#### Input Parameters
* `clientRevision` - _required_ - The revision of the client SDK used by your application. Format:
[PLATFORM_TYPE]:[VERSION_NUMBER]. Possible values of PLATFORM_TYPE are:
 
- "ANDROID" - Client is running the Android SDK. 
- "IOS" - Client is running the iOS SDK. 
- "WEB_APP" - Client is running as a Web App.
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Returns invitations to join rooms.

*Tags:* `rooms`

#### Input Parameters
* `language` - _optional_ - The preferred language to use for strings returned by this method.
* `maxResults` - _optional_ - The maximum number of rooms to return in the response, used for paging. For any response, the actual number of rooms to return may be less than the specified maxResults.
* `pageToken` - _optional_ - The token returned by the previous request.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Create a room. For internal use by the Games SDK only. Calling this method directly is unsupported.

*Tags:* `rooms`

#### Input Parameters
* `language` - _optional_ - The preferred language to use for strings returned by this method.
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Get the data for a room.

*Tags:* `rooms`

#### Input Parameters
* `language` - _optional_ - The preferred language to use for strings returned by this method.
* `roomId` - _required_ - The ID of the room.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Decline an invitation to join a room. For internal use by the Games SDK only. Calling this method directly is unsupported.

*Tags:* `rooms`

#### Input Parameters
* `language` - _optional_ - The preferred language to use for strings returned by this method.
* `roomId` - _required_ - The ID of the room.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Dismiss an invitation to join a room. For internal use by the Games SDK only. Calling this method directly is unsupported.

*Tags:* `rooms`

#### Input Parameters
* `roomId` - _required_ - The ID of the room.
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Join a room. For internal use by the Games SDK only. Calling this method directly is unsupported.

*Tags:* `rooms`

#### Input Parameters
* `language` - _optional_ - The preferred language to use for strings returned by this method.
* `roomId` - _required_ - The ID of the room.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Leave a room. For internal use by the Games SDK only. Calling this method directly is unsupported.

*Tags:* `rooms`

#### Input Parameters
* `language` - _optional_ - The preferred language to use for strings returned by this method.
* `roomId` - _required_ - The ID of the room.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Updates sent by a client reporting the status of peers in a room. For internal use by the Games SDK only. Calling this method directly is unsupported.

*Tags:* `rooms`

#### Input Parameters
* `language` - _optional_ - The preferred language to use for strings returned by this method.
* `roomId` - _required_ - The ID of the room.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Retrieves the metadata for a given snapshot ID.

*Tags:* `snapshots`

#### Input Parameters
* `language` - _optional_ - The preferred language to use for strings returned by this method.
* `snapshotId` - _required_ - The ID of the snapshot.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Returns turn-based matches the player is or was involved in.

*Tags:* `turnBasedMatches`

#### Input Parameters
* `includeMatchData` - _optional_ - True if match data should be returned in the response. Note that not all data will necessarily be returned if include_match_data is true; the server may decide to only return data for some of the matches to limit download size for the client. The remainder of the data for these matches will be retrievable on request.
* `language` - _optional_ - The preferred language to use for strings returned by this method.
* `maxCompletedMatches` - _optional_ - The maximum number of completed or canceled matches to return in the response. If not set, all matches returned could be completed or canceled.
* `maxResults` - _optional_ - The maximum number of matches to return in the response, used for paging. For any response, the actual number of matches to return may be less than the specified maxResults.
* `pageToken` - _optional_ - The token returned by the previous request.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Create a turn-based match.

*Tags:* `turnBasedMatches`

#### Input Parameters
* `language` - _optional_ - The preferred language to use for strings returned by this method.
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Returns turn-based matches the player is or was involved in that changed since the last sync call, with the least recent changes coming first. Matches that should be removed from the local cache will have a status of MATCH_DELETED.

*Tags:* `turnBasedMatches`

#### Input Parameters
* `includeMatchData` - _optional_ - True if match data should be returned in the response. Note that not all data will necessarily be returned if include_match_data is true; the server may decide to only return data for some of the matches to limit download size for the client. The remainder of the data for these matches will be retrievable on request.
* `language` - _optional_ - The preferred language to use for strings returned by this method.
* `maxCompletedMatches` - _optional_ - The maximum number of completed or canceled matches to return in the response. If not set, all matches returned could be completed or canceled.
* `maxResults` - _optional_ - The maximum number of matches to return in the response, used for paging. For any response, the actual number of matches to return may be less than the specified maxResults.
* `pageToken` - _optional_ - The token returned by the previous request.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Get the data for a turn-based match.

*Tags:* `turnBasedMatches`

#### Input Parameters
* `includeMatchData` - _optional_ - Get match data along with metadata.
* `language` - _optional_ - The preferred language to use for strings returned by this method.
* `matchId` - _required_ - The ID of the match.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Cancel a turn-based match.

*Tags:* `turnBasedMatches`

#### Input Parameters
* `matchId` - _required_ - The ID of the match.
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Decline an invitation to play a turn-based match.

*Tags:* `turnBasedMatches`

#### Input Parameters
* `language` - _optional_ - The preferred language to use for strings returned by this method.
* `matchId` - _required_ - The ID of the match.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Dismiss a turn-based match from the match list. The match will no longer show up in the list and will not generate notifications.

*Tags:* `turnBasedMatches`

#### Input Parameters
* `matchId` - _required_ - The ID of the match.
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Finish a turn-based match. Each player should make this call once, after all results are in. Only the player whose turn it is may make the first call to Finish, and can pass in the final match state.

*Tags:* `turnBasedMatches`

#### Input Parameters
* `language` - _optional_ - The preferred language to use for strings returned by this method.
* `matchId` - _required_ - The ID of the match.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Join a turn-based match.

*Tags:* `turnBasedMatches`

#### Input Parameters
* `language` - _optional_ - The preferred language to use for strings returned by this method.
* `matchId` - _required_ - The ID of the match.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Leave a turn-based match when it is not the current player's turn, without canceling the match.

*Tags:* `turnBasedMatches`

#### Input Parameters
* `language` - _optional_ - The preferred language to use for strings returned by this method.
* `matchId` - _required_ - The ID of the match.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Leave a turn-based match during the current player's turn, without canceling the match.

*Tags:* `turnBasedMatches`

#### Input Parameters
* `language` - _optional_ - The preferred language to use for strings returned by this method.
* `matchId` - _required_ - The ID of the match.
* `matchVersion` - _required_ - The version of the match being updated.
* `pendingParticipantId` - _optional_ - The ID of another participant who should take their turn next. If not set, the match will wait for other player(s) to join via automatching; this is only valid if automatch criteria is set on the match with remaining slots for automatched players.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Create a rematch of a match that was previously completed, with the same participants. This can be called by only one player on a match still in their list; the player must have called Finish first. Returns the newly created match; it will be the caller's turn.

*Tags:* `turnBasedMatches`

#### Input Parameters
* `language` - _optional_ - The preferred language to use for strings returned by this method.
* `matchId` - _required_ - The ID of the match.
* `requestId` - _optional_ - A randomly generated numeric ID for each request specified by the caller. This number is used at the server to ensure that the request is handled correctly across retries.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Commit the results of a player turn.

*Tags:* `turnBasedMatches`

#### Input Parameters
* `language` - _optional_ - The preferred language to use for strings returned by this method.
* `matchId` - _required_ - The ID of the match.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

## License

**flow**ground :- Telekom iPaaS / googleapis-com-games-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
