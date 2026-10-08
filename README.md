# AudD (audd)

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

AudD is a music recognition service. Its REST API identifies songs from short audio clips, uploaded files or URLs on api.audd.io, scans audio and video files of any length on the enterprise endpoint (enterprise.audd.io), monitors live audio streams with results delivered by callback or longpoll, and adds an account's own tracks to a custom catalog (special access). Matches return track metadata (artist, title, album, ISRC) with optional Apple Music, Spotify, Deezer and MusicBrainz data.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/audd/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/audd/refs/heads/main/apis.yml)

## Tags

- Music
- Music Recognition
- Audio
- Fingerprinting

## Timestamps

- **Created:** 2026-06-21
- **Modified:** 2026-10-08

## APIs

### AudD Recognition API

Music recognition from a short clip, file or URL (api.audd.io), and the enterprise endpoint for audio and video files of any length (enterprise.audd.io).

- **Human URL:** [https://docs.audd.io/](https://docs.audd.io/)
- **Base URL:** `https://api.audd.io`

#### Tags

- Recognition

#### Properties

- [OpenAPI](openapi/audd-recognition-api-openapi.yml)
- [Documentation](https://docs.audd.io/)
- [API Reference](https://docs.audd.io/#recognize)
- [Documentation](https://docs.audd.io/enterprise/)
- [Postman Collection](collections/audd-recognition-api.postman_collection.json)
- [Open Collection](collections/audd-recognition-api.opencollection.json)

### AudD Custom Catalog API

Add your own tracks to a custom recognition catalog (special access).

- **Human URL:** [https://docs.audd.io/](https://docs.audd.io/)
- **Base URL:** `https://api.audd.io`

#### Tags

- Custom catalog

#### Properties

- [OpenAPI](openapi/audd-custom-catalog-api-openapi.yml)
- [Documentation](https://docs.audd.io/upload_audio_endpoint/)
- [Postman Collection](collections/audd-custom-catalog-api.postman_collection.json)
- [Open Collection](collections/audd-custom-catalog-api.opencollection.json)

### AudD Streams API

Live audio stream monitoring - add and manage streams, with recognition results delivered by callback URL or longpoll.

- **Human URL:** [https://docs.audd.io/](https://docs.audd.io/)
- **Base URL:** `https://api.audd.io`

#### Tags

- Streams

#### Properties

- [OpenAPI](openapi/audd-streams-api-openapi.yml)
- [Documentation](https://docs.audd.io/streams/)
- [Postman Collection](collections/audd-streams-api.postman_collection.json)
- [Open Collection](collections/audd-streams-api.opencollection.json)

## Common Properties

- [Agentic Access](agentic-access/audd-agentic-access.yml)
- [Domain Security](security/audd-domain-security.yml)
- [Authentication](authentication/audd-authentication.yml)
- [Git Hub Organization](https://github.com/AudDMusic)
- [Linked In](https://www.linkedin.com/company/audd-io)
- [Website](https://audd.io/)
- [Documentation](https://docs.audd.io/)
- [Well Known](well-known/audd-well-known.yml)
- [APICatalog](https://audd.io/.well-known/api-catalog)
- [Plans](plans/audd-plans-pricing.yml)
- [Rate Limits](rate-limits/audd-rate-limits.yml)
- [Fin Ops](finops/audd-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
