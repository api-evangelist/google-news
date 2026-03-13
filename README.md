# Google News RSS API

Google News provides RSS feeds that deliver news headlines organized by topic, location, and search query. The feeds expose structured XML data that can be consumed programmatically to retrieve top stories, topic-based headlines (World, Business, Technology, Sports, etc.), location-specific news, and keyword search results across multiple languages and regions.

## Artifacts

- **APIs.yml** - Machine-readable API metadata following the APIs.json specification.
- **OpenAPI** (`openapi/openapi.yml`) - OpenAPI 3.1.0 specification describing the Google News RSS feed endpoints and parameters.
- **JSON Schema** (`json-schema/google-news.json`) - JSON Schema (draft 2020-12) defining the structure of news feed items.
- **JSON-LD** (`json-ld/google-news.jsonld`) - JSON-LD context mapping news feed terms to schema.org vocabularies.

## Key Endpoints

| Method | Path | Description |
|--------|------|-------------|
| GET | `/rss` | Get top news headlines |
| GET | `/rss/headlines/section/topic/{topic}` | Get headlines by topic |
| GET | `/rss/headlines/section/geo/{location}` | Get headlines by location |
| GET | `/rss/search?q={query}` | Search news articles |

## Resources

- [Google News](https://news.google.com)
- [Google News Publisher Center](https://publishercenter.google.com)

## Maintainer

Kin Lane - kin@apievangelist.com
