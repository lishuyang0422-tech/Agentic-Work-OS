# Agentic-Work-OS

**简体中文 | [English](README.md)**

> 多 AI 协作工作系统  
> 一套本地优先、由文件结构驱动的 AI 工作协作系统，让不同 AI Agent 能读懂规则、接力项目、更新状态，并与你长期共同工作。

Agentic-Work-OS 不是一个知识库模板，也不是把所有资料塞进一个文件夹。

它是一套给 AI 在你的电脑上工作的行为协议：输入怎么进入、项目怎么推进、输出怎么交付、经验怎么沉淀、不同 Agent 怎么接力，都用可读的本地文件表达出来。

当一个对话线程出问题、模型额度不足、你想换另一个 Agent 继续做，新的 Agent 可以先读规则、状态和项目记录，再继续工作。上下文不再完全依赖某一个聊天窗口。

## 快速开始

1. 把本仓库复制到本地文件夹。
2. 用能读取本地文件的 AI Agent 打开它。
3. 对 Agent 说：

```text
请先阅读 AGENTS.md 和 System/Core，再运行一个 examples 里的 demo，并解释这个工作区如何运转。
```

4. 推荐先试两个 demo：
   - `examples/weekly-report-demo/`
   - `examples/agentic-work-os-research-demo/`

如果你是第一次使用，建议打开每个 demo 里的 `demo-walkthrough.md`。它会给你可复制的提示词、预期 Agent 动作、输出形态，以及留给下一个 Agent 接力的项目日志。

## 它解决什么问题

| 痛点 | 常见情况 | Agentic-Work-OS 的解法 |
|---|---|---|
| 画像级记忆 | AI 知道你的大致偏好，但记不住项目细节。 | 用项目状态和工作日志承载精准上下文。 |
| 概率级输出 | 每次生成的格式、语气、结构都可能漂移。 | 用规则、模板和验收标准降低漂移。 |
| 孤岛级对话 | 每个聊天窗口都是孤岛，互相不知道发生了什么。 | 让不同 Agent 共享同一套本地工作现场。 |
| 单 Agent 脆弱性 | 线程断裂、额度不足、模型切换会打断工作。 | 新 Agent 读取工作区即可接力。 |

## 核心机制

- **本地优先**：所有核心上下文都在本地文件里，你可以查看、复制、审计。
- **Agent 可读规则**：`AGENTS.md` 与 `System/Core/` 先告诉 Agent 怎么工作。
- **状态胜过记忆**：重要信息写入文件，而不是只留在聊天里。
- **输入输出路由**：原始材料进入 `input/`，成果进入 `output/`。
- **项目连续性**：活跃项目放在 `System/Active_Projects/`。
- **可复用资源**：稳定资料放在 `System/Resources/`。
- **系统成长**：日志、模板、roadmap 让系统在使用中迭代。

## 首版 Demo

### 周报 Demo

虚构用户把一周零散工作记录放入系统，Agent 整理成结构化周报，并记录项目进展。

入口：`examples/weekly-report-demo/demo-walkthrough.md`

### Agentic Work OS 调研 Demo

虚构用户放入几段关于 AI 协作系统的调研素材，Agent 生成一张解释 Agentic-Work-OS 的说明卡。用户在运行 demo 的同时，也能理解这个系统是什么。

入口：`examples/agentic-work-os-research-demo/demo-walkthrough.md`

## 它不是什么

- 不是私人工作区本体。
- 不是任何真实业务工作区。
- 不是完整教学沙箱。
- 不是某个厂商专属框架。
- 不是 RAG 服务器或向量数据库。

## 安全原则

不要把私有资料、公司文件、密钥、个人画像、客户记录或机密项目文件放进公开仓库。

更多说明见 `docs/safety-and-sanitization.md`。

## 许可证

MIT
