# Breaking Bad (breaking-bad)

Community-built REST API exposing characters, quotes, episodes, and on-screen deaths from the Breaking Bad and Better Call Saul television universe. The original hosted service at breakingbadapi.com is no longer reachable as of 2026-05-29 (DNS does not resolve). The canonical source code remains at github.com/timbiles/Breaking-Bad--API under BSD-3-Clause and is the basis for the historical OpenAPI and capability artifacts in this repo.

**URL:** [Visit APIs.json URL](https://github.com/timbiles/Breaking-Bad--API)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=opensource-api-evangelist&utm_content=repo)

## Status

- **x-type:** opensource
- **x-status:** deprecated
- **Deprecation:** Hosted service `breakingbadapi.com` is unreachable as of 2026-05-29 (DNS does not resolve). The source code repo at [timbiles/Breaking-Bad--API](https://github.com/timbiles/Breaking-Bad--API) (BSD-3-Clause, last commit 2022-12-10) remains available. Artifacts here preserve the historical contract.

## Tags:

 - Video, Television, Public APIs, Open Source, Breaking Bad, Better Call Saul, Pop Culture, Deprecated

## Timestamps

- **Created:** 2026-05-28
- **Modified:** 2026-05-29

## APIs

### Breaking Bad API

REST API for Breaking Bad and Better Call Saul data — characters, quotes, episodes, and deaths. Anonymous access (no API key). The original hosted service enforced 10,000 requests per IP per day and is now unreachable.

**Human URL:** [https://github.com/timbiles/Breaking-Bad--API](https://github.com/timbiles/Breaking-Bad--API)

**Base URL:** `https://www.breakingbadapi.com/api` (unreachable)

#### Tags:

 - Video, Television, Characters, Quotes, Episodes, Deaths

#### Properties

- [Documentation](https://github.com/timbiles/Breaking-Bad--API#readme)
- [SourceCode](https://github.com/timbiles/Breaking-Bad--API)
- [OpenAPI](openapi/breaking-bad-openapi.yml)
- [JSONSchema — Character Schema](json-schema/breaking-bad-character-schema.json)
- [JSONSchema — Quote Schema](json-schema/breaking-bad-quote-schema.json)
- [JSONSchema — Episode Schema](json-schema/breaking-bad-episode-schema.json)
- [JSONSchema — Death Schema](json-schema/breaking-bad-death-schema.json)
- [JSONStructure — Character Structure](json-structure/breaking-bad-character-structure.json)
- [JSONStructure — Quote Structure](json-structure/breaking-bad-quote-structure.json)
- [JSONStructure — Episode Structure](json-structure/breaking-bad-episode-structure.json)
- [JSONStructure — Death Structure](json-structure/breaking-bad-death-structure.json)
- [Examples — List Characters](examples/breaking-bad-listcharacters-example.json)
- [Examples — Random Quote](examples/breaking-bad-getrandomquote-example.json)
- [Examples — List Episodes](examples/breaking-bad-listepisodes-example.json)
- [Examples — Random Death](examples/breaking-bad-getrandomdeath-example.json)
- [NaftikoCapability — Characters](capabilities/breaking-bad-characters.yaml)
- [NaftikoCapability — Quotes](capabilities/breaking-bad-quotes.yaml)
- [NaftikoCapability — Episodes](capabilities/breaking-bad-episodes.yaml)
- [NaftikoCapability — Deaths](capabilities/breaking-bad-deaths.yaml)

## Common Properties

- [Website](https://github.com/timbiles/Breaking-Bad--API)
- [SourceCode](https://github.com/timbiles/Breaking-Bad--API)
- [License (BSD-3-Clause)](https://github.com/timbiles/Breaking-Bad--API/blob/master/LICENSE.rst)
- [PublicAPIsListing](https://github.com/public-apis/public-apis)
- [Plans — Free / Anonymous](https://github.com/timbiles/Breaking-Bad--API#readme)
- [RateLimits — 10,000 Requests Per Day](https://github.com/timbiles/Breaking-Bad--API#readme)
- [JSONLD](json-ld/breaking-bad-context.jsonld)
- [Vocabulary](vocabulary/breaking-bad-vocabulary.yml)
- [SpectralRules](rules/breaking-bad-rules.yml)

## Features

| Name | Description |
|------|-------------|
| Anonymous Access | No API key, no authentication, no signup. Hit the endpoints directly. |
| Random Sampling | Dedicated /random endpoints for characters, quotes, and deaths. |
| Series Filtering | Episodes and characters can be filtered by Breaking Bad vs Better Call Saul via the series/category query parameter. |
| On-Screen Death Catalog | Unusual for a TV-show API — every on-screen death is catalogued with cause, responsible character, and last words. |

## Use Cases

| Name | Description |
|------|-------------|
| Trivia and Quiz Apps | Power Breaking Bad trivia games and quote-attribution quizzes. |
| Front-End Tutorials | Widely used as a tutorial dataset for React, Vue, Angular, and Flutter API consumption courses. |
| ChatBot Personality Layer | Inject random Breaking Bad quotes into chatbots and Discord/Slack bots for flavor. |
| Sandbox for API Tooling | Small enough to use as a fixture for testing OpenAPI tooling, mock servers, and code generators. |

## Artifacts

Machine-readable API specifications organized by format.

### OpenAPI

- [Breaking Bad OpenAPI](openapi/breaking-bad-openapi.yml) — 11 operations across Characters, Quotes, Episodes, Deaths

### JSON Schema

- [Character Schema](json-schema/breaking-bad-character-schema.json)
- [Quote Schema](json-schema/breaking-bad-quote-schema.json)
- [Episode Schema](json-schema/breaking-bad-episode-schema.json)
- [Death Schema](json-schema/breaking-bad-death-schema.json)

### JSON Structure

- [Character Structure](json-structure/breaking-bad-character-structure.json)
- [Quote Structure](json-structure/breaking-bad-quote-structure.json)
- [Episode Structure](json-structure/breaking-bad-episode-structure.json)
- [Death Structure](json-structure/breaking-bad-death-structure.json)

### JSON-LD

- [Breaking Bad JSON-LD Context](json-ld/breaking-bad-context.jsonld)

### Examples

- [List Characters](examples/breaking-bad-listcharacters-example.json)
- [Random Quote](examples/breaking-bad-getrandomquote-example.json)
- [List Episodes](examples/breaking-bad-listepisodes-example.json)
- [Random Death](examples/breaking-bad-getrandomdeath-example.json)

## Capabilities

Naftiko capabilities, one self-contained file per business surface (OpenAPI tag). Each file inlines its own `consumes` block plus both REST and MCP exposers.

| Capability | File | Operations |
|------------|------|------------|
| Characters | [breaking-bad-characters.yaml](capabilities/breaking-bad-characters.yaml) | 3 (list, get-by-id, random) |
| Quotes | [breaking-bad-quotes.yaml](capabilities/breaking-bad-quotes.yaml) | 3 (list, get-by-id, random) |
| Episodes | [breaking-bad-episodes.yaml](capabilities/breaking-bad-episodes.yaml) | 2 (list, get-by-id) |
| Deaths | [breaking-bad-deaths.yaml](capabilities/breaking-bad-deaths.yaml) | 3 (list, count, random) |

## Vocabulary

- [Breaking Bad Vocabulary](vocabulary/breaking-bad-vocabulary.yml) — 4 capabilities, 4 content entities, 4 operational dimensions (Lookup, List, Random, Count) across Characters, Quotes, Episodes, and Deaths

## Rules

- [Breaking Bad Spectral Ruleset](rules/breaking-bad-rules.yml) — 30+ rules across info/metadata, paths, operations, tags, parameters, responses, schemas, security, HTTP-method conventions, and deprecation enforcement

## Source Repository

- **Repo:** [timbiles/Breaking-Bad--API](https://github.com/timbiles/Breaking-Bad--API)
- **Language:** JavaScript (Node.js)
- **License:** BSD-3-Clause
- **Last commit:** 2022-12-10
- **Status:** Source available; hosted endpoint deprecated

## Notes

This entry was bulk-registered as part of a public-apis catalog sweep on 2026-05-28 and fully enriched on 2026-05-29. Because the hosted API at `breakingbadapi.com` is unreachable, the OpenAPI spec, JSON Schemas, capabilities, and Spectral rules are preserved as a historical record of the API contract — useful as a teaching fixture, an OpenAPI tooling sandbox, or the basis for a local re-implementation seeded from the canonical source repo.

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
