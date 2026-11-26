# Awesome Agent Workflows [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> Formas repetibles de trabajar con agentes de programación con IA: planes y especificaciones, colas de tareas, prompts y skills reutilizables, puntos de revisión y pasos que esperan a una persona.

Esta lista trata del trabajo alrededor de un agente más que del agente en sí: cómo se escribe una tarea, cómo se divide, se entrega, se revisa y se aprueba. Las entradas son de código abierto o de lectura libre salvo que se indique lo contrario.

<!-- lang-bar -->
🌐 [English](readme.md) · [简体中文](readme.zh-CN.md) · **Español** · [日本語](readme.ja.md) · [한국어](readme.ko.md) · [Português (BR)](readme.pt-BR.md) · [Français](readme.fr.md) · [Deutsch](readme.de.md) · [हिन्दी](readme.hi.md) · [বাংলা](readme.bn.md) · [Bahasa Indonesia](readme.id.md) · [العربية](readme.ar.md) · 🔗 [Sitio web](https://thirstyeggplant.github.io/awesome-agent-workflows/es/)
<!-- /lang-bar -->

<sub>Traducción de la versión en inglés. Los nombres de herramientas y sitios se mantienen en su idioma original.</sub>

<a id="contents"></a>
## Contenido

- [Destacado](#featured)
- [Principios y guías](#principles-and-guides)
- [Archivos de instrucciones y estándares](#instruction-files-and-standards)
- [Planificación y desarrollo guiado por especificaciones](#planning-and-spec-driven-development)
- [Seguimiento de tareas para agentes](#task-tracking-for-agents)
- [Prompts, skills y subagentes reutilizables](#reusable-prompts-skills-and-subagents)
- [Revisión y aprobación](#review-and-approval)
- [Agentes en paralelo](#running-agents-side-by-side)
- [Agentes en CI](#agents-in-ci)
- [Frameworks con una persona en el circuito](#frameworks-with-a-person-in-the-loop)
- [Listas relacionadas](#related-lists)

<a id="featured"></a>
## Destacado

- [Aubergine](https://github.com/thirstyeggplant/aubergine) - Terminales en un lienzo en el navegador, con flujos de trabajo cuyos pasos pueden esperar la aprobación del propietario, una cola de tareas y borradores revisados antes de usarse. *(Mantenido por los autores de esta lista.)*

<a id="principles-and-guides"></a>
## Principios y guías

- [Cómo construir agentes eficaces](https://www.anthropic.com/engineering/building-effective-agents) - Los patrones de Anthropic para flujos de trabajo y agentes, desde el encadenamiento de prompts hasta orquestador y trabajadores.
- [Buenas prácticas de Claude Code](https://www.anthropic.com/engineering/claude-code-best-practices) - Explorar, planificar, programar y hacer commit, con puntos de control en los que puede intervenir una persona.
- [12-Factor Agents](https://github.com/humanlayer/12-factor-agents) - Principios para agentes lo bastante fiables para producción, incluido contactar a personas como una llamada a herramienta.

<a id="instruction-files-and-standards"></a>
## Archivos de instrucciones y estándares

- [AGENTS.md](https://agents.md) - Un archivo Markdown en un repositorio que explica a cualquier agente de programación cómo compilar, probar y seguir sus convenciones.
- [Model Context Protocol](https://modelcontextprotocol.io) - El protocolo abierto para dar herramientas y contexto a los agentes, con su [especificación](https://github.com/modelcontextprotocol/modelcontextprotocol).
- [Agent Skills](https://github.com/anthropics/skills) - Carpetas de instrucciones y scripts que un agente carga cuando una tarea lo requiere.
- [Claude Code hooks](https://docs.claude.com/en/docs/claude-code/hooks) - Comandos que se ejecutan en puntos fijos del turno de un agente, para comprobaciones que no deben depender de la memoria del modelo.

<a id="planning-and-spec-driven-development"></a>
## Planificación y desarrollo guiado por especificaciones

- [Spec Kit](https://github.com/github/spec-kit) - El kit de GitHub para escribir una especificación, un plan y tareas antes de que un agente escriba código.
- [OpenSpec](https://github.com/Fission-AI/OpenSpec) - Desarrollo guiado por especificaciones en el que cada cambio se propone, revisa y archiva como archivos del repositorio.
- [BMAD Method](https://github.com/bmad-code-org/BMAD-METHOD) - Roles ágiles interpretados por agentes, desde analista y arquitecto hasta desarrollador y QA.
- [Agent OS](https://github.com/buildermethods/agent-os) - Escribe los estándares y especificaciones de un código en archivos con los que trabajan los agentes.
- [Superpowers](https://github.com/obra/superpowers) - Una biblioteca de skills que guía a un agente por la lluvia de ideas, la planificación, el desarrollo guiado por pruebas y la revisión.

<a id="task-tracking-for-agents"></a>
## Seguimiento de tareas para agentes

- [Task Master](https://github.com/eyaltoledano/claude-task-master) - Convierte un documento de producto en tareas dependientes que un agente resuelve una a una.
- [Beads](https://github.com/gastownhall/beads) - Un gestor de incidencias dentro del repositorio, pensado para que los agentes abran, tomen y cierren trabajo.
- [Backlog.md](https://github.com/MrLesk/Backlog.md) - Un tablero de tareas en Markdown dentro de Git que comparten personas y agentes.

<a id="reusable-prompts-skills-and-subagents"></a>
## Prompts, skills y subagentes reutilizables

- [Awesome Copilot](https://github.com/github/awesome-copilot) - Instrucciones, prompts, agentes y skills de la comunidad para GitHub Copilot.
- [Awesome CursorRules](https://github.com/PatrickJS/awesome-cursorrules) - Archivos de reglas para Cursor, ordenados por lenguaje y framework.
- [Agents by wshobson](https://github.com/wshobson/agents) - Plugins, subagentes y comandos escritos una vez en Markdown y generados para varios agentes de programación.
- [Awesome Claude Code Subagents](https://github.com/VoltAgent/awesome-claude-code-subagents) - Más de cien definiciones de subagentes especializados.
- [Claude Cookbooks](https://github.com/anthropics/claude-cookbooks) - Cuadernos con patrones, incluidos flujos de agentes y uso de herramientas.

<a id="review-and-approval"></a>
## Revisión y aprobación

- [HumanLayer](https://github.com/humanlayer/humanlayer) - Flujos para agentes de programación en problemas difíciles, con pasos de investigación, plan e implementación que revisa una persona.
- [PR-Agent](https://github.com/The-PR-Agent/pr-agent) - Un revisor de código abierto que comenta pull requests, como segunda pasada junto a la revisión de una persona.
- [Claude Code Security Review](https://github.com/anthropics/claude-code-security-review) - Una GitHub Action que revisa cada cambio en busca de problemas de seguridad.

<a id="running-agents-side-by-side"></a>
## Agentes en paralelo

- [Claude Squad](https://github.com/smtg-ai/claude-squad) - Varios agentes de terminal a la vez, cada uno en su propio worktree de Git, gestionados desde una terminal.
- [Container Use](https://github.com/dagger/container-use) - Un contenedor y una rama por agente, para que varios trabajen en un proyecto sin chocar.
- [Crystal](https://github.com/stravu/crystal) - Una app de escritorio para sesiones de agentes en paralelo en worktrees, para comparar enfoques (ahora Nimbalyst).
- [Ruflo](https://github.com/ruvnet/ruflo) - Coordina enjambres de agentes con memoria compartida en torno a Claude Code y otros agentes.

<a id="agents-in-ci"></a>
## Agentes en CI

- [Claude Code Action](https://github.com/anthropics/claude-code-action) - Ejecuta Claude Code desde issues y pull requests en GitHub Actions.
- [OpenHands](https://github.com/OpenHands/OpenHands) - Una plataforma abierta para agentes de programación que funciona en local, en la nube o sin interfaz en CI.
- [SWE-agent](https://github.com/SWE-agent/SWE-agent) - Toma un issue de GitHub e intenta resolverlo con el modelo de lenguaje que elijas.

<a id="frameworks-with-a-person-in-the-loop"></a>
## Frameworks con una persona en el circuito

- [LangGraph](https://github.com/langchain-ai/langgraph) - Agentes como grafos que pueden [pausarse para una persona](https://langchain-ai.github.io/langgraph/concepts/human_in_the_loop/) y reanudar desde un estado guardado.
- [OpenAI Agents SDK](https://github.com/openai/openai-agents-python) - Un framework ligero para flujos multiagente con traspasos y salvaguardas.
- [CrewAI](https://github.com/crewAIInc/crewAI) - Orquesta agentes que interpretan roles, con tareas que pueden pedir información a una persona.

<a id="related-lists"></a>
## Listas relacionadas

- [Awesome Claude Code](https://github.com/hesreallyhim/awesome-claude-code) - Skills, hooks, comandos y herramientas para Claude Code.

<a id="contributing"></a>
## Contribuir

Las contribuciones son bienvenidas. Lee primero la [guía de contribución](contributing.md) .
