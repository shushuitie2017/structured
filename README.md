<div align="center">

# 🧭 结构化 · Structured

<img src="assets/demo-timeline.png" alt="儿童学习时间轴：1590 个知识点按 4–15 岁排成一排直方块，按学科着色" width="820" />

> *「每个孩子该学什么、先学什么、学完又能解锁什么 —— 摊开成一张看得见的图。」*

[![▶ 在线体验](https://img.shields.io/badge/▶_在线体验-Live-60a5fa?style=flat-square)](https://shushuitie2017.github.io/structured/)
![知识点](https://img.shields.io/badge/知识点-1,590-34d399?style=flat-square)
![先修关系](https://img.shields.io/badge/先修关系-3,221-f472b6?style=flat-square)
![学科](https://img.shields.io/badge/学科-8-a78bfa?style=flat-square)
![许可](https://img.shields.io/badge/许可-ODbL_1.0_·_CC_BY--SA_4.0-fbbf24?style=flat-square)
![语言](https://img.shields.io/badge/UI-简体中文-fb923c?style=flat-square)

**把 1,590 个小学知识点按 4–15 岁排成一条时间轴 —— 点任意一个，立刻看清它的整条先修链，和掌握后能解锁什么。全中文。**

<sub>一张连通的「学习之图」，不是又一份扁平的课标清单。</sub>

[▶ 在线体验](#-在线体验) · [看效果](#-看效果) · [它能做什么](#-它能做什么) · [类别对照](#-类别对照表) · [怎么用](#-怎么用数据) · [关于作者](#-关于作者)

简体中文 · [English](README.en.md)

</div>

---

## ▶ 在线体验

### 👉 **<https://shushuitie2017.github.io/structured/>**

打开即用，无需安装。拖拽平移、滚轮缩放、悬停高亮、点击追溯 —— 一个知识点从哪来、到哪去，一目了然。

---

## 🎬 看效果

**横轴就是年龄（4–15 岁）。** 每个年龄一个网格块，块越高＝那个年龄要学的知识点越多。7 岁、9 岁最密，向两端递减 —— 一眼看清小学阶段的「知识密度曲线」。

<div align="center">
<img src="assets/demo-timeline.png" alt="按年龄分布的知识点时间轴总览" width="780" />
</div>

**点任意一个知识点，追溯它的整条先修链。** 比如点「造句」，画面立刻高亮出它向后**解锁**的 15 个知识点 —— 从「词与词之间空格」到「扩展名词短语」「多步问题解决」，一条清晰的成长路径向右铺开，其余全部淡出。名称、描述、掌握证据、先修理由，全是中文。

<div align="center">
<img src="assets/demo-trace.png" alt="点击“造句”高亮它的先修链与解锁项，右侧中文详情面板" width="780" />
</div>

> **不是「有哪些知识点」，而是「它们怎么一环扣一环」。** 这正是一张 DAG（有向无环图）能给你、而清单给不了的东西。

---

## ✨ 它能做什么

| | 功能 | 说明 |
|---|---|---|
| 🗓️ | **年龄时间轴** | 1,590 个知识点按适龄（4–15 岁）排成直方块，分布密度一眼可见 |
| 🔗 | **先修链追溯** | 点击任一知识点，递归高亮它「学之前必须先掌握」的整条链路 |
| 🔓 | **解锁预览** | 反向看这个知识点掌握后能继续学什么 |
| 🎨 | **学科分色** | 8 大学科各一色，块内按学科归组 |
| 🔍 | **中文搜索** | 输入中文名回车即定位（如「分数」「造句」「力与运动」） |
| 🈶 | **全中文内容** | 名称 / 描述 / 掌握证据 / 先修理由 全部简体中文，附英文原名 |
| 📦 | **纯数据可复用** | UTF-8 JSON，无运行时无依赖，加载即用，带 JSON Schema 与校验器 |

---

## 📊 数据里有什么

| 学科 | 知识点 | 学科 | 知识点 |
|---|---:|---|---:|
| 🟢 科学 | 547 | 🟡 历史 | 90 |
| 🔵 数学 | 503 | 🟣 个人与社会性发展 | 88 |
| 🌸 英语 | 286 | 🟠 生活技能 | 37 |
| 🔷 计算 | 21 | 🔴 学会学习 | 18 |

- **1,590 个微主题** —— 每个是一个可教学的单一想法，带大白话描述、掌握证据、类型、学科+领域、适龄区间。
- **3,221 条先修依赖** —— 有向无环图，每条边标注 `hard`（强）/`soft`（弱）+ 一句理由。
- **对齐各国课标** —— 每个知识点链接到它提炼自的标准（NGSS / Common Core / 英国国家课程等）。

---

## 🈶 类别对照表

数据字段为英文；下表给中文对照（阅读辅助，数据本体不改动）。

**8 大学科**：科学 Science · 数学 Mathematics · 英语 English · 历史 History · 个人与社会性发展 Personal & Social Development · 生活技能 Life Skills · 计算 Computing · 学会学习 Learning to Learn

**5 种知识点类型**：概念性 CONCEPTUAL · 程序性 PROCEDURAL · 表征性 REPRESENTATIONAL · 语言性 LANGUAGE · 元认知 META
**先修强度**：强先修 hard（不先掌握几乎学不会）· 弱先修 soft（先掌握有帮助但非必需）

<details><summary>展开 ~55 个领域（domain）中英对照</summary>

| 学科 | 英文领域 | 中文 |
|---|---|---|
| English | Grammar & Punctuation | 语法与标点 |
| English | Phonics & Word Reading | 自然拼读与单词认读 |
| English | Reading Comprehension | 阅读理解 |
| English | Writing Composition | 写作 |
| Mathematics | Counting & Cardinality | 计数与基数 |
| Mathematics | Fractions | 分数 |
| Mathematics | Geometry | 几何 |
| Mathematics | Algebra | 代数 |
| Science | Scientific Inquiry | 科学探究 |
| Science | Forces & Motion | 力与运动 |
| Science | The Human Body | 人体 |
| Science | Space Exploration | 太空探索 |
| History | Ancient Egypt | 古埃及 |
| Personal & Social Development | Emotional Literacy | 情绪素养 |
| Life Skills | Money & Finance | 金钱与理财 |
| Computing | Artificial Intelligence | 人工智能 |

完整对照见 demo 内的学科图例与详情面板。

</details>

---

## 🛠 怎么用数据

纯数据，无运行时、无依赖 —— 加载 JSON 即可。

```js
import topics from './data/topics.json' with { type: 'json' };
import deps   from './data/dependencies.json' with { type: 'json' };
import zh     from './data/i18n/zh.json' with { type: 'json' };  // 中文内容层（可选）

const byId = new Map(topics.topics.map(t => [t.id, t]));
// 「造句」的所有先修知识点（中文名）
const prereqs = deps.dependencies
  .filter(d => d.topicId === 'mt_N8CpN1EJrP')
  .map(d => zh.topics[d.prerequisiteId]?.name ?? byId.get(d.prerequisiteId).name);
```

校验结构与引用完整性：`node scripts/validate.mjs`

| 文件 | 内容 |
|---|---|
| [`data/topics.json`](data/topics.json) | 微主题（图的节点，英文原文） |
| [`data/dependencies.json`](data/dependencies.json) | 先修边（`topicId` 依赖 `prerequisiteId`） |
| [`data/i18n/zh.json`](data/i18n/zh.json) | **中文内容层**：1,590 知识点 + 3,218 先修理由的简体中文 |
| [`data/clusters.json`](data/clusters.json) | 家长向领域摘要 |

---

## 💡 背后的故事

课程数据要么是一份读不动的扁平清单，要么锁在某个 App 里。可孩子的学习明明是**有先后、能连成网**的：会「造句」才谈得上「扩写句子」，懂「振动发声」才学得了「音量规律」。

于是有了这个 **Structured / 结构化** —— 把这些知识点摊平在一条 4–15 岁的时间轴上，再把「谁是谁的前提」一条条连起来，做成一张点开就能追溯的图，全中文。名字很直白：把散落的知识点，变得**结构化**。

---

## ⚖️ 诚实边界

- **适龄从 4 岁起**：底层数据里没有 4 岁以下的知识点，所以时间轴从 4 岁开始（不是 1 岁）。
- **课标原文是英文**：`curriculum-standards.json`（第三方官方标准）保持英文原样，未翻译（详见许可）。
- **中文是译文**：知识点内容由英文原始数据集翻译而来，力求自然，但个别专有表述可能与你熟悉的说法略有出入 —— 详情面板同时给出英文原名，便于核对。
- **它描述「典型顺序」，不是唯一真理**：先修关系是一种合理的教学次序参考，不代表每个孩子都必须严格照此。

---

## 👤 关于作者

**蓝猫 · BlueCat** —— AI-native builder，做 3D、教育与工具类产品，作品覆盖中 / 英 / 日。

<table>
<tr>
<td width="220" align="center">
<img src="assets/wechat-qr.jpg" width="200" alt="微信联系二维码" /><br/>
<sub>👆 微信 · 交流 / 合作</sub>
</td>
<td>

| | |
|---|---|
| 🐙 GitHub | **[@shushuitie2017](https://github.com/shushuitie2017)** |
| 🧭 本项目 | [结构化 · Structured](https://shushuitie2017.github.io/structured/) |
| 💬 微信 | 扫左侧二维码 |

想聊教育数据、3D 可视化、AI 产品，欢迎加微信。

</td>
</tr>
</table>

### 🌟 也在做

| 项目 | 一句话 | 在线 |
|---|---|---|
| 🧒 **蓝猫学 Claude** | 给孩子的 AI 互动小课本 | [learn.bluecatbot.com](https://learn.bluecatbot.com) |
| 🔧 **HardwareLab** | 3D 硬件拆解教学平台，60fps 程序化建模 | [hardware.bluecatbot.com](https://hardware.bluecatbot.com) |
| ⌨️ **MODKEYS** | 浏览器里的 3D 客制化键盘配置器 | [keyboard.bluecatbot.com](https://keyboard.bluecatbot.com) |
| 🎨 **矢安 SVGSafe** | 授权清晰的免费 SVG 图标 / 插画库 | [svg.bluecatbot.com](https://svg.bluecatbot.com) |
| 📝 **vlog 三语博客** | 每日热点 + 经典书方法论，中英日 | [vlog.bluecatbot.com](https://vlog.bluecatbot.com) |

---

## 📜 数据来源与许可

本项目是对一个**开放数据集**的中文版（文档汉化 + 全量中文内容层 + 交互式 demo）。底层数据集**采用多重许可**，使用或再分发前请阅读：

| 层 | 许可 |
|---|---|
| **数据库**（集合、结构、ID、主题↔主题 / 主题↔标准的关系） | [**ODbL 1.0**](LICENSE) —— 研究与商用皆可，**要求署名 + 相同方式共享** |
| **文本内容**（name / description / evidence / reason / summary，含其简体中文译文） | [**CC BY-SA 4.0**](LICENSE-CONTENT) —— 署名 + 相同方式共享 |
| **`curriculum-standards.json`**（第三方课标） | 各上游自有许可，见 [**PROVENANCE.md**](PROVENANCE.md)，未翻译、未改动 |

> **署名（ODbL / CC BY-SA 要求，必须保留）：**
> Marble Skill Taxonomy (v1) · © Generative Spark, Inc. (Marble) · <https://withmarble.com> · licensed under ODbL 1.0 (database) and CC BY-SA 4.0 (content).

简体中文译文（`data/i18n/zh.json`）为对上述 CC BY-SA 内容的翻译，同样在 CC BY-SA 4.0 下发布并保留署名。正式引用见 [CITATION.cff](CITATION.cff)，变更见 [CHANGELOG.md](CHANGELOG.md)。

---

<div align="center">

*「散落的知识点，连成一张看得见的图。」*

**[▶ 打开时间轴](https://shushuitie2017.github.io/structured/)**

</div>
