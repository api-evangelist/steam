# Steam (steam)

Steam is Valve's PC gaming platform and digital distribution storefront. The Steamworks Web API at https://api.steampowered.com/ is a constellation of HTTP interfaces for games, players, friends, achievements, items, the economy, leaderboards, remote storage, and the Steam Workshop.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/steam/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=steam-api-evangelist&utm_content=repo)

## Type

- **x-type:** company

## Tags

 - Gaming, Valve, Distribution, Steamworks, Marketplace, Web API

## Timestamps

- **Created:** 2026-05-08
- **Modified:** 2026-05-08

## APIs

| Interface | Description |
|---|---|
| ISteamNews | Per-game news feeds |
| ISteamUserStats | Achievements + stats schema/global/per-user |
| ISteamUser | Player profiles, friends, bans |
| ISteamUserAuth | Session ticket authentication |
| ISteamApps | App catalog and server queries |
| ISteamCommunity | Restricted Community ops (e.g. ReportAbuse) |
| ISteamEconomy | Asset class info / pricing / transactions |
| IGameInventory | Primary inventory-economy partner interface |
| IInventoryService | Modern Steam Inventory Service |
| ISteamGameServer | Game Server Login Tokens (GSLTs) |
| ISteamRemoteStorage | Steam Cloud + UGC storage |
| ISteamLeaderboards | Per-app leaderboards |
| IPlayerService | Player-centric data (owned games, level, etc.) |
| IGameNotificationsService | In-game prompt/turn notifications |
| ISteamWebAPIUtil | Server time, supported-API list |
| IPublishedFileService | Steam Workshop / UGC published files |
| IBroadcastService | Steam game-broadcast metadata |
| Steam Store API | Storefront app/package details (unofficial) |
| ISteamCheckout | In-game microtransaction checkout |
| ISteamMicroTxn | Microtransaction lifecycle (init/finalize/refund/query) |
| ISteamDeepLinkService | Time-limited Steam deep links |

## Common Properties

- [Website](https://store.steampowered.com/)
- [Steamworks Documentation](https://partner.steamgames.com/doc/home)
- [Web API Reference](https://partner.steamgames.com/doc/webapi)
- [Public Web API Docs](https://steamcommunity.com/dev)
- [API Key Registration](https://steamcommunity.com/dev/apikey)
- [Steam Direct](https://partner.steamgames.com/steamdirect)
- [Plans](plans/steam-plans-pricing.yml) — API Commons Plans 0.1 (reconciled)
- [RateLimits](rate-limits/steam-rate-limits.yml) — API Commons Rate Limits 0.1 (reconciled)
- [FinOps](finops/steam-finops.yml) — FOCUS-aligned FinOps Framework 1.0 (reconciled, payouts perspective)

## Plans Summary

- **Public Steam Web API** — free with a Steam Web API key
- **Steam Direct (Game Publisher)** — $100 USD per-product submission fee (recoupable from first $1K adjusted gross)
- **Revenue Share** — graduated 30% / 25% / 20% across $0-$10M / $10M-$50M / $50M+ lifetime gross

## Rate Limits Summary

- **Steam Web API:** ~100,000 calls/day soft quota per API key
- **Storefront API:** ~1 request/second per IP safe ceiling
- **GetPlayerSummaries batch:** up to 100 SteamIDs per call
- **One Web API key per Steam account**

## Artifacts

| Artifact | Path |
|---|---|
| Plans | `plans/steam-plans-pricing.yml` |
| Rate Limits | `rate-limits/steam-rate-limits.yml` |
| FinOps | `finops/steam-finops.yml` |

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
