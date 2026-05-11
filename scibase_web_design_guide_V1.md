# SciBase 官网设计指南 V1

版本：V1  
对应原型：[scibase_web_prototype.html](/Users/shangfukai/Dev/Scibase/LandingPage/scibase_web_prototype.html)  
更新时间：2026-05-11  
视觉方向：黑 / 白 / 红，简约、克制、学术手绘感

---

## 1. 项目定位

**SciBase** 是面向大模型时代的 AI-Ready 学术知识基础设施。它不是传统文献检索系统，而是一个可计算、可理解、可追溯、可被 AI Agent 直接调用的知识基座，覆盖公开学术文献、图书、专利等多类型知识资产。

核心定位：

> 从“文献检索”升级为“知识基座”：不仅让人类检索，更让 Research Agent、Prior-Art Agent、Technical Intelligence Agent 获得可信、可追溯、可计算的证据层。

核心特征：

- **全面性**：跨学科、多类型、多来源、多语种。
- **实时性**：持续增量采集、加工和更新。
- **AI-Ready**：面向模型训练、RAG 推理、Agent 知识调用设计。
- **可追溯**：保留来源、原始响应、解析版本、证据片段和治理信号。

---

## 2. 页面目标

该页面是 SciBase 的产品介绍首页，用于向外部用户解释：

1. SciBase 是什么。
2. SciBase 的数据规模和覆盖能力。
3. SciBase 如何服务人类用户、Agent 与企业系统。
4. SciBase 的五层数据基座如何支撑可追溯知识对象。
5. 用户如何开始使用：API、在线体验、联系我们。

页面不设计成传统数据库门户，也不采用夸张科技感，而是呈现为一个**学术感、基础设施感、数据可信感**兼具的产品介绍页。

---

## 3. 目标用户

### 3.1 2B 用户，主要目标

包括：

- Auto-Research / Deep Research 产品团队。
- 企业数据挖掘服务团队。
- 投研、咨询、药研、知识产权、技术情报团队。
- 大模型公司、RAG 平台、企业知识库厂商。

他们关注：

- 数据规模和覆盖类型。
- 数据来源可信度。
- 是否有全文、证据片段和引用上下文。
- 是否适合 Agent 调用。
- 是否可通过 API 集成。
- 是否有数据治理、版权、质量和追溯能力。

### 3.2 2C 用户，次要目标

包括科研人员、学生、技术研究者、普通检索用户。

他们关注：

- 是否可以检索论文、专利、图书。
- 是否有轻量在线体验。
- 是否能快速看到权威结果。
- 是否能追溯结果来源与证据。

---

## 4. 页面信息架构

当前 V1 页面按照 5 个主模块组织：

```text
顶部导航
→ Hero / 概览
→ Overview 数据规模
→ Scenarios 核心场景
→ Data Foundation Layers 数据基座五层架构
→ Task Examples 任务样例
→ Entry 使用入口
```

导航锚点：

```text
概览 / 场景 / 技术架构 / 任务样例 / 使用入口
```

其中，“任务样例”不是独立行业案例，而是对核心场景的进一步拆分，展示可以直接调用、交付和评估的具体任务。

---

## 5. 视觉系统

### 5.1 总体风格

采用**黑 / 白 / 红的极简学术风**：

- 白色与近白背景。
- 黑色 / 炭黑正文。
- 克制 SciBase 红作为唯一强调色。
- 细线边框、网格底纹、低对比阴影。
- 大字号衬线标题，正文使用现代无衬线。
- 插图采用黑色墨线、少量红色标注、学术笔记与档案图解气质。

避免：

- 米白 / 棕色旧方案。
- 高饱和蓝紫科技渐变。
- 玻璃拟态、发光、赛博风。
- 复杂 3D、装饰性光斑或过度动效。

关键词：

```text
Minimal / Academic / Infrastructure / Trustworthy / Archival / Agent-ready
```

### 5.2 当前色彩

| 用途 | 当前值 | 说明 |
|---|---:|---|
| 页面背景 | `#fbfbfa` | 近白底色，叠加极浅网格 |
| 卡片 / 纸面 | `#ffffff` | 主要内容容器 |
| 主文字 | `#101010` | 标题与重点信息 |
| 次级文字 | `#686868` | 说明文字 |
| 强边框 | `rgba(16, 16, 16, 0.32)` | hover / 架构强调 |
| 弱边框 | `rgba(16, 16, 16, 0.14)` | 常规分割 |
| 浅灰块 | `#f1f1ef` / `#e8e8e4` | 图表、端点、插图底 |
| 强调红 | `#a61826` | CTA、标签、动效、插图红线 |
| 红色底 | `rgba(166, 24, 38, 0.09)` | 弱强调背景 |

