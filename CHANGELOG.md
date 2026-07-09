# Changelog

All notable changes to the Marble Skill Taxonomy dataset are documented here.
Dataset releases are versioned independently of the taxonomy `version` field
(the underlying taxonomy is `v1`).

## 中文文档版 · Chinese documentation edition — 2026-07-10

A Chinese-language documentation edition of the dataset. **No data was changed.**

- Added a fully translated Simplified-Chinese `README.md`, with a category glossary
  (subjects / domains / topic types / dependency strengths) to help Chinese readers
  navigate the English data.
- Kept the original English README as `README.en.md`.
- **All `data/*.json` files, `schema/`, `scripts/`, IDs and SHA-256 checksums are
  unchanged** — `curriculum-standards.json` (third-party) is left verbatim.
- Licensing and attribution are inherited unchanged from upstream: `LICENSE` (ODbL 1.0),
  `LICENSE-CONTENT` (CC BY-SA 4.0), `PROVENANCE.md`, and `CITATION.cff` are byte-for-byte
  identical to the original. Full credit remains with Marble / Generative Spark, Inc.

## [1.0.0] — 2026-07-08

Initial public release.

### Included
- **1,590 micro-topics** across 8 subjects (`data/topics.json`).
- **3,221 prerequisite dependencies** with `hard`/`soft` strength + reasons (`data/dependencies.json`).
- **7 curricula / 3,261 standards** with 1,859 topic↔standard links (`data/curriculum-standards.json`).
- **183 domain clusters** (`data/clusters.json`).
- JSON Schemas + a dependency-free validator.

### Curriculum text shipped
- **Full text:** UK National Curriculum (OGL v3.0), Common Core ELA + Math (CCSS Public License).
- **Codes only** (verbatim text omitted pending rights clearance): NGSS K-5 + Middle School, C3 Framework, IB PYP PSPE. See [PROVENANCE.md](PROVENANCE.md).

### Excluded
- Semantic embeddings (derived / recomputable).
- All per-child and user data (never published).
