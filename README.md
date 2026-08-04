# Steam (steam)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Steam is Valve's PC gaming platform and digital distribution storefront. Valve exposes the Steamworks Web API at https://api.steampowered.com/ — a constellation of HTTP interfaces for games, players, friends, achievements, items, the economy, leaderboards, remote storage, and the Steam Workshop. A subset of read-only interfaces are public (with a Steam Web API key); the full Steamworks set requires a publisher account and partner-restricted methods. There is no per-call fee for the Steamworks Web API itself; Valve monetizes through a $100 Steam Direct submission fee per product and a revenue share on store sales.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/steam/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/steam/refs/heads/main/apis.yml)

## Tags

- Gaming
- Valve
- Distribution
- Steamworks
- Marketplace
- Web API

## Timestamps

- **Created:** 2026-05-08
- **Modified:** 2026-05-08

## APIs

### ISteamNews

ISteamNews exposes per-game news feeds via GetNewsForApp. Path pattern http://api.steampowered.com/ISteamNews/<method>/v<version>/.

#### Tags

- News
- Feeds
- Public

#### Properties

- [Documentation](https://steamcommunity.com/dev)
- [API Reference](https://partner.steamgames.com/doc/webapi)
- [Postman Collection](collections/steam.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/steam.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### ISteamUserStats

ISteamUserStats provides global achievement percentages, schema for game stats and achievements, and per-user achievement / stats retrieval (GetGlobalAchievementPercentagesForApp, GetSchemaForGame, GetUserStatsForGame, GetPlayerAchievements, etc.).

#### Tags

- Stats
- Achievements
- Global Stats
- Schema

#### Properties

- [API Reference](https://partner.steamgames.com/doc/webapi/ISteamUserStats)
- [Postman Collection](collections/steam.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/steam.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### ISteamUser

ISteamUser exposes player profile, friend list, and ban-status endpoints (GetPlayerSummaries, GetFriendList, GetPlayerBans, ResolveVanityURL).

#### Tags

- Users
- Profiles
- Friends
- Bans

#### Properties

- [API Reference](https://partner.steamgames.com/doc/webapi/ISteamUser)
- [Postman Collection](collections/steam.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/steam.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### ISteamUserAuth

ISteamUserAuth issues and validates Steam session tickets (AuthenticateUserTicket, AuthenticateUser) used by partner servers to verify a connecting player's Steam identity.

#### Tags

- Authentication
- Sessions
- Tickets

#### Properties

- [API Reference](https://partner.steamgames.com/doc/webapi/ISteamUserAuth)
- [Postman Collection](collections/steam.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/steam.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### ISteamApps

ISteamApps exposes catalog and server queries (GetAppList, GetServersAtAddress, UpToDateCheck) used to enumerate Steam applications and validate version state.

#### Tags

- Apps
- Catalog
- Servers

#### Properties

- [API Reference](https://partner.steamgames.com/doc/webapi/ISteamApps)
- [Postman Collection](collections/steam.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/steam.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### ISteamCommunity

ISteamCommunity provides restricted access to Steam Community features (e.g., ReportAbuse) for trusted partners.

#### Tags

- Community
- Reports

#### Properties

- [API Reference](https://partner.steamgames.com/doc/webapi/ISteamCommunity)
- [Postman Collection](collections/steam.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/steam.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### ISteamEconomy

ISteamEconomy is a secondary economy-system interface (GetAssetClassInfo, GetAssetPrices, FinalizeAssetTransaction) used to look up asset metadata and pricing for in-game items.

#### Tags

- Economy
- Trades
- Asset Class

#### Properties

- [API Reference](https://partner.steamgames.com/doc/webapi/ISteamEconomy)
- [Postman Collection](collections/steam.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/steam.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### IGameInventory

IGameInventory is the primary inventory-economy interface used by partner servers to manipulate item ownership (AddItem, ConsumeItem, GetUserInventory, GetItemDefArchive).

#### Tags

- Inventory
- Items
- Economy

#### Properties

- [API Reference](https://partner.steamgames.com/doc/webapi/IGameInventory)
- [Postman Collection](collections/steam.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/steam.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### IInventoryService

IInventoryService is the modern Steam Inventory Service interface used to add/remove/exchange items, manage definitions, and query inventories at scale.

#### Tags

- Inventory
- Items
- Service

#### Properties

- [API Reference](https://partner.steamgames.com/doc/webapi/IInventoryService)
- [Postman Collection](collections/steam.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/steam.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### ISteamGameServer

ISteamGameServer issues and manages persistent Game Server Login Tokens (GSLTs) used by dedicated game servers to authenticate to Steam.

#### Tags

- Game Servers
- Sessions
- Login Tokens

#### Properties

- [API Reference](https://partner.steamgames.com/doc/webapi/ISteamGameServer)
- [Postman Collection](collections/steam.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/steam.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### ISteamRemoteStorage

ISteamRemoteStorage exposes Steam Cloud and UGC (user-generated content) storage endpoints — fetching files, retrieving UGC details, and listing published files.

#### Tags

- Remote Storage
- Cloud Saves
- UGC

#### Properties

- [API Reference](https://partner.steamgames.com/doc/webapi/ISteamRemoteStorage)
- [Postman Collection](collections/steam.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/steam.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### ISteamLeaderboards

ISteamLeaderboards manages per-app leaderboards — creation, score upload/reset, and entry retrieval.

#### Tags

- Leaderboards
- Scores

#### Properties

- [API Reference](https://partner.steamgames.com/doc/webapi/ISteamLeaderboards)
- [Postman Collection](collections/steam.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/steam.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### IPlayerService

IPlayerService exposes player-centric endpoints (GetOwnedGames, GetRecentlyPlayedGames, GetSteamLevel, GetBadges, IsPlayingSharedGame).

#### Tags

- Players
- Owned Games
- Recently Played
- Badges

#### Properties

- [API Reference](https://partner.steamgames.com/doc/webapi/IPlayerService)
- [Postman Collection](collections/steam.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/steam.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### IGameNotificationsService

IGameNotificationsService delivers turn-based and prompt-style in-game notifications to players (UpdateNotificationSettings, UserCreateSession).

#### Tags

- Notifications
- In-Game

#### Properties

- [API Reference](https://partner.steamgames.com/doc/webapi/IGameNotificationsService)
- [Postman Collection](collections/steam.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/steam.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### ISteamWebAPIUtil

ISteamWebAPIUtil provides helper endpoints — GetServerInfo (Steam server time/version) and GetSupportedAPIList (interfaces and methods callable by the API key).

#### Tags

- Utility
- Server Info
- Schema

#### Properties

- [API Reference](https://partner.steamgames.com/doc/webapi/ISteamWebAPIUtil)
- [Postman Collection](collections/steam.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/steam.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### IPublishedFileService

IPublishedFileService manages Steam Workshop / UGC published files — query, vote, change visibility, manage tags and previews.

#### Tags

- Workshop
- UGC
- Published Files

#### Properties

- [API Reference](https://partner.steamgames.com/doc/webapi/IPublishedFileService)
- [Postman Collection](collections/steam.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/steam.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### IBroadcastService

IBroadcastService exposes Steam game-broadcast metadata and stream-discovery endpoints used for in-app broadcast lookups.

#### Tags

- Broadcast
- Streaming
- Game Live

#### Properties

- [API Reference](https://partner.steamgames.com/doc/webapi/IBroadcastService)
- [Postman Collection](collections/steam.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/steam.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Steam Store API

An unofficial-but-widely-used set of storefront endpoints (https://store.steampowered.com/api/) returns app details, package details, currency conversion, and feature lists. Used by community sites and third-party catalogs.

#### Tags

- Store
- Pricing
- App Details

#### Properties

- [API Reference](https://store.steampowered.com/api/appdetails)
- [Postman Collection](collections/steam.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/steam.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### ISteamCheckout

ISteamCheckout is the partner-only interface used to initiate, authorize, and finalize in-game microtransaction purchases through Steam Checkout.

#### Tags

- Checkout
- In-Game Purchases
- Microtransactions

#### Properties

- [API Reference](https://partner.steamgames.com/doc/webapi/ISteamCheckout)
- [Postman Collection](collections/steam.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/steam.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### ISteamMicroTxn

ISteamMicroTxn / ISteamMicroTxnSandbox handle the full microtransaction lifecycle — InitTxn, FinalizeTxn, GetReport, RefundTxn, QueryTxn — used by F2P and live-service titles.

#### Tags

- Microtransactions
- Payments
- Refunds

#### Properties

- [API Reference](https://partner.steamgames.com/doc/webapi/ISteamMicroTxn)
- [Postman Collection](collections/steam.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/steam.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### ISteamDeepLinkService

ISteamDeepLinkService creates and resolves time-limited deep links into the Steam client and store, useful for marketing campaigns and partner referrals.

#### Tags

- Deep Links
- Marketing

#### Properties

- [API Reference](https://partner.steamgames.com/doc/webapi/ISteamDeepLinkService)
- [Postman Collection](collections/steam.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/steam.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [GitHub Organization](https://github.com/valvesoftware)
- [LinkedIn](https://www.linkedin.com/company/valvesoftware)
- [Website](https://store.steampowered.com/)
- [Documentation](https://partner.steamgames.com/doc/home)
- [API Reference](https://partner.steamgames.com/doc/webapi)
- [Public  Web  A P I  Docs](https://steamcommunity.com/dev)
- [Getting Started](https://partner.steamgames.com/doc/gettingstarted)
- [A P I  Key  Registration](https://steamcommunity.com/dev/apikey)
- [Steam  Direct](https://partner.steamgames.com/steamdirect)
- [Steamworks  S D K](https://partner.steamgames.com/doc/sdk)
- [Steam  Workshop  Docs](https://partner.steamgames.com/doc/features/workshop)
- [Sign Up](https://partner.steamgames.com/)
- [Login](https://store.steampowered.com/login/)
- [Status Page](https://steamstat.us/)
- [Status ( Official)](https://store.steampowered.com/stats/)
- [Steam  Store](https://store.steampowered.com/)
- [Steam  Community](https://steamcommunity.com/)
- [Steamworks  Discord](https://discord.gg/steamworks)
- [Steamworks  Documentation](https://partner.steamgames.com/doc)
- [Privacy Policy](https://store.steampowered.com/privacy_agreement/)
- [Subscriber  Agreement](https://store.steampowered.com/subscriber_agreement/)
- [Steam  Web  A P I  Terms of  Use](https://steamcommunity.com/dev/apiterms)
- [Steamworks  Forum](https://steamcommunity.com/groups/steamworks)
- [Plans](plans/steam-plans-pricing.yml)
- [Rate Limits](rate-limits/steam-rate-limits.yml)
- [Fin Ops](finops/steam-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
