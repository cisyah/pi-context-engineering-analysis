# Pi-Agent Context Engineering Analysis

An interactive analysis of how [Pi-Agent](https://github.com/earendil-works/pi-mono) manages context engineering — the strategies for building, constraining, and stabilizing context throughout an agent's lifecycle.

**[→ View Live Analysis](https://pi-context-engineering.vercel.app)**

## What's Inside

This project provides a deep-dive breakdown of Pi-Agent's context engineering approach from an AI Product Manager's perspective. The interactive web page covers:

| # | Section | Focus |
|---|---------|-------|
| 01 | 总览 | 三个基础矛盾与收敛入口 |
| 02 | 生命周期 | 一次任务中的上下文流动 |
| 03 | 启动 | 资源发现和信任边界 |
| 04 | 会话树 | 上下文不是线性聊天记录 |
| 05 | 系统提示词 | 最大的单次文本装配 |
| 06 | Agent Loop | 每轮调用前的最后装配线 |
| 07 | Compaction | 用摘要替代膨胀历史 |

## Project Structure

```
├── index.html              # Interactive analysis page
├── mermaid.min.js          # Diagram rendering library
├── docs/                   # Source analysis documents
│   ├── 01-概述与架构总览.md
│   ├── 02-完整生命周期中的上下文构建.md
│   ├── 03-上下文工程约束机制.md
│   ├── 04-上下文来源分类与稳定性约束.md
│   └── 05-额外发现与深度洞察.md
└── README.md
```

## Stack

- Pure HTML / CSS / JavaScript — zero build step
- [Mermaid.js](https://mermaid.js.org/) for architecture diagrams
- Single-file deployment, no dependencies

## Deploy

Hosted on [Vercel](https://vercel.com). Push to `main` to deploy automatically.

## License

Analysis content © Cissie (Xu Yahang). Pi-Agent source code belongs to its respective owners.
