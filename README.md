# Wahoo Fitness (wahoo)

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
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