### 5.3 字体

- 英文与大标题：`Georgia`, `Times New Roman`, `Songti SC`, `SimSun`, serif。
- 中文正文：`Inter`, `Noto Sans SC`, `PingFang SC`, `Microsoft YaHei`, Arial, sans-serif。
- API / 代码：`SFMono-Regular`, Consolas, Menlo, monospace。

字体原则：

- 标题使用衬线，建立学术与档案感。
- 正文使用无衬线，保证中文长段落可读性。
- 不使用负字距。
- 不用随 viewport 线性缩放的小文本，移动端通过断行和布局重排处理。

---

## 6. 插图系统

V1 使用 8 张生成式 PNG 插图，均为无文字图片，不含 logo、水印或界面文案。

统一风格：

```text
black ink linework, sparse red accents, white paper background,
academic notebook / archival diagram feel, hand-drawn but polished,
minimal composition, no text, no logo, no watermark
```

当前资产：

| 使用位置 | 文件 |
|---|---|
| Hero 主视觉 | `assets/images/scibase-hero.png` |
| Overview 描述图 | `assets/images/scibase-overview.png` |
| Research Agent 场景 | `assets/images/scenario-research-agent.png` |
| Prior-Art 场景 | `assets/images/scenario-prior-art.png` |
| Enterprise Mining 场景 | `assets/images/scenario-enterprise-mining.png` |
| 自动综述任务样例 | `assets/images/case-ai-research.png` |
| 查新任务样例 | `assets/images/case-top-journals.png` |
| 企业情报任务样例 | `assets/images/case-paper-patent.png` |

插图约束：

- 图片中不放文字，避免生成模型产生伪字。
- 不使用 SVG 作为场景插图。
- 保持白底、黑线、红色少量强调。
- 场景图与任务样例图需要能在 3 列卡片中清晰阅读。
- 技术架构不使用生成图，改由 HTML / CSS / inline SVG 组件构成。

---

## 7. 模块设计说明

## 7.1 顶部导航

### 目的

提供页面主模块跳转，同时强化 SciBase 品牌。

### 当前内容

左侧：

```text
SciBase
AI-Ready Knowledge Base
```

右侧锚点：

```text
概览 / 场景 / 技术架构 / 任务样例 / 使用入口
```

### 交互

- Sticky 顶部导航。
- 背景为近白半透明 + blur。
- hover 时出现红色细线。
- 移动端隐藏右侧导航，只保留品牌。

---

## 7.2 Hero

### 目的

第一屏解释 SciBase 的核心定位，并给出进入架构和使用入口的主路径。

### 当前内容

Eyebrow：

```text
For Human Search · For Agent Calls
```

标题：

```text
面向人类与 AI 的新一代知识基础设施
```

说明：

```text
SciBase 覆盖公开学术文献、图书、专利等多类型知识资产，将跨源数据持续加工为可计算、可理解、可追溯、可被 Agent 直接调用的 AI-Ready Knowledge Objects。
```

按钮：

```text
查看数据架构
了解使用入口
```

右侧视觉：

```text
assets/images/scibase-hero.png
```

设计要点：

- 桌面端保持左右双栏。
- 标题是页面最大视觉元素。
- Hero 图片作为右侧主视觉，使用薄边框和轻阴影，不加厚重卡片感。
- 首屏底部保留后续内容线索。

---

## 7.3 Overview 数据规模

### 目的

用规模指标和基础图表建立“知识基座”的覆盖能力和可信感。

### 当前标题

```text
覆盖论文、图书、专利的知识总览
```

### 当前说明

```text
SciBase 不是传统文献检索系统，而是面向大模型时代的 AI-Ready 学术知识基础设施，强调全面性、实时性与 Agent 可用性。
```

### Overview 插图

```text
assets/images/scibase-overview.png
```

表达方向：

- 多源知识资产汇聚。
- 形成可计算、可追溯的 knowledge objects。
- 适合放在指标区左侧或上方。

### 指标卡片

| 指标 | 当前展示 |
|---|---:|
| 知识记录总量 | 5.16 亿 |
| 学术文献总量 | 3.41 亿 |
| 图书总量 | 1.05 亿 |
| 专利规模 | 7000 万 |
| AI-Ready 含全文记录 | 1.02 亿 |
| 语言覆盖 | 814 |
| Venue 覆盖 | 132.99 万 |
| OA 开放获取文献 | 125M，约占 28.12% |

### CSS 图表

保留两个小图：

1. 语言分布 Top 5。
2. 四大学科域。

语言分布：

| 语言 | 数量 |
|---|---:|
| 英文 en | 2.89 亿 |
| 中文 zh | 5013 万 |
| 德语 de | 2145 万 |
| 法语 fr | 1262 万 |
| 西语 es | 885 万 |

