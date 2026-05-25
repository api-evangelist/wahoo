# Wahoo Fitness (wahoo)

Wahoo Fitness is an Atlanta, Georgia endurance-training hardware and software company building cycling and run-training products: ELEMNT GPS bike computers (ACE, ROAM, BOLT), KICKR smart trainers and bikes (KICKR BIKE PRO/SHIFT, KICKR MOVE, KICKR CORE, KICKR ROLLR), the KICKR RUN smart treadmill, TICKR and TRACKR heart-rate monitors and sensors (including TRACKR RADAR rear-facing radar), and SPEEDPLAY road and power pedals. The public Wahoo Cloud API at `api.wahooligan.com` exposes OAuth 2.0 access to user profiles, workouts, workout summaries, FIT-file uploads, structured plans, GPS routes, and cycling power zones, plus a `workout_summary` webhook.

**URL:** [Visit APIs.json](https://raw.githubusercontent.com/api-evangelist/wahoo/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags

Fitness, Cycling, Endurance Training, Bike Computers, Smart Trainers, Indoor Cycling, Heart Rate, Power Meters, GPS, Wearables, Hardware, FIT Files, Webhooks, OAuth

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## APIs

### Wahoo Cloud API

OAuth 2.0 REST API connecting Wahoo users to third-party mobile and web apps. Manages user profiles, workouts, workout summaries, FIT-file uploads, structured workout plans, GPS routes, and cycling power zones; delivers `workout_summary` webhook events under the `offline_data` scope.

**Human URL:** [https://cloud-api.wahooligan.com/](https://cloud-api.wahooligan.com/)
**Base URL:** `https://api.wahooligan.com`

- [API Reference](https://cloud-api.wahooligan.com/)
- [Developer Portal — Cloud](https://developers.wahooligan.com/cloud)
- [Sign Up](https://developers.wahooligan.com/)
- [API Agreement](https://www.wahoofitness.com/wahoo-api-agreement)
- [OpenAPI](openapi/wahoo-cloud-api-openapi.yml)
- [AsyncAPI — Webhooks](asyncapi/wahoo-webhooks-asyncapi.yml)
- [JSON Schema — Workout](json-schema/wahoo-workout-schema.json)
- [JSON Schema — Workout Summary](json-schema/wahoo-workout-summary-schema.json)
- [JSON-LD Context](json-ld/wahoo-context.jsonld)
- [Plans](plans/wahoo-plans-pricing.yml)
- [Rate Limits](rate-limits/wahoo-rate-limits.yml)
- [Vocabulary](vocabulary/wahoo-vocabulary.yml)
- [Example — Workout Summary Webhook](examples/wahoo-workout-summary-event-example.json)
- [Example — Power Zones](examples/wahoo-power-zones-example.json)

#### Naftiko Capabilities

- [Users](capabilities/cloud-users.yaml)
- [Workouts](capabilities/cloud-workouts.yaml)
- [Workout File Uploads](capabilities/cloud-file-uploads.yaml)
- [Plans](capabilities/cloud-plans.yaml)
- [Routes](capabilities/cloud-routes.yaml)
- [Power Zones](capabilities/cloud-power-zones.yaml)
- [Permissions](capabilities/cloud-permissions.yaml)

#### OAuth Scopes

`email`, `user_read`, `user_write`, `workouts_read`, `workouts_write`, `offline_data`, `plans_read`, `plans_write`, `power_zones_read`, `power_zones_write`, `routes_read`, `routes_write`

#### Rate Limits

| Tier | 5 min | 1 hour | 1 day |
|---|---|---|---|
| Sandbox | 25 | 100 | 250 |
| Production | 200 | 1,000 | 5,000 |

Authentication, token refresh, and FIT-file downloads are exempt. Starting **2026-01-01**, apps are capped at **10 unrevoked access tokens per user**.

#### Webhook Retry Policy

`workout_summary` events are retried at **30 min → 4 h → 24 h → 72 h** until a `200` response is received; then dropped.

### Wahoo iOS API

Native iOS SDK for interacting with Wahoo devices over BLE/ANT+ and integrating with the Wahoo Cloud. Documented in the Wahoo developer portal under the iOS product. Access is gated by the Wahoo API Agreement and an app-approval workflow.

- [Developer Portal](https://developers.wahooligan.com/)

### Wahoo Android API

Native Android SDK for interacting with Wahoo devices over BLE/ANT+ and integrating with the Wahoo Cloud. Documented in the Wahoo developer portal under the Android product. Access is gated by the Wahoo API Agreement and an app-approval workflow.

- [Developer Portal](https://developers.wahooligan.com/)

## Common Links

- [Website](https://www.wahoofitness.com/)
- [Developer Portal](https://developers.wahooligan.com/)
- [API Reference](https://cloud-api.wahooligan.com/)
- [API Agreement](https://www.wahoofitness.com/wahoo-api-agreement)
- [GitHub — wahoofitness](https://github.com/wahoofitness)
- [Support](https://support.wahoofitness.com/)
- [Wahoo X / SYSTM Training App](https://wahooxsystm.com/)
- [Blog](https://www.wahoofitness.com/blog)
- [Twitter](https://twitter.com/wahoofitness)
- [LinkedIn](https://www.linkedin.com/company/wahoo-fitness/)
- [YouTube](https://www.youtube.com/user/WahooFitness)

## Solutions

- Sync Wahoo workouts into a third-party training platform.
- Push structured workout plans from a coaching service into a user's ELEMNT bike computer.
- Push GPS routes from a route-planning service into ELEMNT for turn-by-turn navigation.
- Maintain cycling power zones synced to FTP test results.
- Stream `workout_summary` webhook events into analytics, coaching, or social-fitness platforms.
- Upload raw FIT files captured by non-Wahoo devices into a user's Wahoo workout history.

## Integrations

- **Garmin** — FIT-file format interoperability
- **Strava** — workout sync via third-party bridges
- **TrainingPeaks** — plan and workout interoperability
- **Zwift** — KICKR trainer control over BLE/ANT+ FE-C (outside the Cloud API)
- **Apple Health** — via iOS app

## Maintainer

Kin Lane — [kin@apievangelist.com](mailto:kin@apievangelist.com)
