# Awesome Agent Workflows [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> 与 AI 编程智能体协作的可复用方法：计划与规格、任务队列、可复用的提示词和技能、评审检查点，以及等待人工确认的步骤。

本列表关注的是智能体周围的工作，而不是智能体本身：任务如何被写下、拆分、移交、检查和批准。除非另有说明，条目均为开源或可免费阅读。

<!-- lang-bar -->
🌐 [English](readme.md) · **简体中文** · [Español](readme.es.md) · [日本語](readme.ja.md) · [한국어](readme.ko.md) · [Português (BR)](readme.pt-BR.md) · [Français](readme.fr.md) · [Deutsch](readme.de.md) · [हिन्दी](readme.hi.md) · [বাংলা](readme.bn.md) · [Bahasa Indonesia](readme.id.md) · [العربية](readme.ar.md) · 🔗 [网站](https://thirstyeggplant.github.io/awesome-agent-workflows/zh-CN/)
<!-- /lang-bar -->

<sub>本页译自英文版。工具和网站名称保留原文。</sub>

<a id="contents"></a>
## 目录

- [精选推荐](#featured)
- [原则与指南](#principles-and-guides)
- [指令文件与标准](#instruction-files-and-standards)
- [规划与规格驱动开发](#planning-and-spec-driven-development)
- [面向智能体的任务跟踪](#task-tracking-for-agents)
- [可复用的提示词、技能和子智能体](#reusable-prompts-skills-and-subagents)
- [评审与批准](#review-and-approval)
- [并行运行智能体](#running-agents-side-by-side)
- [CI 中的智能体](#agents-in-ci)
- [有人参与环节的框架](#frameworks-with-a-person-in-the-loop)
- [相关列表](#related-lists)

<a id="featured"></a>
## 精选推荐

- [Aubergine](https://github.com/thirstyeggplant/aubergine) - 浏览器画布上的终端，带有可等待所有者批准的工作流步骤、任务队列，以及使用前需审阅的草稿。*（由本列表的维护者开发。）*

<a id="principles-and-guides"></a>
## 原则与指南

- [构建高效的智能体](https://www.anthropic.com/engineering/building-effective-agents) - Anthropic 总结的工作流与智能体模式，从提示词链到编排者与执行者。
- [Claude Code 最佳实践](https://www.anthropic.com/engineering/claude-code-best-practices) - 探索、规划、编码、提交，并设有人可以介入的检查点。
- [12-Factor Agents](https://github.com/humanlayer/12-factor-agents) - 让智能体足以用于生产环境的原则，包括把联系人工作为一次工具调用。

<a id="instruction-files-and-standards"></a>
## 指令文件与标准

- [AGENTS.md](https://agents.md) - 仓库中的一个普通 Markdown 文件，告诉任何编程智能体如何构建、测试并遵循项目约定。
- [Model Context Protocol](https://modelcontextprotocol.io) - 为智能体提供工具和上下文的开放协议，另见其 [规范](https://github.com/modelcontextprotocol/modelcontextprotocol).
- [Agent Skills](https://github.com/anthropics/skills) - 由指令和脚本组成的文件夹，智能体在任务需要时加载。
- [Claude Code hooks](https://docs.claude.com/en/docs/claude-code/hooks) - 在智能体回合的固定时刻运行的命令，用于不应依赖模型记忆的检查。

<a id="planning-and-spec-driven-development"></a>
## 规划与规格驱动开发

- [Spec Kit](https://github.com/github/spec-kit) - GitHub 的工具包，在智能体写代码之前先写好规格、计划和任务。
- [OpenSpec](https://github.com/Fission-AI/OpenSpec) - 规格驱动开发：每个变更都以仓库中的文件形式提出、评审和归档。
- [BMAD Method](https://github.com/bmad-code-org/BMAD-METHOD) - 由智能体扮演的敏捷角色，从分析师、架构师到开发者和测试。
- [Agent OS](https://github.com/buildermethods/agent-os) - 把代码库的标准和规格写成智能体可依据的文件。
- [Superpowers](https://github.com/obra/superpowers) - 一个技能库，引导智能体完成头脑风暴、规划、测试驱动开发和评审。

<a id="task-tracking-for-agents"></a>
## 面向智能体的任务跟踪

- [Task Master](https://github.com/eyaltoledano/claude-task-master) - 把产品文档拆成有依赖关系的任务，让智能体逐个完成。
- [Beads](https://github.com/gastownhall/beads) - 存放在仓库中的问题跟踪器，专为智能体创建、领取和关闭任务而设计。
- [Backlog.md](https://github.com/MrLesk/Backlog.md) - 放在 Git 中、由人和智能体共享的 Markdown 任务看板。

<a id="reusable-prompts-skills-and-subagents"></a>
## 可复用的提示词、技能和子智能体

- [Awesome Copilot](https://github.com/github/awesome-copilot) - 面向 GitHub Copilot 的社区指令、提示词、智能体和技能。
- [Awesome CursorRules](https://github.com/PatrickJS/awesome-cursorrules) - Cursor 规则文件，按语言和框架分类。
- [Agents by wshobson](https://github.com/wshobson/agents) - 用 Markdown 编写一次即可为多个编程智能体生成的插件、子智能体和命令。
- [Awesome Claude Code Subagents](https://github.com/VoltAgent/awesome-claude-code-subagents) - 一百多个专业子智能体定义。
- [Claude Cookbooks](https://github.com/anthropics/claude-cookbooks) - 收录各种模式的笔记本，包括智能体工作流和工具调用。

<a id="review-and-approval"></a>
## 评审与批准

- [HumanLayer](https://github.com/humanlayer/humanlayer) - 面向难题的编程智能体工作流，包含由人评审的调研、规划和实现步骤。
- [PR-Agent](https://github.com/The-PR-Agent/pr-agent) - 一个开源的代码评审工具，会在 pull request 上发表评论，作为人工评审之外的第二道把关。
- [Claude Code Security Review](https://github.com/anthropics/claude-code-security-review) - 一个检查每次变更安全问题的 GitHub Action。

<a id="running-agents-side-by-side"></a>
## 并行运行智能体

- [Claude Squad](https://github.com/smtg-ai/claude-squad) - 同时运行多个终端智能体，各自位于独立的 Git worktree，并在一个终端中统一管理。
- [Container Use](https://github.com/dagger/container-use) - 每个智能体一个容器和一个分支，让多个智能体在同一项目中互不干扰。
- [Crystal](https://github.com/stravu/crystal) - 在 worktree 中并行运行智能体会话的桌面应用，便于比较不同方案（现名 Nimbalyst）。
- [Ruflo](https://github.com/ruvnet/ruflo) - 围绕 Claude Code 等智能体，协调共享记忆的智能体集群。

<a id="agents-in-ci"></a>
## CI 中的智能体

- [Claude Code Action](https://github.com/anthropics/claude-code-action) - 在 GitHub Actions 中通过 issue 和 pull request 运行 Claude Code。
- [OpenHands](https://github.com/OpenHands/OpenHands) - 开放的编程智能体平台，可在本地、云端或 CI 中无界面运行。
- [SWE-agent](https://github.com/SWE-agent/SWE-agent) - 接收一个 GitHub issue 并尝试修复，可使用你选择的语言模型。

<a id="frameworks-with-a-person-in-the-loop"></a>
## 有人参与环节的框架

- [LangGraph](https://github.com/langchain-ai/langgraph) - 以图的形式构建智能体，可以 [暂停等待人工](https://langchain-ai.github.io/langgraph/concepts/human_in_the_loop/) 并从保存的状态继续运行。
- [OpenAI Agents SDK](https://github.com/openai/openai-agents-python) - 一个支持交接和防护机制的轻量多智能体工作流框架。
- [CrewAI](https://github.com/crewAIInc/crewAI) - 编排扮演不同角色的智能体，任务可以向人请求输入。

<a id="related-lists"></a>
## 相关列表

- [Awesome Claude Code](https://github.com/hesreallyhim/awesome-claude-code) - Claude Code 的技能、钩子、命令和工具。

<a id="contributing"></a>
## 参与贡献

欢迎贡献。请先阅读 [贡献指南](contributing.md) 。
