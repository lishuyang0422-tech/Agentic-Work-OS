# Introduction Copy

## 中文短版

Agentic-Work-OS 是一套本地优先的多 AI 协作工作系统。它不是知识库模板，而是一套让 AI Agent 在你的电脑上按规则工作、接力项目、沉淀经验的文件结构协议。

当一个对话线程断掉、模型额度不够、或者你想让另一个 Agent 接手时，新的 Agent 可以读取同一套规则、状态、项目日志和输出文件继续工作。上下文不再被锁死在某一个聊天窗口里。

首版包含两个完全虚构的 demo：周报整理 demo 和 Agentic Work OS 自解释调研 demo，帮助用户在几分钟内理解“输入 -> 处理 -> 输出 -> 留痕 -> 接力”的基本循环。

## 中文长版

我们常常把 AI 当成一个更聪明的聊天框：问一个问题，得到一个答案。但真实工作不是一次性问答。真实工作需要项目状态、文件归档、交付标准、协作记录、复盘机制，也需要在不同 AI Agent 之间顺畅接力。

Agentic-Work-OS 试图解决这个问题。

它把 AI 工作从单个聊天线程中释放出来，用本地文件结构承载规则、状态、项目、输入、输出和系统日志。这样一来，一个 Agent 做过的工作不会只停留在对话里；另一个 Agent 可以读取文件继续推进，人类也可以审计、修改和重组整个工作现场。

它特别适合这些场景：

- 一个 AI 线程太长、跑偏或中断，需要新线程继续；
- 不同模型适合不同任务，需要多 Agent 协作；
- 你希望把项目经验沉淀成可复用的规则和模板；
- 你不想把所有工作上下文交给单一平台或单一厂商。

Agentic-Work-OS 的目标不是替你保存一切，而是让 AI 知道如何与你一起工作。

## English Short Version

Agentic-Work-OS is a local-first workspace protocol for multi-agent collaboration. It is not a note-taking template. It gives AI agents a shared file-based work environment where they can read rules, route inputs, update project state, create outputs, and hand work off across threads or models.

The first release includes two fictional demos: a weekly report demo and a self-explaining Agentic Work OS research demo.

## English Long Version

Most AI work still lives inside fragile chat threads. That is fine for one-off questions, but real work needs continuity: project state, decisions, inputs, outputs, reusable references, and a way for another agent to continue when a thread breaks or a model changes.

Agentic-Work-OS is a small local-first starter system for that problem.

It uses a readable file structure to define how AI agents should work with a human: where to read rules, where to find current state, where raw inputs go, where outputs should be saved, and where meaningful changes should be logged.

This makes AI work easier to inspect, easier to hand off, and less dependent on one chat session or one vendor.

Use it if you want to experiment with:

- agent handoff across threads;
- multi-agent review and decision-making;
- file-based project memory;
- local-first AI workflows;
- public-safe workflow templates.

Agentic-Work-OS is not a private workspace export. It is a starter kit for designing your own AI-readable work system.
