# Wahoo Fitness (wahoo)

Wahoo Fitness is an Atlanta, Georgia endurance-training hardware and software company building cycling and run-training products: the ELEMNT family of GPS bike computers (ACE, ROAM, BOLT), the KICKR family of smart trainers and bikes (KICKR BIKE PRO/SHIFT, KICKR MOVE, KICKR CORE, KICKR ROLLR, KICKR RUN treadmill), TICKR and TRACKR heart-rate monitors and sensors (including TRACKR RADAR rear-facing radar), and SPEEDPLAY road and power pedals. Wahoo publishes a public Cloud API at api.wahooligan.com that allows third-party applications to authenticate Wahoo users via OAuth 2.0 and read/write user profiles, workouts, workout summaries, FIT-file uploads, structured workout plans, GPS routes, and cycling power zones. The Cloud API delivers workout_summary webhook events when the offline_data scope is granted. Companion AppleHealth / native iOS and Android APIs round out the developer surface; access is gated by the Wahoo API Agreement and an app-approval workflow that promotes integrations from sandbox to production.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/wahoo/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/wahoo/refs/heads/main/apis.yml)

## Scope

- **Type:** Index
- **Position:** Provider
- **Access:** 3rd-Party

## Tags

- Fitness
- Cycling
- Endurance Training
- Bike Computers
- Smart Trainers
- Indoor Cycling
- Heart Rate
- Power Meters
- GPS
- Wearables
- Hardware
- FIT Files
- Webhooks
- OAuth

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## APIs

### Wahoo Cloud API

OAuth 2.0 REST API that connects Wahoo users to third-party mobile and web applications. Manages user profiles, workouts, workout summaries, FIT-file uploads, structured workout plans, GPS routes, and cycling power zones. Delivers workout_summary webhook events when offline_data scope is granted. Sandbox apps are promoted to production after Wahoo review.

- **Human URL:** [https://cloud-api.wahooligan.com/](https://cloud-api.wahooligan.com/)
- **Base URL:** `https://api.wahooligan.com`

#### Tags

- Fitness
- Cycling
- Workouts
- OAuth

#### Properties

- [Documentation](https://cloud-api.wahooligan.com/)
- [Documentation](https://developers.wahooligan.com/cloud)
- [Sign Up](https://developers.wahooligan.com/)
- [Terms of Service](https://www.wahoofitness.com/wahoo-api-agreement)
- [OpenAPI](openapi/wahoo-cloud-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/wahoo-cloud-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/wahoo-cloud-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [AsyncAPI](asyncapi/wahoo-webhooks-asyncapi.yml) — [AsyncAPI Specification](https://www.asyncapi.com/docs/reference/specification/latest)
- [JSON Schema](json-schema/wahoo-workout-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/wahoo-workout-summary-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON-LD](json-ld/wahoo-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Plans](plans/wahoo-plans-pricing.yml)
- [Rate Limits](rate-limits/wahoo-rate-limits.yml)
- [Vocabulary](vocabulary/wahoo-vocabulary.yml)
- [Example](examples/wahoo-workout-summary-event-example.json)
- [Example](examples/wahoo-power-zones-example.json)
- [Webhook](https://cloud-api.wahooligan.com/#webhooks)
- [Authentication](https://cloud-api.wahooligan.com/#authentication)

### Wahoo iOS API

Native iOS SDK for interacting with Wahoo devices directly over BLE/ANT+ and integrating with the Wahoo Cloud. Documented at the Wahoo developer portal under the iOS product. Access is gated by the Wahoo API Agreement and an app-approval workflow.

- **Human URL:** [https://developers.wahooligan.com/](https://developers.wahooligan.com/)

#### Tags

- Fitness
- Cycling
- iOS
- SDK

#### Properties

- [Documentation](https://developers.wahooligan.com/)
- [Sign Up](https://developers.wahooligan.com/)
- [Postman Collection](collections/wahoo-cloud-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/wahoo-cloud-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Wahoo Android API

Native Android SDK for interacting with Wahoo devices over BLE/ANT+ and integrating with the Wahoo Cloud. Documented at the Wahoo developer portal under the Android product. Access is gated by the Wahoo API Agreement and an app-approval workflow.

- **Human URL:** [https://developers.wahooligan.com/](https://developers.wahooligan.com/)

#### Tags

- Fitness
- Cycling
- Android
- SDK

#### Properties

- [Documentation](https://developers.wahooligan.com/)
- [Sign Up](https://developers.wahooligan.com/)
- [Postman Collection](collections/wahoo-cloud-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/wahoo-cloud-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Website](https://www.wahoofitness.com/)
- [Developer Portal](https://developers.wahooligan.com/)
- [API Reference](https://cloud-api.wahooligan.com/)
- [A P I Agreement](https://www.wahoofitness.com/wahoo-api-agreement)
- [Git Hub](https://github.com/wahoofitness)
- [Support](https://support.wahoofitness.com/)
- [Training App](https://www.wahoofitness.com/devices/training-app)
- [Wahoo X](https://wahooxsystm.com/)
- [Blog](https://www.wahoofitness.com/blog)
- [Twitter](https://twitter.com/wahoofitness)
- [Instagram](https://www.instagram.com/wahoofitness/)
- [YouTube](https://www.youtube.com/user/WahooFitness)
- [LinkedIn](https://www.linkedin.com/company/wahoo-fitness/)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
