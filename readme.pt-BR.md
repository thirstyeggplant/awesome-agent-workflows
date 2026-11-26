# Awesome Agent Workflows [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> Formas repetíveis de trabalhar com agentes de programação com IA: planos e especificações, filas de tarefas, prompts e skills reutilizáveis, pontos de revisão e etapas que esperam por uma pessoa.

Esta lista trata do trabalho em volta de um agente, e não do agente em si: como uma tarefa é escrita, dividida, entregue, conferida e aprovada. Os itens são open source ou de leitura livre, salvo indicação em contrário.

<!-- lang-bar -->
**🔗 Site: [https://thirstyeggplant.github.io/awesome-agent-workflows/pt-BR/](https://thirstyeggplant.github.io/awesome-agent-workflows/pt-BR/)**

🌐 [English](readme.md) · [简体中文](readme.zh-CN.md) · [Español](readme.es.md) · [日本語](readme.ja.md) · [한국어](readme.ko.md) · **Português (BR)** · [Français](readme.fr.md) · [Deutsch](readme.de.md) · [हिन्दी](readme.hi.md) · [বাংলা](readme.bn.md) · [Bahasa Indonesia](readme.id.md) · [العربية](readme.ar.md)
<!-- /lang-bar -->

<sub>Tradução da versão em inglês. Nomes de ferramentas e sites foram mantidos no original.</sub>

<a id="contents"></a>
## Conteúdo

- [Destaque](#featured)
- [Princípios e guias](#principles-and-guides)
- [Arquivos de instruções e padrões](#instruction-files-and-standards)
- [Planejamento e desenvolvimento guiado por especificações](#planning-and-spec-driven-development)
- [Acompanhamento de tarefas para agentes](#task-tracking-for-agents)
- [Prompts, skills e subagentes reutilizáveis](#reusable-prompts-skills-and-subagents)
- [Revisão e aprovação](#review-and-approval)
- [Agentes lado a lado](#running-agents-side-by-side)
- [Agentes em CI](#agents-in-ci)
- [Frameworks com uma pessoa no circuito](#frameworks-with-a-person-in-the-loop)
- [Listas relacionadas](#related-lists)

<a id="featured"></a>
## Destaque

- [Aubergine](https://github.com/thirstyeggplant/aubergine) - Terminais em uma tela no navegador, com fluxos cujas etapas podem esperar a aprovação do dono, uma fila de tarefas e rascunhos revisados antes do uso. *(Mantido pelos donos desta lista.)*

<a id="principles-and-guides"></a>
## Princípios e guias

- [Como construir agentes eficazes](https://www.anthropic.com/engineering/building-effective-agents) - Os padrões da Anthropic para fluxos e agentes, do encadeamento de prompts a orquestrador e trabalhadores.
- [Boas práticas do Claude Code](https://www.anthropic.com/engineering/claude-code-best-practices) - Explorar, planejar, programar e fazer commit, com pontos de controle em que uma pessoa pode intervir.
- [12-Factor Agents](https://github.com/humanlayer/12-factor-agents) - Princípios para agentes confiáveis o bastante para produção, incluindo contatar pessoas como uma chamada de ferramenta.

<a id="instruction-files-and-standards"></a>
## Arquivos de instruções e padrões

- [AGENTS.md](https://agents.md) - Um arquivo Markdown simples no repositório que diz a qualquer agente de programação como compilar, testar e seguir as convenções.
- [Model Context Protocol](https://modelcontextprotocol.io) - O protocolo aberto para dar ferramentas e contexto aos agentes, com sua [especificação](https://github.com/modelcontextprotocol/modelcontextprotocol).
- [Agent Skills](https://github.com/anthropics/skills) - Pastas de instruções e scripts que um agente carrega quando a tarefa pede.
- [Claude Code hooks](https://docs.claude.com/en/docs/claude-code/hooks) - Comandos que rodam em pontos fixos do turno de um agente, para verificações que não devem depender da memória do modelo.

<a id="planning-and-spec-driven-development"></a>
## Planejamento e desenvolvimento guiado por especificações

- [Spec Kit](https://github.com/github/spec-kit) - O kit do GitHub para escrever uma especificação, um plano e tarefas antes de um agente escrever código.
- [OpenSpec](https://github.com/Fission-AI/OpenSpec) - Desenvolvimento guiado por especificações em que cada mudança é proposta, revisada e arquivada como arquivos no repositório.
- [BMAD Method](https://github.com/bmad-code-org/BMAD-METHOD) - Papéis ágeis desempenhados por agentes, de analista e arquiteto a desenvolvedor e QA.
- [Agent OS](https://github.com/buildermethods/agent-os) - Registra os padrões e especificações de uma base de código em arquivos usados pelos agentes.
- [Superpowers](https://github.com/obra/superpowers) - Uma biblioteca de skills que conduz o agente por brainstorming, planejamento, TDD e revisão.

<a id="task-tracking-for-agents"></a>
## Acompanhamento de tarefas para agentes

- [Task Master](https://github.com/eyaltoledano/claude-task-master) - Transforma um documento de produto em tarefas dependentes que o agente resolve uma por vez.
- [Beads](https://github.com/gastownhall/beads) - Um rastreador de issues dentro do repositório, feito para agentes abrirem, assumirem e fecharem trabalho.
- [Backlog.md](https://github.com/MrLesk/Backlog.md) - Um quadro de tarefas em Markdown no Git, compartilhado por pessoas e agentes.

<a id="reusable-prompts-skills-and-subagents"></a>
## Prompts, skills e subagentes reutilizáveis

- [Awesome Copilot](https://github.com/github/awesome-copilot) - Instruções, prompts, agentes e skills da comunidade para o GitHub Copilot.
- [Awesome CursorRules](https://github.com/PatrickJS/awesome-cursorrules) - Arquivos de regras para o Cursor, organizados por linguagem e framework.
- [Agents by wshobson](https://github.com/wshobson/agents) - Plugins, subagentes e comandos escritos uma vez em Markdown e gerados para vários agentes de programação.
- [Awesome Claude Code Subagents](https://github.com/VoltAgent/awesome-claude-code-subagents) - Mais de cem definições de subagentes especializados.
- [Claude Cookbooks](https://github.com/anthropics/claude-cookbooks) - Notebooks com padrões, incluindo fluxos de agentes e uso de ferramentas.

<a id="review-and-approval"></a>
## Revisão e aprovação

- [HumanLayer](https://github.com/humanlayer/humanlayer) - Fluxos para agentes de programação em problemas difíceis, com etapas de pesquisa, plano e implementação revisadas por uma pessoa.
- [PR-Agent](https://github.com/The-PR-Agent/pr-agent) - Um revisor open source que comenta pull requests, uma segunda passada ao lado da revisão humana.
- [Claude Code Security Review](https://github.com/anthropics/claude-code-security-review) - Uma GitHub Action que revisa cada mudança em busca de problemas de segurança.

<a id="running-agents-side-by-side"></a>
## Agentes lado a lado

- [Claude Squad](https://github.com/smtg-ai/claude-squad) - Vários agentes de terminal ao mesmo tempo, cada um em seu próprio worktree do Git, gerenciados a partir de um terminal.
- [Container Use](https://github.com/dagger/container-use) - Um contêiner e um branch por agente, para que vários trabalhem no mesmo projeto sem conflito.
- [Crystal](https://github.com/stravu/crystal) - Um app de desktop para sessões paralelas de agentes em worktrees, para comparar abordagens (agora Nimbalyst).
- [Ruflo](https://github.com/ruvnet/ruflo) - Coordena enxames de agentes com memória compartilhada em torno do Claude Code e de outros agentes.

<a id="agents-in-ci"></a>
## Agentes em CI

- [Claude Code Action](https://github.com/anthropics/claude-code-action) - Executa o Claude Code a partir de issues e pull requests no GitHub Actions.
- [OpenHands](https://github.com/OpenHands/OpenHands) - Uma plataforma aberta para agentes de programação que roda localmente, na nuvem ou sem interface em CI.
- [SWE-agent](https://github.com/SWE-agent/SWE-agent) - Pega uma issue do GitHub e tenta corrigi-la, com o modelo de linguagem que você escolher.

<a id="frameworks-with-a-person-in-the-loop"></a>
## Frameworks com uma pessoa no circuito

- [LangGraph](https://github.com/langchain-ai/langgraph) - Agentes como grafos que podem [pausar para uma pessoa](https://langchain-ai.github.io/langgraph/concepts/human_in_the_loop/) e retomar de um estado salvo.
- [OpenAI Agents SDK](https://github.com/openai/openai-agents-python) - Um framework enxuto para fluxos multiagente com repasses e salvaguardas.
- [CrewAI](https://github.com/crewAIInc/crewAI) - Orquestra agentes que desempenham papéis, com tarefas que podem pedir informações a uma pessoa.

<a id="related-lists"></a>
## Listas relacionadas

- [Awesome Claude Code](https://github.com/hesreallyhim/awesome-claude-code) - Skills, hooks, comandos e ferramentas para o Claude Code.

<a id="contributing"></a>
## Como contribuir

Contribuições são bem-vindas. Leia primeiro as [diretrizes de contribuição](contributing.md) .
