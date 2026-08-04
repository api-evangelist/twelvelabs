# TwelveLabs (twelvelabs)

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

TwelveLabs builds video-understanding foundation models (Marengo for search and embeddings, Pegasus for analyzing video and generating text). The TwelveLabs API lets developers upload and index video, run any-to-video semantic search, generate text from video (titles, topics, hashtags, summaries, chapters, highlights, and open-ended analysis), and create multimodal embeddings over a REST interface authenticated with an x-api-key header.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/twelvelabs/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/twelvelabs/refs/heads/main/apis.yml)

## Tags

- AI
- Video Understanding
- Multimodal
- Search
- Embeddings

## Timestamps

- **Created:** 2026-06-20
- **Modified:** 2026-06-20

## APIs

### TwelveLabs Indexes API

Create, list, retrieve, update, and delete video indexes, and manage the indexed videos within them. Each index is configured with the Marengo and/or Pegasus models and the visual/audio modalities to enable.

- **Human URL:** [https://docs.twelvelabs.io/v1.3/api-reference/indexes/list](https://docs.twelvelabs.io/v1.3/api-reference/indexes/list)
- **Base URL:** `https://api.twelvelabs.io/v1.3`

#### Tags

- Indexes
- Videos
- Catalog

#### Properties

- [Documentation](https://docs.twelvelabs.io/v1.3/docs/concepts/indexes)
- [API Reference](https://docs.twelvelabs.io/v1.3/api-reference/indexes/list)
- [OpenAPI](openapi/twelvelabs-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/twelvelabs.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/twelvelabs.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### TwelveLabs Tasks (Upload) API

Upload video by file or public URL and index it into a target index. Create, list, retrieve, and delete asynchronous video indexing tasks and poll their status (validating, pending, indexing, ready, failed).

- **Human URL:** [https://docs.twelvelabs.io/v1.3/api-reference/upload-content/tasks/create](https://docs.twelvelabs.io/v1.3/api-reference/upload-content/tasks/create)
- **Base URL:** `https://api.twelvelabs.io/v1.3`

#### Tags

- Tasks
- Upload
- Indexing

#### Properties

- [Documentation](https://docs.twelvelabs.io/v1.3/docs/filtering-indexes-and-tasks)
- [API Reference](https://docs.twelvelabs.io/v1.3/api-reference/upload-content/tasks/create)
- [OpenAPI](openapi/twelvelabs-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/twelvelabs.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/twelvelabs.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### TwelveLabs Search API

Any-to-video semantic search across an index using text and/or media (image) queries, powered by the Marengo model, with visual / audio / transcription search options, clip or video grouping, and token-paginated results.

- **Human URL:** [https://docs.twelvelabs.io/v1.3/api-reference/any-to-video-search/make-search-request](https://docs.twelvelabs.io/v1.3/api-reference/any-to-video-search/make-search-request)
- **Base URL:** `https://api.twelvelabs.io/v1.3`

#### Tags

- Search
- Semantic Search
- Marengo

#### Properties

- [Documentation](https://docs.twelvelabs.io/v1.3/docs/guides/search)
- [API Reference](https://docs.twelvelabs.io/v1.3/api-reference/any-to-video-search/make-search-request)
- [OpenAPI](openapi/twelvelabs-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/twelvelabs.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/twelvelabs.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### TwelveLabs Analyze / Generate API

Generate text from video with the Pegasus model - open-ended analysis via the sync /analyze endpoint (with optional NDJSON streaming), async analysis tasks for longer video, plus gist (titles, topics, hashtags) and summarize (summaries, chapters, highlights) generation.

- **Human URL:** [https://docs.twelvelabs.io/v1.3/api-reference/analyze-videos/analyze](https://docs.twelvelabs.io/v1.3/api-reference/analyze-videos/analyze)
- **Base URL:** `https://api.twelvelabs.io/v1.3`

#### Tags

- Analyze
- Generate
- Pegasus

#### Properties

- [Documentation](https://docs.twelvelabs.io/v1.3/docs/guides/generate-text-from-video/summaries-chapters-and-highlights)
- [API Reference](https://docs.twelvelabs.io/v1.3/api-reference/analyze-videos/analyze)
- [OpenAPI](openapi/twelvelabs-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [AsyncAPI](asyncapi/twelvelabs-asyncapi.yml) — [AsyncAPI Specification](https://www.asyncapi.com/docs/reference/specification/latest)
- [Postman Collection](collections/twelvelabs.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/twelvelabs.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### TwelveLabs Embed API

Create multimodal Marengo embeddings for text, image, audio, and video in one shared vector space - synchronously for short inputs and via asynchronous embedding tasks for longer audio and video, for use in search, RAG, classification, and recommendation pipelines.

- **Human URL:** [https://docs.twelvelabs.io/v1.3/api-reference/create-embeddings-v2/create-embeddings](https://docs.twelvelabs.io/v1.3/api-reference/create-embeddings-v2/create-embeddings)
- **Base URL:** `https://api.twelvelabs.io/v1.3`

#### Tags

- Embeddings
- Multimodal
- Marengo

#### Properties

- [Documentation](https://www.twelvelabs.io/blog/introducing-twelve-labs-embed-api-open-beta)
- [API Reference](https://docs.twelvelabs.io/v1.3/api-reference/create-embeddings-v2/create-embeddings)
- [OpenAPI](openapi/twelvelabs-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/twelvelabs.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/twelvelabs.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [GitHub Organization](https://github.com/twelvelabs-io)
- [LinkedIn](https://www.linkedin.com/company/twelvelabs)
- [Website](https://www.twelvelabs.io)
- [Documentation](https://docs.twelvelabs.io)
- [Plans](plans/twelvelabs-plans-pricing.yml)
- [Rate Limits](rate-limits/twelvelabs-rate-limits.yml)
- [Fin Ops](finops/twelvelabs-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