四大学科域：

| 学科域 | 文献量 |
|---|---:|
| 物理科学 | 7487 万 |
| 社会科学 | 5044 万 |
| 健康科学 | 3894 万 |
| 生命科学 | 3190 万 |

---

## 7.4 Scenarios 核心场景

### 目的

解释 SciBase 不只是检索系统，而是可被 Agent 和企业系统调用的数据基础设施。

### 当前标题

```text
面向人类与 Agent 的核心使用场景
```

### 场景卡片

#### Scenario 01：Research Agent 数据源供给

插图：

```text
assets/images/scenario-research-agent.png
```

说明：

```text
为 Auto-Research、Deep Research、技术调研 Agent 提供论文、专利、图书、证据片段和引用上下文，支持自动综述和报告生成。
```

标签：

```text
自动文献综述 / 技术路线调研 / 证据包生成
```

#### Scenario 02：Prior-Art 与技术查新

插图：

```text
assets/images/scenario-prior-art.png
```

说明：

```text
围绕一个技术 idea，跨论文、专利、图书和产品资料进行相似技术发现、claim 对比、novelty 风险判断与白区机会分析。
```

标签：

```text
专利查新 / Novelty 分析 / 论文-专利关联
```

#### Scenario 03：企业数据挖掘服务

插图：

```text
assets/images/scenario-enterprise-mining.png
```

说明：

```text
面向 2B 客户提供外部知识 enrichment：将企业项目、研发方向、客户需求与全球论文、专利、作者、机构、公司进行链接。
```

标签：

```text
知识图谱补全 / 技术情报监控 / 机构画像
```

---

## 7.5 Data Foundation Layers 数据基座五层架构

### 目的

展示 SciBase 的底层数据接入、留存、解析、对象化和治理能力。V1 已从早期 Harvest 五段流水线改为更贴近实际的 **SciBase 数据基座五层架构**。

### 当前标题

```text
SciBase 数据基座五层架构
```

### 当前说明

```text
从多源接入、原始留存、标准化解析，到知识对象、证据层与索引治理，形成可追溯、可计算、可被 Agent 调用的数据基座。
```

### 五层结构

| 层级 | 名称 | 作用 |
|---:|---|---|
| 1 | 多源接入层 | 接入论文、专利、图书、标准、数据集、代码等多类型来源 |
| 2 | 原始数据层 | 保存原始响应、全文、文件和采集上下文，保证可追溯 |
| 3 | 标准化与解析层 | 统一 schema，解析全文结构，抽取章节、图表、引用和 claims |
| 4 | 知识对象与证据层 | 生成 Paper、Patent、Book 等 canonical objects 和 evidence spans |
| 5 | 索引治理层 | 构建全文、向量、图谱、质量、版权和版本索引 |

### 表现方式

- 使用 HTML / CSS 构建分层表格式结构。
- 每层配一个与实际含义匹配的 inline SVG 小图。
- 不再使用每层重复的节点网络图。
- 白底、黑线、红色节点，保持与全站插图系统一致。
- 通过 `.layer-pulse`、hover 边框、红色图形节点形成克制动态效果。

### 每层图形语义

| 层级 | 图形方向 |
|---:|---|
| 1 | 多种来源汇入中心，表达论文、专利、图书、标准、数据集、代码接入 |
| 2 | 原始湖仓、文件、全文、响应包与采集上下文 |
| 3 | 文档解析为 schema blocks、章节、图表、引用、claims |
| 4 | canonical object、证据片段、对象关系与来源证据 |
| 5 | 全文索引、向量索引、图谱、质量、版权、版本治理 |

### 动效原则

- 动效低频、克制，服务于“数据流动与治理”表达。
- 支持 `prefers-reduced-motion`，关闭非必要动画。
- 不做强闪烁、不做炫光、不做复杂粒子背景。

---

## 7.6 Task Examples 任务样例

### 目的

本区不是“典型案例”或行业案例，而是对核心场景的进一步细化，展示 SciBase 可以支持的具体任务单元。

### 当前标题

```text
从核心场景拆出的具体任务样例
```

### 当前说明

```text
这里不是另起一组行业案例，而是把上面的三类核心场景进一步拆成可直接调用、交付和评估的任务单元。
```

### 任务卡片

#### Example 01 · Research Agent：自动综述与证据包生成

插图：

```text
assets/images/case-ai-research.png
```

说明：

```text
给定一个研究问题，Agent 调用 SciBase 检索论文、图书与专利上下文，抽取关键证据片段、引用链路和方法差异，生成可追溯的综述草稿。
```

标签：

```text
Query 扩展 / Evidence Pack / 引用上下文
```

#### Example 02 · Prior-Art：技术 idea 查新与相似证据定位

