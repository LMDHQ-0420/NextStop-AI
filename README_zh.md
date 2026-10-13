<p align="center">
  <img src="assets/logo-with-text.svg" alt="NextStop AI" width="720">
</p>

<p align="center">
  <strong>发现值得读的研究，讲清值得分享的贡献。</strong>
</p>

<p align="center">
  以证据为基础的 AI 论文检索与可视化 Skill。
</p>

<p align="center">
  <a href="README.md">English</a> · 简体中文
</p>

<p align="center">
  <a href="#skills">Skills</a> ·
  <a href="#快速开始">快速开始</a> ·
  <a href="#示例">示例</a> ·
  <a href="#参与贡献">参与贡献</a>
</p>

---

## 项目介绍

NextStop AI 将研究工作中的两个环节连接起来：找到具有实质贡献的大模型论文，再通过清晰、基于证据的视觉叙事讲明白这些贡献。

每个 Skill 都是一个独立的 `SKILL.md` 提示词，可以在兼容的编程 Agent 中加载，也可以直接作为 AI 助手的任务提示词使用。仓库不附带脚本或参考文件，具体任务所需的工具由运行环境提供。

## Skills

| Skill | 用途 | 产出 |
| --- | --- | --- |
| [论文检索](skills/paper-search/SKILL.md) | 检索过去 72 小时内的大语言模型与多模态研究，核实创新性、发布事件及独立关注信号。 | 最多 10 篇排序推荐，包含原始文献、关键证据、局限与优先阅读清单。 |
| [论文可视化](skills/paper-visualization/SKILL.md) | 阅读论文，提炼最重要的贡献，围绕原始图表与结果组织视觉叙事。 | 自包含 HTML 海报、高清 PNG、总览图、ZIP 包、可直接发布的宣传文案及策划证据文档。 |

### 核心原则

- **科学价值优先。** 声誉与热度辅助筛选，实质性创新是必要条件。
- **主张可核查。** 发布时间、比较对象、指标和外部关注都有对应依据。
- **呈现原始证据。** 保留论文图表及理解结果所必需的实验条件。
- **先叙事，后排版。** 由研究贡献决定故事线和页数。
- **交付完整成果。** 可视化包含可编辑 HTML、渲染图片和发布文案。

## 快速开始

### 1. 获取 Skill

```bash
git clone git@github.com:LMDHQ-0420/NextStop-AI.git
cd NextStop-AI
```

按照所用 Agent 的本地 Skill 目录约定，安装 `skills/` 中需要的文件夹；也可以将对应 `SKILL.md` 的内容直接作为 AI 助手的任务指令。两个 Skill 的提示词均使用中文。

### 2. 发起任务

**检索近期论文**

```text
使用 paper-search，筛选过去 72 小时内最值得关注的大语言模型
与多模态论文，使用 Asia/Shanghai 时区报告检索时间。
```

运行环境需要支持实时联网，以核实论文发布事件与外部关注。如果符合标准的论文不足 10 篇，按实际数量输出。

**制作论文海报**

```text
使用 paper-visualization，阅读我提供的论文和补充材料，
制作完整海报交付包及可直接发布的中文宣传文案。
```

提供论文全文或全文链接，以及可选的补充材料和视觉参考。运行环境需要支持论文读取、浏览器渲染和文件导出。PNG 从最终 HTML 直接渲染，分辨率至少为设计画布的 3 倍。

## 示例

以下 OVO-Bench 海报总览展示了论文可视化工作流的产出形式。八页内容从研究问题展开，通过原始证据呈现结果与局限；实际任务的页数由论文内容决定。

[![OVO-Bench：八页论文海报总览](assets/paper-visualization-ovo-bench.png)](assets/paper-visualization-ovo-bench.png)

<p align="center">
  <sub>点击图片查看完整分辨率的总览。</sub>
</p>

## 参与贡献

欢迎通过 Issue 或 Pull Request 提出改进，包括更清晰的指令、更充分的证据核查，以及帮助读者理解研究的示例。

每个 Skill 保持为独立的 `SKILL.md`，沿用统一结构：任务目标、输入与默认值、执行流程、质量要求、输出要求、交付前检查。提出修改时，请说明使用场景及其对产出的具体帮助。
