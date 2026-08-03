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
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

AudD is a music recognition service that identifies songs from audio files, URLs, or microphone input via a simple REST API. The api.audd.io API returns rich track metadata (artist, title, album, ISRC, links to Apple Music, Spotify, Deezer and more), supports recognition by humming/singing, lyrics search, and an enterprise endpoint for scanning long audio and video files.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/audd/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/audd/refs/heads/main/apis.yml)

## Tags

- Music
- Music Recognition
- Audio
- Fingerprinting
- Lyrics

## Timestamps

- **Created:** 2026-06-21
- **Modified:** 2026-06-21

## APIs

### AudD Music Recognition API

Identifies music from an audio file upload, a remote audio/video URL, or base64-encoded audio. Returns artist, title, album, release date, label, timecode, and optional metadata from Apple Music, Spotify, Deezer, Napster, and MusicBrainz.

- **Human URL:** [https://docs.audd.io/](https://docs.audd.io/)
- **Base URL:** `https://api.audd.io`

#### Tags

- Music Recognition
- Audio
- Fingerprinting

#### Properties

- [Documentation](https://docs.audd.io/)
- [API Reference](https://docs.audd.io/#recognize)
- [OpenAPI](openapi/audd-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/audd.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/audd.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### AudD Recognize with Offset API

Recognition variant that returns the offset (position) of the matched fragment within the submitted audio, also used as the method for recognition by humming or singing a melody.

- **Human URL:** [https://docs.audd.io/](https://docs.audd.io/)
- **Base URL:** `https://api.audd.io`

#### Tags

- Music Recognition
- Offset
- Timecode

#### Properties

- [Documentation](https://docs.audd.io/)
- [OpenAPI](openapi/audd-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/audd.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/audd.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### AudD Humming Recognition API

Identifies a song from a recording of a person humming or singing the melody, delivered through the recognizeWithOffset method against the AudD humming database.

- **Human URL:** [https://docs.audd.io/](https://docs.audd.io/)
- **Base URL:** `https://api.audd.io`

#### Tags

- Humming
- Music Recognition
- Melody

#### Properties

- [Documentation](https://docs.audd.io/)
- [OpenAPI](openapi/audd-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/audd.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/audd.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### AudD Enterprise File Scan API

Enterprise endpoint that scans hours- or days-long audio and video files in 12-second chunks, returning every matched song with timecodes, offsets, and detailed metadata. Supports skip, every, limit, and accurate_offsets controls.

- **Human URL:** [https://docs.audd.io/enterprise/](https://docs.audd.io/enterprise/)
- **Base URL:** `https://enterprise.audd.io`

#### Tags

- Enterprise
- File Scan
- Long Audio

#### Properties

- [Documentation](https://docs.audd.io/enterprise/)
- [OpenAPI](openapi/audd-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/audd.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/audd.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### AudD Lyrics API

Searches for song lyrics by title, artist, or an excerpt of the lyrics via the findLyrics method, returning matching songs with full lyrics and metadata.

- **Human URL:** [https://docs.audd.io/](https://docs.audd.io/)
- **Base URL:** `https://api.audd.io`

#### Tags

- Lyrics
- Search
- Metadata

#### Properties

- [Documentation](https://docs.audd.io/)
- [OpenAPI](openapi/audd-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/audd.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/audd.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [GitHub Organization](https://github.com/AudDMusic)
- [LinkedIn](https://www.linkedin.com/company/audd-io)
- [Website](https://audd.io/)
- [Documentation](https://docs.audd.io/)
- [Plans](plans/audd-plans-pricing.yml)
- [Rate Limits](rate-limits/audd-rate-limits.yml)
- [Fin Ops](finops/audd-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