插图：

```text
assets/images/case-top-journals.png
```

说明：

```text
输入一段技术 idea 或 claim 草稿，系统跨论文、专利、图书和标准发现相似表述，返回 novelty 风险点、相似证据和可继续追问的白区方向。
```

标签：

```text
相似技术发现 / Claim 对比 / 白区机会
```

#### Example 03 · Enterprise Mining：企业研发方向与外部知识链接

插图：

```text
assets/images/case-paper-patent.png
```

说明：

```text
围绕企业项目、产品路线或客户需求，持续链接全球论文、专利、作者、机构和公司，形成技术画像、竞品监控和主题变化提醒。
```

标签：

```text
项目 enrichment / 竞品监控 / 主题 Watch
```

---

## 7.7 Entry 使用入口

### 目的

把页面从产品展示转向转化，说明用户如何开始使用 SciBase。

### 当前标题

```text
使用入口：API、在线体验与联系我们
```

### 当前结构

V1 使用三张并列卡片：

```text
API / Online Experience / Contact
```

#### API

说明：

```text
SciBase 以 API 作为主要集成方式：基础 API 面向检索、元数据、全文与证据获取，Agent-native API 面向可追溯任务调用和自动化研究工作流。
```

Basic API：

```text
GET /metadata/search
GET /content/fetch
POST /evidence/query
```

Agent-native API：

```text
POST /agent/search
POST /agent/evidence-pack
POST /agent/prior-art
```

#### Online Experience

说明：

```text
在线体验聚焦 Agent Search：用户以自然语言提出研究问题，系统返回论文、专利、图书和证据片段，并展示来源、质量信号与可追溯链路。
```

Agent Search：

```text
Ask research questions
Inspect evidence spans
Trace source provenance
```

按钮：

```text
进入在线体验
```

#### Contact

说明：

```text
面向 API 试用、数据合作、Agent 场景共建和企业知识基础设施集成需求，可以通过邮箱联系 SciBase 团队，二维码位置预留给后续商务或产品入口。
```

当前预留：

```text
contact@scibase.ai
QR placeholder
联系我们
```

---

## 8. 响应式规则

### 桌面端

- 页面最大宽度约 1240px。
- Hero 保持左右双栏。
- Overview 使用插图 + 4 列指标网格。
- 场景卡片为 3 列。
- 任务样例卡片为 3 列。
- 数据架构五层横向表格式堆叠，保持每层图形可读。
- 使用入口为 3 张并列卡片。

### 平板与移动端

- 多列内容降为单列。
- 顶部导航仅保留品牌。
- Hero 图片与正文上下堆叠。
- 指标卡片、场景卡片、任务样例卡片单列堆叠。
- 数据架构每层信息纵向排列，SVG 插图保持在内容流内，不与文字重叠。
- 使用入口三张卡片纵向排列。

---

## 9. 交互与动效

V1 动效只做低频反馈，不做强表现型动画：

- 导航 hover 红线。
- 按钮 hover 轻微反转或边框强调。
- 场景 / 任务卡片 hover 轻微上浮。
- 架构层 hover 边框强调。
- 架构区域保留克制脉冲，表达数据流与治理。
- `prefers-reduced-motion` 下禁用非必要 animation 与 transition。

---

## 10. 开发注意事项

1. 当前原型是单文件静态 HTML，目标文件为 `scibase_web_prototype.html`。
2. 当前资源目录为 `assets/images/`，包含 8 张生成式 PNG 插图。
3. 插图应继续保持无文字、无 logo、无水印。
4. 技术架构区使用 HTML / CSS / inline SVG 组件，不使用生成图片。
5. 指标图表当前为 CSS 条形图，后续可接入 ECharts / Recharts，但 V1 不引入额外库。
6. 页面需要保留 anchor id，方便导航跳转。
7. 首页不建议加入复杂检索框，当前重点是解释定位、能力和入口。
8. 后续如果迁移到 React / Next.js，应优先保留当前信息架构、视觉系统和插图资产命名。

---

## 11. V1 验收清单

- 页面主色为黑 / 白 / 红，没有回退到米白 / 棕色旧方案。
- Hero 右侧图片清晰，且不含文字、水印或伪字符。
- Overview 指标与两个 CSS 图表正常展示。
- 三个核心场景均有对应插图、标题、说明和标签。
- 数据架构为五层结构，且每层 SVG 与语义匹配，不重复套用同一图形。
- “任务样例”不再写成“典型案例”，内容是核心场景的进一步拆分。
- Entry 为 API、Online Experience、Contact 三张卡片。
- 桌面端无内容重叠，移动端单列堆叠正常。
- 架构动效低频、克制，并尊重 `prefers-reduced-motion`。

