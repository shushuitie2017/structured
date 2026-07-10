**简体中文** | [English](README.en.md)

# Marble 技能分类体系（中文文档版）

一套开放、结构化的分类体系，刻画**孩子在小学阶段学些什么**——把知识拆解为细粒度的「微主题（micro-topic）」，串成一张先修关系图，并对齐各国课程标准。由 [Marble](https://withmarble.com) 制作。

> **版本：** `v1` · **主题数：** 1,590 · **先修关系边：** 3,221 · **学科：** 8

> **关于本仓库：** 这是 [os-taxonomy](https://github.com/withmarbleapp/os-taxonomy) 的**中文文档版**。`data/` 下的数据文件**保持英文原文不变**（结构、ID、校验和均与上游一致），仅将 README 文档与类别标签汉化，并附一份「类别对照表」帮助中文读者阅读英文数据。许可证与署名完全沿用上游（见下方 [许可证](#许可证)）。

## 先看效果

> 🌐 **在线交互 demo（全中文）：** **[shushuitie2017.github.io/structured](https://shushuitie2017.github.io/structured/)** —— **儿童学习时间轴**：横轴 4–15 岁，把 1,590 个知识点按适龄排布成一排"直方块"，点击任一知识点即可高亮它的整条先修链与后续解锁。知识点名称、描述、掌握证据、先修理由均已译成简体中文。

![该分类体系呈现为一张旋转的 3D 图：每个点是一个微主题，按学科着色，用先修关系相连](media/curriculum-viz.gif)

每个点是一个微主题，按学科着色；高度代表年龄；每条线是一条先修关系（[高清视频](media/curriculum-viz.mp4)）。也可在官方站点 [withmarble.com/curriculum](https://withmarble.com/curriculum) 交互式探索——点击任一概念，即可追溯学习者在掌握它之前必须先学会的一切。


## 这是什么

大多数课程数据要么是一份扁平的标准清单，要么被锁在某个产品内部。而这份数据集是一张**互相连通的学习之图**：

- **1,590 个微主题** —— 一个可教学的单一想法（例如 *「Building sentences（造句）」*、*「Apparent brightness of stars（恒星的视亮度）」*），每个都带有一段大白话描述、掌握程度的**证据（evidence）**判据、一个类型（概念性 / 程序性 / 表征性 / 语言性 / 元认知）、一个学科 + 领域（domain），以及一个大致的年龄区间。
- **3,221 条先修依赖** —— 一张有向无环图：*「主题 X 依赖先修 Y」*，每条边标注 `hard`（强）/`soft`（弱），并附一句**理由（reason）**。
- **课程对齐** —— 每个微主题都链接到它所提炼自的标准（NGSS、Common Core、英国国家课程等）。
- **领域聚类（domain clusters）** —— 183 段面向家长、每段一小节、按（学科、领域、年龄段）划分的摘要。

### 学科

| 学科 | 主题数 |
|---|---:|
| Science（科学） | 547 |
| Mathematics（数学） | 503 |
| English（英语） | 286 |
| History（历史） | 90 |
| Personal & Social Development（个人与社会性发展） | 88 |
| Life Skills（生活技能） | 37 |
| Computing（计算） | 21 |
| Learning to Learn（学会学习） | 18 |

## 类别对照表

数据文件中的类别标签均为英文；下表提供中文对照，仅供阅读参考（数据本体不改动）。

### 学科（subject）

| 英文 | 中文 |
|---|---|
| Science | 科学 |
| Mathematics | 数学 |
| English | 英语 |
| History | 历史 |
| Personal & Social Development | 个人与社会性发展 |
| Life Skills | 生活技能 |
| Computing | 计算 |
| Learning to Learn | 学会学习 |

### 领域（domain）

| 学科 | 英文领域 | 中文 |
|---|---|---|
| English | English Thinking | 英语思维 |
| English | Grammar & Punctuation | 语法与标点 |
| English | Handwriting & Transcription | 书写与誊抄 |
| English | Phonics & Word Reading | 自然拼读与单词认读 |
| English | Reading Comprehension | 阅读理解 |
| English | Speaking & Listening | 口语与听力 |
| English | Spelling & Word Study | 拼写与词汇研习 |
| English | Vocabulary | 词汇 |
| English | Writing Composition | 写作 |
| Mathematics | Counting & Cardinality | 计数与基数 |
| Mathematics | Number Representation & Place Value | 数的表示与位值 |
| Mathematics | Addition & Subtraction | 加法与减法 |
| Mathematics | Multiplication & Division | 乘法与除法 |
| Mathematics | Fractions | 分数 |
| Mathematics | Ratio & Proportion | 比与比例 |
| Mathematics | Algebra | 代数 |
| Mathematics | Geometry | 几何 |
| Mathematics | Measurement | 测量 |
| Mathematics | Data & Statistics | 数据与统计 |
| Mathematics | Probability | 概率 |
| Mathematics | Mathematical Thinking | 数学思维 |
| Science | Scientific Inquiry | 科学探究 |
| Science | Organisms & Life Processes | 生物体与生命过程 |
| Science | The Human Body | 人体 |
| Science | Animals of the World | 世界动物 |
| Science | Insects & Minibeasts | 昆虫与小生物 |
| Science | Ocean Life | 海洋生物 |
| Science | Ecosystems & Habitats | 生态系统与栖息地 |
| Science | Rainforests | 雨林 |
| Science | Polar Regions | 极地 |
| Science | Dinosaurs & Paleontology | 恐龙与古生物学 |
| Science | Matter & Materials | 物质与材料 |
| Science | Forces & Motion | 力与运动 |
| Science | Energy | 能量 |
| Science | Waves, Light & Sound | 波、光与声 |
| Science | Earth's Systems | 地球系统 |
| Science | Weather & Climate | 天气与气候 |
| Science | Volcanoes & Earthquakes | 火山与地震 |
| Science | Space Systems & Earth's History | 太空系统与地球历史 |
| Science | Space Exploration | 太空探索 |
| History | Historical Thinking | 历史思维 |
| History | Ancient Egypt | 古埃及 |
| History | Ancient Greece & Rome | 古希腊与古罗马 |
| History | Medieval Times | 中世纪 |
| Personal & Social Development | Self-Awareness | 自我觉察 |
| Personal & Social Development | Self-Regulation & Resilience | 自我调节与韧性 |
| Personal & Social Development | Emotional Literacy | 情绪素养 |
| Personal & Social Development | Empathy & Social Awareness | 共情与社会觉察 |
| Personal & Social Development | Friendship & Cooperation | 友谊与合作 |
| Personal & Social Development | Responsible Decision-Making | 负责任的决策 |
| Life Skills | Money & Finance | 金钱与理财 |
| Life Skills | Entrepreneurship | 创业 |
| Computing | Artificial Intelligence | 人工智能 |
| Learning to Learn | Learning to Learn | 学会学习 |

### 主题类型（type）

| 英文 | 中文 | 含义 |
|---|---|---|
| CONCEPTUAL | 概念性 | 理解一个概念、原理或关系 |
| PROCEDURAL | 程序性 | 会执行一套步骤或方法 |
| REPRESENTATIONAL | 表征性 | 会读写某种表示法（图、符号、记法等） |
| LANGUAGE | 语言性 | 掌握某个术语或表达方式 |
| META | 元认知 | 关于学习本身的策略与自我调控 |

### 先修强度（dependency strength）

| 英文 | 中文 | 含义 |
|---|---|---|
| hard | 强先修 | 不先掌握先修，几乎无法学会目标主题 |
| soft | 弱先修 | 先掌握先修有帮助，但非绝对必需 |

## 文件

所有数据都放在 [`data/`](data/) 下，为 UTF-8 编码的 JSON。JSON Schema 见 [`schema/`](schema/)；数量统计与 SHA-256 校验和见 [`manifest.json`](data/manifest.json)。

| 文件 | 内容 |
|---|---|
| [`data/topics.json`](data/topics.json) | 微主题（图的**节点**）。 |
| [`data/dependencies.json`](data/dependencies.json) | 先修**边**（`topicId` 依赖 `prerequisiteId`）。 |
| [`data/curriculum-standards.json`](data/curriculum-standards.json) | 来源课程标准，按课程分组。 |
| [`data/clusters.json`](data/clusters.json) | 面向家长的领域摘要。 |
| [`data/manifest.json`](data/manifest.json) | 数量统计、分学科明细、各文件校验和。 |

### 一个主题（topic）长这样

```json
{
  "id": "mt_N8CpN1EJrP",
  "type": "CONCEPTUAL",
  "subject": "English",
  "domain": "Grammar & Punctuation",
  "name": "Building sentences",
  "description": "Understand that words combine to make sentences — a sentence expresses a complete thought…",
  "ageRangeStart": 4,
  "ageRangeEnd": 6,
  "centrality": 0.257,
  "evidence": [
    "Distinguish between complete sentences and fragments",
    "Compose a complete sentence with a subject and verb"
  ],
  "assessmentPrompt": "If {{name}} says something like \"The dog\", can they tell you that's not a complete sentence…?",
  "standards": ["ccss-ela:L.K.1f", "uk-nc-2013:Eng.App2.Y1.Sent.1"]
}
```

- `id` —— 稳定标识符（`mt_…`），被依赖关系和相邻节点引用。
- `standards` —— `curriculum-standards.json` 中的键（`"<课程 slug>:<代码>"`）。
- `assessmentPrompt` —— 针对该想法的自然语言检验话术。含一个 `{{name}}` 占位符（孩子的名字）；显示前请替换或删除。

### 一条依赖（dependency）长这样

```json
{ "topicId": "mt__00ZSLnB7p", "prerequisiteId": "mt_VBl1T1sFCM", "strength": "hard",
  "reason": "Must understand vibrations make sound before finding volume patterns" }
```

`topicId` **依赖** `prerequisiteId`。把边反过来，就得到「解锁（unlocks）」关系。

## 怎么用

纯数据——没有运行时、没有依赖。加载 JSON 即可开用。

```js
import topics from './data/topics.json' with { type: 'json' };
import deps from './data/dependencies.json' with { type: 'json' };

const byId = new Map(topics.topics.map(t => [t.id, t]));
const prereqs = deps.dependencies
  .filter(d => d.topicId === 'mt_N8CpN1EJrP')
  .map(d => byId.get(d.prerequisiteId).name);
```

校验结构与引用完整性：

```bash
node scripts/validate.mjs
```

## 许可证

本数据集**采用多重许可**——使用或再分发前请务必先阅读本节。

| 层 | 许可证 |
|---|---|
| **数据库本身** —— 集合、结构、ID、主题↔主题与主题↔标准之间的关系 | [**ODbL 1.0**](LICENSE) —— 可免费用于研究**及**商业用途，**要求署名**，**相同方式共享**（衍生*数据库*必须在 ODbL 下保持开放）。 |
| **Marble 撰写的文本内容** —— 主题的 `description`/`name`/`evidence`/`assessmentPrompt`、依赖的 `reason`、聚类的 `summary` | [**CC BY-SA 4.0**](LICENSE-CONTENT) —— 精神一致：署名 + 相同方式共享。 |
| **`curriculum-standards.json`** —— 提取自第三方框架 | **并非** Marble 有权重新授权的内容。每个来源都受**其自身的上游许可**约束——见 [**PROVENANCE.md**](PROVENANCE.md)。 |

**为什么既是相同方式共享、又对商用友好：** ODbL 区分*衍生数据库*（扩展/修改本分类体系 → 必须保持开放）与*产出作品*（把它用在某个产品、模型或应用里 → 仍归你所有）。因此你可以基于它构建商业产品而无需开源你的产品；你只需把对*分类体系本身*的改进回馈出来。

### 署名

任何使用都必须注明：

> Marble Skill Taxonomy (v1) · © Generative Spark, Inc. (Marble) · https://withmarble.com · licensed under ODbL 1.0 (database) and CC BY-SA 4.0 (content).

以及你所使用的任何课程标准在 [PROVENANCE.md](PROVENANCE.md) 中对应的上游声明。正式引用格式见 [CITATION.cff](CITATION.cff)。

## 本次*未*包含的内容

本次发布刻意排除：语义嵌入（embeddings，属派生数据、可重新计算）与任何按孩子/按用户的数据（从不公开）。详见 [CHANGELOG.md](CHANGELOG.md)。
