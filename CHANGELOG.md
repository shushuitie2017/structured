# Changelog

All notable changes to the Marble Skill Taxonomy dataset are documented here.
Dataset releases are versioned independently of the taxonomy `version` field
(the underlying taxonomy is `v1`).

## 交互式时间轴 demo + 中文内容层 · 2026-07-10

- **重做 `index.html` 交互 demo**：改为**年龄时间轴**布局（横轴 4–15 岁，每个年龄一个网格块，
  块高＝该年龄知识点数量），先修连线默认隐藏、点击/悬停节点才高亮其整条先修链与解锁项，
  彻底改掉此前 3D 力导向图的杂乱。搜索、学科筛选、重置视图、详情面板一应俱全。
- **新增中文内容层 `data/i18n/zh.json`**：把全部 1,590 个知识点的 name/description/evidence、
  以及 3,218 条唯一先修理由译成简体中文，供 demo 优先显示（回退英文原文）。
  原始 `data/*.json` **保持英文原文不变**（校验和不变）。
- **许可**：`zh.json` 是对 Marble 所撰文本（CC BY-SA 4.0）的翻译，属衍生内容，
  同样在 CC BY-SA 4.0 下发布并保留署名；第三方课标（`curriculum-standards.json`）未翻译、未改动。

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
