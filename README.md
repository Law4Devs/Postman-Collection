# Law4Devs API — Postman Collection

> **Structured EU regulatory compliance data, ready to explore.**
> 22 endpoints · 12 folders · SDKs · OpenAPI 3.0.3 · REST · JSON

---

<div align="center">
  <img src="https://res.cloudinary.com/dp9q7kbap/image/upload/v1773262750/logo_o9usas.png" width="300" alt="Law4Devs Logo">
  <br>
  <img src="https://res.cloudinary.com/dp9q7kbap/image/upload/v1773262738/law4devs-title_bmd09z.svg" width="300" alt="Law4Devs">
  <br>
  <img src="https://res.cloudinary.com/dp9q7kbap/image/upload/v1773262738/law4devs-subtitle_eygff7.svg" width="600" alt="Structured EU regulatory compliance data for developers">
</div>

**Law4Devs** is a structured data API that makes EU regulatory compliance accessible to developers. It parses and exposes all 19 major EU digital regulations — including the CRA, NIS2, GDPR, DORA, AI Act, DSA, and more — as machine-readable JSON: articles, recitals, requirements, compliance deadlines, annexes, and semantic tags, all under one consistent API surface.

The goal is simple: instead of reading hundreds of pages of legal text, developers and compliance engineers can query the exact articles, requirements, and deadlines that apply to their product or organisation, filter by stakeholder role or semantic tag, and integrate compliance data directly into their tooling or dashboards.

---

## About This Collection

This Postman collection covers the full **Law4Devs REST API (v1)** — all public endpoints, organised into folders by resource type. Every request is pre-configured with the `{{base_url}}` environment variable and meaningful example values for path and query parameters, so you can start making real requests in seconds.

**Included files:**

| File | Purpose |
|------|---------|
| `law4devs.postman_collection.json` | Postman Collection v2.1 — all 22 API endpoints |
| `law4devs.postman_environment.json` | Environment with `base_url` pre-set with prod endpoint |

---

## Getting Started

### 1. Import the collection

In Postman, click **Import** → **File** and select:

```
law4devs.postman_collection.json
```

### 2. Import the environment

Click **Import** again and select:

```
law4devs.postman_environment.json
```

Then open the **Environments** panel (top-right selector) and choose **Law4Devs — Local**.

### 3. Send your first request

Open the **Health** folder and run `GET Health Check`. You should receive:

```json
{
  "data": {
    "status": "ok",
    "database": "connected"
  }
}
```

If the request succeeds, you're all set. Browse the other folders to explore the full API.

---

## Collection Structure

| Folder | Endpoints | Description |
|--------|-----------|-------------|
| **Health** | 1 | API and database liveness check |
| **Frameworks** | 2 | List all 19 EU regulations; fetch one by slug |
| **Articles** | 3 | Paginated articles per framework, detail view, related articles |
| **Recitals** | 2 | Preamble paragraphs per framework |
| **Requirements** | 2 | Extracted compliance requirements (global and per-framework) |
| **Annexes** | 2 | Technical annexes per framework |
| **Compliance** | 2 | Compliance deadlines (global and per-framework) |
| **Stats** | 2 | Coverage statistics (global and per-framework) |
| **Search** | 1 | Full-text search with faceted filtering |
| **Tags** | 2 | Semantic tags — list all, fetch one by slug |
| **Changelog** | 2 | Content update history (global and per-framework) |
| **Compare** | 1 | Cross-framework article comparison |

---

## Environment Variables

| Variable | Default | Description |
|----------|---------|-------------|
| `base_url` | `https://api.law4devs.eu` | Base URL of the Law4Devs API server (no trailing slash). |

---

## API Overview

All endpoints are under `/v1/`. Responses follow a consistent envelope:

```
GET  /v1/health
GET  /v1/frameworks
GET  /v1/frameworks/:slug
GET  /v1/frameworks/:slug/articles
GET  /v1/frameworks/:slug/articles/:article_number
GET  /v1/frameworks/:slug/articles/:article_number/related
GET  /v1/frameworks/:slug/recitals
GET  /v1/frameworks/:slug/recitals/:recital_number
GET  /v1/frameworks/:slug/requirements
GET  /v1/requirements
GET  /v1/frameworks/:slug/annexes
GET  /v1/frameworks/:slug/annexes/:annex_number
GET  /v1/frameworks/:slug/compliance/deadlines
GET  /v1/compliance/deadlines
GET  /v1/frameworks/:slug/stats
GET  /v1/stats
GET  /v1/search
GET  /v1/tags
GET  /v1/tags/:slug
GET  /v1/frameworks/:slug/changelog
GET  /v1/changelog
GET  /v1/compare
```

**Framework slugs** (use in `:slug` path parameters):

`cra` · `nis2` · `dora` · `gdpr` · `ai_act` · `eidas` · `dsa` · `dma` · `data_act` · `dga` · `eidas2` · `cer` · `psd2` · `mica` · `cybersecurity_act` · `eprivacy` · `red` · `csrd` · `nis1`

### Response envelopes

**Paginated list:**
```json
{
  "data": [ ... ],
  "meta": { "api_version": "1.0", "total": 71, "page": 1, "per_page": 20, "pages": 4 },
  "links": { "next": "?page=2&per_page=20", "prev": null }
}
```

**Detail object:**
```json
{ "data": { ... } }
```

**Error:**
```json
{ "error": { "code": "NOT_FOUND", "message": "Framework 'xyz' not found." } }
```

---

## Pagination

All list endpoints accept:

| Parameter | Default | Range | Description |
|-----------|---------|-------|-------------|
| `page` | `1` | ≥ 1 | Page number |
| `per_page` | `20` | 1 – 100 | Results per page |

Invalid values return `400 INVALID_PARAM`.

---

## Resources

| Resource | URL |
|----------|-----|
| Full Documentation | `https://docs.law4devs.eu/`  |
| Interactive docs (Swagger UI) | `https://api.law4devs.eu/docs` |
| Reference docs (ReDoc) | `https://api.law4devs.eu/redoc` |
| Raw OpenAPI 3.0.3 spec (JSON) | `https://api.law4devs.eu/v1/openapi.json` |

---

*Law4Devs — making EU compliance programmable.*
