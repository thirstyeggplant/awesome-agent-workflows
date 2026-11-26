# Awesome Agent Workflows [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> AI コーディングエージェントと働くための再現可能な方法：計画と仕様、タスクキュー、再利用できるプロンプトとスキル、レビューの関門、そして人を待つステップ。

このリストが扱うのはエージェントそのものではなく、その周りの仕事です。タスクをどう書き、分割し、引き渡し、確認し、承認するか。特に記載がない限り、項目はオープンソースか自由に読めるものです。

<!-- lang-bar -->
**🔗 ウェブサイト: [https://thirstyeggplant.github.io/awesome-agent-workflows/ja/](https://thirstyeggplant.github.io/awesome-agent-workflows/ja/)**

🌐 [English](readme.md) · [简体中文](readme.zh-CN.md) · [Español](readme.es.md) · **日本語** · [한국어](readme.ko.md) · [Português (BR)](readme.pt-BR.md) · [Français](readme.fr.md) · [Deutsch](readme.de.md) · [हिन्दी](readme.hi.md) · [বাংলা](readme.bn.md) · [Bahasa Indonesia](readme.id.md) · [العربية](readme.ar.md)
<!-- /lang-bar -->

<sub>英語版からの翻訳です。ツール名やサイト名は原文のままにしています。</sub>

<a id="contents"></a>
## 目次

- [注目](#featured)
- [原則とガイド](#principles-and-guides)
- [指示ファイルと標準](#instruction-files-and-standards)
- [計画と仕様駆動開発](#planning-and-spec-driven-development)
- [エージェントのためのタスク管理](#task-tracking-for-agents)
- [再利用できるプロンプト、スキル、サブエージェント](#reusable-prompts-skills-and-subagents)
- [レビューと承認](#review-and-approval)
- [エージェントを並べて動かす](#running-agents-side-by-side)
- [CI のエージェント](#agents-in-ci)
- [人が介在するフレームワーク](#frameworks-with-a-person-in-the-loop)
- [関連リスト](#related-lists)

<a id="featured"></a>
## 注目

- [Aubergine](https://github.com/thirstyeggplant/aubergine) - ブラウザのキャンバス上のターミナル。オーナーの承認を待てるステップを持つワークフロー、タスクキュー、使う前にレビューする下書きを備えています。*（このリストの管理者が開発しています。）*

<a id="principles-and-guides"></a>
## 原則とガイド

- [効果的なエージェントの作り方](https://www.anthropic.com/engineering/building-effective-agents) - プロンプトチェーンからオーケストレーターとワーカーまで、Anthropic によるワークフローとエージェントのパターン。
- [Claude Code のベストプラクティス](https://www.anthropic.com/engineering/claude-code-best-practices) - 調べる、計画する、書く、コミットする。人が介入できるチェックポイント付き。
- [12-Factor Agents](https://github.com/humanlayer/12-factor-agents) - 本番運用に耐えるエージェントのための原則。人への連絡をツール呼び出しとして扱うことも含みます。

<a id="instruction-files-and-standards"></a>
## 指示ファイルと標準

- [AGENTS.md](https://agents.md) - リポジトリに置くただの Markdown ファイルで、どのコーディングエージェントにもビルド、テスト、規約の守り方を伝えます。
- [Model Context Protocol](https://modelcontextprotocol.io) - エージェントにツールとコンテキストを与えるためのオープンプロトコル。こちらは [仕様](https://github.com/modelcontextprotocol/modelcontextprotocol).
- [Agent Skills](https://github.com/anthropics/skills) - タスクが必要とするときにエージェントが読み込む、指示とスクリプトのフォルダ。
- [Claude Code hooks](https://docs.claude.com/en/docs/claude-code/hooks) - エージェントのターンの決まった時点で実行されるコマンド。モデルの記憶に頼るべきでないチェックのために。

<a id="planning-and-spec-driven-development"></a>
## 計画と仕様駆動開発

- [Spec Kit](https://github.com/github/spec-kit) - エージェントがコードを書く前に、仕様、計画、タスクを書くための GitHub のツールキット。
- [OpenSpec](https://github.com/Fission-AI/OpenSpec) - 各変更をリポジトリ内のファイルとして提案・レビュー・保管する仕様駆動開発。
- [BMAD Method](https://github.com/bmad-code-org/BMAD-METHOD) - アナリストやアーキテクトから開発者、QA まで、アジャイルの役割をエージェントが担います。
- [Agent OS](https://github.com/buildermethods/agent-os) - コードベースの標準と仕様を、エージェントが参照するファイルに書き出します。
- [Superpowers](https://github.com/obra/superpowers) - ブレインストーミング、計画、テスト駆動開発、レビューへとエージェントを導くスキルライブラリ。

<a id="task-tracking-for-agents"></a>
## エージェントのためのタスク管理

- [Task Master](https://github.com/eyaltoledano/claude-task-master) - プロダクト文書を依存関係のあるタスクに分解し、エージェントが 1 つずつ進めます。
- [Beads](https://github.com/gastownhall/beads) - リポジトリ内に置く課題管理ツールで、エージェントが作業を起票・着手・完了できるように作られています。
- [Backlog.md](https://github.com/MrLesk/Backlog.md) - 人とエージェントが共有する、Git 上の Markdown タスクボード。

<a id="reusable-prompts-skills-and-subagents"></a>
## 再利用できるプロンプト、スキル、サブエージェント

- [Awesome Copilot](https://github.com/github/awesome-copilot) - GitHub Copilot 向けのコミュニティ製の指示、プロンプト、エージェント、スキル。
- [Awesome CursorRules](https://github.com/PatrickJS/awesome-cursorrules) - 言語とフレームワーク別に整理した Cursor のルールファイル。
- [Agents by wshobson](https://github.com/wshobson/agents) - Markdown で一度書くだけで、複数のコーディングエージェント向けに生成されるプラグイン、サブエージェント、コマンド。
- [Awesome Claude Code Subagents](https://github.com/VoltAgent/awesome-claude-code-subagents) - 100 を超える専門サブエージェントの定義。
- [Claude Cookbooks](https://github.com/anthropics/claude-cookbooks) - エージェントのワークフローやツール利用などのパターンを集めたノートブック。

<a id="review-and-approval"></a>
## レビューと承認

- [HumanLayer](https://github.com/humanlayer/humanlayer) - 難しい問題に取り組むコーディングエージェントのためのワークフロー。調査、計画、実装の各ステップを人がレビューします。
- [PR-Agent](https://github.com/The-PR-Agent/pr-agent) - プルリクエストにコメントするオープンソースのレビュアー。人のレビューに加える二重チェックとして。
- [Claude Code Security Review](https://github.com/anthropics/claude-code-security-review) - 変更ごとにセキュリティ上の問題をレビューする GitHub Action。

<a id="running-agents-side-by-side"></a>
## エージェントを並べて動かす

- [Claude Squad](https://github.com/smtg-ai/claude-squad) - 複数のターミナルエージェントを同時に、それぞれ専用の Git worktree で動かし、1 つのターミナルから管理します。
- [Container Use](https://github.com/dagger/container-use) - エージェントごとにコンテナとブランチを用意し、複数が衝突せずに 1 つのプロジェクトで作業できます。
- [Crystal](https://github.com/stravu/crystal) - worktree で並列にエージェントのセッションを走らせ、やり方を比べるデスクトップアプリ（現 Nimbalyst）。
- [Ruflo](https://github.com/ruvnet/ruflo) - Claude Code などを中心に、共有メモリを持つエージェント群を協調させます。

<a id="agents-in-ci"></a>
## CI のエージェント

- [Claude Code Action](https://github.com/anthropics/claude-code-action) - GitHub Actions で issue やプルリクエストから Claude Code を実行します。
- [OpenHands](https://github.com/OpenHands/OpenHands) - ローカル、クラウド、または CI でヘッドレスに動く、コーディングエージェントのためのオープンなプラットフォーム。
- [SWE-agent](https://github.com/SWE-agent/SWE-agent) - 好きな言語モデルを使って、GitHub の issue を受け取り修正を試みます。

<a id="frameworks-with-a-person-in-the-loop"></a>
## 人が介在するフレームワーク

- [LangGraph](https://github.com/langchain-ai/langgraph) - グラフとして構成したエージェントで、 [人のために一時停止](https://langchain-ai.github.io/langgraph/concepts/human_in_the_loop/) し、保存した状態から再開できます。
- [OpenAI Agents SDK](https://github.com/openai/openai-agents-python) - 引き継ぎとガードレールを備えた、マルチエージェントワークフローのための小さなフレームワーク。
- [CrewAI](https://github.com/crewAIInc/crewAI) - 役割を持つエージェントを編成し、タスクから人に入力を求めることもできます。

<a id="related-lists"></a>
## 関連リスト

- [Awesome Claude Code](https://github.com/hesreallyhim/awesome-claude-code) - Claude Code のためのスキル、フック、コマンド、ツール。

<a id="contributing"></a>
## コントリビュート

コントリビュート歓迎です。まず [コントリビューションガイドライン](contributing.md) をお読みください。
