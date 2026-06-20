# TwelveLabs (twelvelabs)

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
