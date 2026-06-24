# Pi-Agent 上下文工程策略分析

[English](#english) | 中文

从 AI 产品经理视角，交互式拆解 [Pi-Agent](https://github.com/earendil-works/pi-mono) 的上下文工程策略——上下文如何构建、约束与稳定化。

**🔗 [在线查看分析页面](https://pi-context-engineering-analys1s.vercel.app)**

## 分析维度

| # | 模块 | 核心问题 |
|---|------|----------|
| 01 | 总览 | 上下文工程不是 prompt 拼接，三个基础矛盾是什么？ |
| 02 | 生命周期 | 一次任务中上下文如何流动？ |
| 03 | 启动 | 资源如何分层发现？信任边界在哪？ |
| 04 | 会话树 | 为什么上下文不是线性聊天记录？ |
| 05 | 系统提示词 | 最大的单次文本装配做了什么？ |
| 06 | Agent Loop | 每轮调用前的装配线如何工作？ |
| 07 | Compaction | 历史如何被压缩而不丢失可恢复性？ |
| 08 | 三维约束 | 防欠给、防错给、防过给如何同时成立？ |
| 09 | 来源稳定性 | 三层来源模型和稳定性矩阵是什么？ |
| 10 | 深度洞察 | 架构设计、韧性机制与默认值策略 |

## 项目结构

```
├── index.html              # 交互式分析页面
├── docs/                   # 原始分析文档
│   ├── 01-概述与架构总览.md
│   ├── 02-完整生命周期中的上下文构建.md
│   ├── 03-上下文工程约束机制.md
│   ├── 04-上下文来源分类与稳定性约束.md
│   └── 05-额外发现与深度洞察.md
└── README.md
```

## 技术栈

- 纯 HTML / CSS / JavaScript，零构建步骤
- [Mermaid.js](https://mermaid.js.org/) 渲染架构图
- CDN 加载，单文件部署

## 部署

托管于 [Vercel](https://vercel.com)，推送到 `main` 分支即自动部署。

---

<a id="english"></a>

# Pi-Agent Context Engineering Analysis

English | [中文](#pi-agent-上下文工程策略分析)

An interactive teardown of [Pi-Agent](https://github.com/earendil-works/pi-mono)'s context engineering — how context is built, constrained, and stabilized throughout an agent's lifecycle. Analyzed from an AI Product Manager's perspective.

**🔗 [View Live Analysis](https://pi-context-engineering-analys1s.vercel.app)**

## Analysis Dimensions

| # | Module | Core Question |
|---|--------|---------------|
| 01 | Overview | Context engineering ≠ prompt concatenation. What are the three fundamental tensions? |
| 02 | Lifecycle | How does context flow through a single task? |
| 03 | Startup | How are resources discovered in layers? Where are the trust boundaries? |
| 04 | Session Tree | Why isn't context a linear chat log? |
| 05 | System Prompt | What does the largest single-text assembly do? |
| 06 | Agent Loop | How does the per-turn assembly line work? |
| 07 | Compaction | How is history compressed without losing recoverability? |
| 08 | 3D Constraints | How do under-supply, wrong-supply, and over-supply prevention coexist? |
| 09 | Source Stability | What are the three-layer source model and stability matrix? |
| 10 | Deep Insights | Architecture, resilience mechanisms, and default value strategies |

## Project Structure

```
├── index.html              # Interactive analysis page
├── docs/                   # Source analysis documents (Chinese)
│   ├── 01-概述与架构总览.md
│   ├── 02-完整生命周期中的上下文构建.md
│   ├── 03-上下文工程约束机制.md
│   ├── 04-上下文来源分类与稳定性约束.md
│   └── 05-额外发现与深度洞察.md
└── README.md
```

## Tech Stack

- Pure HTML / CSS / JavaScript — zero build step
- [Mermaid.js](https://mermaid.js.org/) for architecture diagrams
- CDN-loaded, single-file deployment

## Deploy

Hosted on [Vercel](https://vercel.com). Push to `main` to deploy automatically.

## License

Analysis content © Cissie (Xu Yahang). Pi-Agent source code belongs to its respective owners.
