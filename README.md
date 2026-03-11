# Law4Devs API — Postman Collection

> **Structured EU regulatory compliance data, ready to explore.**
> 22 endpoints · 12 folders · SDKs · OpenAPI 3.0.3 · REST · JSON

---

<div align="center">
  <img src="https://private-user-images.githubusercontent.com/16967174/561491644-ffb560fd-f7fa-4382-892c-e1b0a897bd24.png?jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NzMyMjMwNDYsIm5iZiI6MTc3MzIyMjc0NiwicGF0aCI6Ii8xNjk2NzE3NC81NjE0OTE2NDQtZmZiNTYwZmQtZjdmYS00MzgyLTg5MmMtZTFiMGE4OTdiZDI0LnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNjAzMTElMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjYwMzExVDA5NTIyNlomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWRjODdjYzQ3NDdhMjg3YmEyNzBiOWU1YzU2N2I1OGMzZjM0OWRkZTA5ZDhmOGIwNGE4NjgzNWZiODNlZTBlNjUmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.j2JWwnukrtmbMJgBWIuPszb0y9hDTVMHv4U2uOCy6Hc" width="300" alt="Law4Devs Logo">
  <br>
  <img src="https://private-user-images.githubusercontent.com/16967174/561491766-01227714-6612-4dcf-bfe2-59d244927e9c.svg?jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NzMyMjMwNDYsIm5iZiI6MTc3MzIyMjc0NiwicGF0aCI6Ii8xNjk2NzE3NC81NjE0OTE3NjYtMDEyMjc3MTQtNjYxMi00ZGNmLWJmZTItNTlkMjQ0OTI3ZTljLnN2Zz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNjAzMTElMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjYwMzExVDA5NTIyNlomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTczMDdjYWUzODAxMGMzZGM0M2M0YTcxMDRlYTgzZjZkOTkyNjlhNzhjNDAzZjE5MzI3NmExYTgxMmI4OGNlNzUmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.KBZLJ-ZBvqFQnkWlOLLPPvEw8VY1zkzRkkR3vRNMV7E" width="300" alt="Law4Devs">
  <br>
  <img src="https://private-user-images.githubusercontent.com/16967174/561491884-049dfdad-4f1e-4b37-81dc-f3281a543ec5.svg?jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NzMyMjMwNTQsIm5iZiI6MTc3MzIyMjc1NCwicGF0aCI6Ii8xNjk2NzE3NC81NjE0OTE4ODQtMDQ5ZGZkYWQtNGYxZS00YjM3LTgxZGMtZjMyODFhNTQzZWM1LnN2Zz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNjAzMTElMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjYwMzExVDA5NTIzNFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWIyODZiMGFjNDUxMDY5YTZiMTMzYzhkOWI2YmVkOWYzYmFiOGQ3OTk3ZGUyYWIwM2Q0NzRkYmQ0NGI0ZDViMzEmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.hqVkse7FTL6rwN_EvJ19Iz5rGAzSQ5sIVW1xS4CdkUQ" width="600" alt="Structured EU regulatory compliance data for developers">
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

All endpoints are under `/api/v1/`. Responses follow a consistent envelope:

```
GET  /api/v1/health
GET  /api/v1/frameworks
GET  /api/v1/frameworks/:slug
GET  /api/v1/frameworks/:slug/articles
GET  /api/v1/frameworks/:slug/articles/:article_number
GET  /api/v1/frameworks/:slug/articles/:article_number/related
GET  /api/v1/frameworks/:slug/recitals
GET  /api/v1/frameworks/:slug/recitals/:recital_number
GET  /api/v1/frameworks/:slug/requirements
GET  /api/v1/requirements
GET  /api/v1/frameworks/:slug/annexes
GET  /api/v1/frameworks/:slug/annexes/:annex_number
GET  /api/v1/frameworks/:slug/compliance/deadlines
GET  /api/v1/compliance/deadlines
GET  /api/v1/frameworks/:slug/stats
GET  /api/v1/stats
GET  /api/v1/search
GET  /api/v1/tags
GET  /api/v1/tags/:slug
GET  /api/v1/frameworks/:slug/changelog
GET  /api/v1/changelog
GET  /api/v1/compare
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
| Raw OpenAPI 3.0.3 spec (JSON) | `https://api.law4devs.eu/api/v1/openapi.json` |

---

*Law4Devs — making EU compliance programmable.*
