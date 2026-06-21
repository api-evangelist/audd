# AudD (audd)

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
