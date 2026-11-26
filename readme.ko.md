# Awesome Agent Workflows [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> AI 코딩 에이전트와 일하는 반복 가능한 방법: 계획과 명세, 작업 큐, 재사용 가능한 프롬프트와 스킬, 리뷰 체크포인트, 그리고 사람을 기다리는 단계.

이 목록은 에이전트 자체가 아니라 에이전트를 둘러싼 일에 관한 것입니다. 작업을 어떻게 적고, 나누고, 넘기고, 확인하고, 승인하는지. 따로 표시하지 않은 항목은 오픈 소스이거나 자유롭게 읽을 수 있습니다.

<!-- lang-bar -->
**🔗 웹사이트: [https://thirstyeggplant.github.io/awesome-agent-workflows/ko/](https://thirstyeggplant.github.io/awesome-agent-workflows/ko/)**

🌐 [English](readme.md) · [简体中文](readme.zh-CN.md) · [Español](readme.es.md) · [日本語](readme.ja.md) · **한국어** · [Português (BR)](readme.pt-BR.md) · [Français](readme.fr.md) · [Deutsch](readme.de.md) · [हिन्दी](readme.hi.md) · [বাংলা](readme.bn.md) · [Bahasa Indonesia](readme.id.md) · [العربية](readme.ar.md)
<!-- /lang-bar -->

<sub>영어판을 번역한 문서입니다. 도구와 사이트 이름은 원문 그대로 두었습니다.</sub>

<a id="contents"></a>
## 목차

- [추천](#featured)
- [원칙과 가이드](#principles-and-guides)
- [지시 파일과 표준](#instruction-files-and-standards)
- [계획과 명세 기반 개발](#planning-and-spec-driven-development)
- [에이전트용 작업 관리](#task-tracking-for-agents)
- [재사용 가능한 프롬프트, 스킬, 서브에이전트](#reusable-prompts-skills-and-subagents)
- [리뷰와 승인](#review-and-approval)
- [에이전트 나란히 실행하기](#running-agents-side-by-side)
- [CI 속 에이전트](#agents-in-ci)
- [사람이 참여하는 프레임워크](#frameworks-with-a-person-in-the-loop)
- [관련 목록](#related-lists)

<a id="featured"></a>
## 추천

- [Aubergine](https://github.com/thirstyeggplant/aubergine) - 브라우저 캔버스 위의 터미널. 소유자의 승인을 기다릴 수 있는 단계로 된 워크플로, 작업 큐, 사용 전에 검토하는 초안을 제공합니다. *(이 목록의 관리자가 만들었습니다.)*

<a id="principles-and-guides"></a>
## 원칙과 가이드

- [효과적인 에이전트 만들기](https://www.anthropic.com/engineering/building-effective-agents) - 프롬프트 체이닝부터 오케스트레이터와 워커까지, 워크플로와 에이전트를 위한 Anthropic의 패턴.
- [Claude Code 모범 사례](https://www.anthropic.com/engineering/claude-code-best-practices) - 탐색, 계획, 코딩, 커밋. 사람이 개입할 수 있는 체크포인트와 함께.
- [12-Factor Agents](https://github.com/humanlayer/12-factor-agents) - 프로덕션에 쓸 만큼 믿을 수 있는 에이전트를 위한 원칙. 사람에게 연락하는 것을 도구 호출로 다루는 방법도 포함합니다.

<a id="instruction-files-and-standards"></a>
## 지시 파일과 표준

- [AGENTS.md](https://agents.md) - 저장소에 두는 평범한 Markdown 파일로, 어떤 코딩 에이전트에게든 빌드, 테스트, 규칙 준수 방법을 알려 줍니다.
- [Model Context Protocol](https://modelcontextprotocol.io) - 에이전트에게 도구와 컨텍스트를 제공하는 개방형 프로토콜. 관련 [명세](https://github.com/modelcontextprotocol/modelcontextprotocol).
- [Agent Skills](https://github.com/anthropics/skills) - 작업에 필요할 때 에이전트가 불러오는 지시문과 스크립트 폴더.
- [Claude Code hooks](https://docs.claude.com/en/docs/claude-code/hooks) - 에이전트 턴의 정해진 시점에 실행되는 명령. 모델의 기억에 의존하면 안 되는 검사를 위해.

<a id="planning-and-spec-driven-development"></a>
## 계획과 명세 기반 개발

- [Spec Kit](https://github.com/github/spec-kit) - 에이전트가 코드를 쓰기 전에 명세, 계획, 작업을 작성하기 위한 GitHub의 툴킷.
- [OpenSpec](https://github.com/Fission-AI/OpenSpec) - 각 변경을 저장소의 파일로 제안하고 검토하고 보관하는 명세 기반 개발.
- [BMAD Method](https://github.com/bmad-code-org/BMAD-METHOD) - 분석가와 아키텍트부터 개발자와 QA까지, 에이전트가 맡는 애자일 역할.
- [Agent OS](https://github.com/buildermethods/agent-os) - 코드베이스의 표준과 명세를 에이전트가 참고할 파일로 작성합니다.
- [Superpowers](https://github.com/obra/superpowers) - 브레인스토밍, 계획, 테스트 주도 개발, 리뷰 과정을 에이전트에게 안내하는 스킬 라이브러리.

<a id="task-tracking-for-agents"></a>
## 에이전트용 작업 관리

- [Task Master](https://github.com/eyaltoledano/claude-task-master) - 제품 문서를 의존 관계가 있는 작업으로 나누고, 에이전트가 하나씩 처리합니다.
- [Beads](https://github.com/gastownhall/beads) - 저장소 안에 두는 이슈 트래커로, 에이전트가 작업을 등록하고 맡고 닫을 수 있게 만들어졌습니다.
- [Backlog.md](https://github.com/MrLesk/Backlog.md) - 사람과 에이전트가 함께 쓰는 Git 속 Markdown 작업 보드.

<a id="reusable-prompts-skills-and-subagents"></a>
## 재사용 가능한 프롬프트, 스킬, 서브에이전트

- [Awesome Copilot](https://github.com/github/awesome-copilot) - GitHub Copilot을 위한 커뮤니티 지시문, 프롬프트, 에이전트, 스킬.
- [Awesome CursorRules](https://github.com/PatrickJS/awesome-cursorrules) - 언어와 프레임워크별로 정리한 Cursor 규칙 파일.
- [Agents by wshobson](https://github.com/wshobson/agents) - Markdown으로 한 번 작성해 여러 코딩 에이전트용으로 생성하는 플러그인, 서브에이전트, 명령.
- [Awesome Claude Code Subagents](https://github.com/VoltAgent/awesome-claude-code-subagents) - 100개가 넘는 전문 서브에이전트 정의.
- [Claude Cookbooks](https://github.com/anthropics/claude-cookbooks) - 에이전트 워크플로와 도구 사용을 포함한 패턴 노트북.

<a id="review-and-approval"></a>
## 리뷰와 승인

- [HumanLayer](https://github.com/humanlayer/humanlayer) - 어려운 문제를 다루는 코딩 에이전트용 워크플로. 조사, 계획, 구현 단계를 사람이 검토합니다.
- [PR-Agent](https://github.com/The-PR-Agent/pr-agent) - 풀 리퀘스트에 코멘트를 남기는 오픈 소스 리뷰어로, 사람의 리뷰에 더하는 두 번째 검토입니다.
- [Claude Code Security Review](https://github.com/anthropics/claude-code-security-review) - 모든 변경 사항의 보안 문제를 검토하는 GitHub Action.

<a id="running-agents-side-by-side"></a>
## 에이전트 나란히 실행하기

- [Claude Squad](https://github.com/smtg-ai/claude-squad) - 여러 터미널 에이전트를 동시에 각자의 Git worktree에서 실행하고 하나의 터미널에서 관리합니다.
- [Container Use](https://github.com/dagger/container-use) - 에이전트마다 컨테이너와 브랜치를 하나씩 두어, 여럿이 충돌 없이 한 프로젝트에서 작업합니다.
- [Crystal](https://github.com/stravu/crystal) - worktree에서 에이전트 세션을 병렬로 돌려 접근 방식을 비교하는 데스크톱 앱 (현재 Nimbalyst).
- [Ruflo](https://github.com/ruvnet/ruflo) - Claude Code 등을 중심으로 공유 메모리를 가진 에이전트 무리를 조율합니다.

<a id="agents-in-ci"></a>
## CI 속 에이전트

- [Claude Code Action](https://github.com/anthropics/claude-code-action) - GitHub Actions에서 이슈와 풀 리퀘스트로 Claude Code를 실행합니다.
- [OpenHands](https://github.com/OpenHands/OpenHands) - 로컬, 클라우드, 또는 CI에서 헤드리스로 실행되는 코딩 에이전트용 개방형 플랫폼.
- [SWE-agent](https://github.com/SWE-agent/SWE-agent) - 원하는 언어 모델로 GitHub 이슈를 받아 해결을 시도합니다.

<a id="frameworks-with-a-person-in-the-loop"></a>
## 사람이 참여하는 프레임워크

- [LangGraph](https://github.com/langchain-ai/langgraph) - 그래프로 구성한 에이전트로, [사람을 위해 멈추고](https://langchain-ai.github.io/langgraph/concepts/human_in_the_loop/) 저장된 상태에서 다시 이어 갈 수 있습니다.
- [OpenAI Agents SDK](https://github.com/openai/openai-agents-python) - 인계와 가드레일을 갖춘 멀티 에이전트 워크플로용 작은 프레임워크.
- [CrewAI](https://github.com/crewAIInc/crewAI) - 역할을 맡은 에이전트를 조율하며, 작업이 사람에게 입력을 요청할 수 있습니다.

<a id="related-lists"></a>
## 관련 목록

- [Awesome Claude Code](https://github.com/hesreallyhim/awesome-claude-code) - Claude Code용 스킬, 훅, 명령, 도구.

<a id="contributing"></a>
## 기여하기

기여를 환영합니다. 먼저 [기여 가이드라인](contributing.md) 을 읽어 주세요.
