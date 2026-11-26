# Awesome Agent Workflows [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> Des façons reproductibles de travailler avec des agents de code IA : plans et spécifications, files de tâches, prompts et skills réutilisables, points de relecture et étapes qui attendent une personne.

Cette liste porte sur le travail autour d’un agent plutôt que sur l’agent lui-même : comment une tâche est rédigée, découpée, transmise, vérifiée et validée. Les entrées sont open source ou librement consultables, sauf mention contraire.

<!-- lang-bar -->
🌐 [English](readme.md) · [简体中文](readme.zh-CN.md) · [Español](readme.es.md) · [日本語](readme.ja.md) · [한국어](readme.ko.md) · [Português (BR)](readme.pt-BR.md) · **Français** · [Deutsch](readme.de.md) · [हिन्दी](readme.hi.md) · [বাংলা](readme.bn.md) · [Bahasa Indonesia](readme.id.md) · [العربية](readme.ar.md) · 🔗 [Site web](https://thirstyeggplant.github.io/awesome-agent-workflows/fr/)
<!-- /lang-bar -->

<sub>Traduction de la version anglaise. Les noms d’outils et de sites sont laissés dans leur langue d’origine.</sub>

<a id="contents"></a>
## Sommaire

- [À la une](#featured)
- [Principes et guides](#principles-and-guides)
- [Fichiers d’instructions et standards](#instruction-files-and-standards)
- [Planification et développement piloté par les spécifications](#planning-and-spec-driven-development)
- [Suivi des tâches pour agents](#task-tracking-for-agents)
- [Prompts, skills et sous-agents réutilisables](#reusable-prompts-skills-and-subagents)
- [Relecture et validation](#review-and-approval)
- [Plusieurs agents côte à côte](#running-agents-side-by-side)
- [Agents en CI](#agents-in-ci)
- [Frameworks avec une personne dans la boucle](#frameworks-with-a-person-in-the-loop)
- [Listes connexes](#related-lists)

<a id="featured"></a>
## À la une

- [Aubergine](https://github.com/thirstyeggplant/aubergine) - Des terminaux sur un canevas dans le navigateur, avec des workflows dont les étapes peuvent attendre l’accord du propriétaire, une file de tâches et des brouillons relus avant usage. *(Maintenu par les auteurs de cette liste.)*

<a id="principles-and-guides"></a>
## Principes et guides

- [Construire des agents efficaces](https://www.anthropic.com/engineering/building-effective-agents) - Les patterns d’Anthropic pour les workflows et les agents, de l’enchaînement de prompts à l’orchestrateur et ses exécutants.
- [Bonnes pratiques de Claude Code](https://www.anthropic.com/engineering/claude-code-best-practices) - Explorer, planifier, coder et committer, avec des points de contrôle où une personne peut intervenir.
- [12-Factor Agents](https://github.com/humanlayer/12-factor-agents) - Des principes pour des agents assez fiables pour la production, dont le fait de contacter une personne via un appel d’outil.

<a id="instruction-files-and-standards"></a>
## Fichiers d’instructions et standards

- [AGENTS.md](https://agents.md) - Un simple fichier Markdown dans un dépôt qui explique à n’importe quel agent de code comment compiler, tester et suivre les conventions.
- [Model Context Protocol](https://modelcontextprotocol.io) - Le protocole ouvert pour donner outils et contexte aux agents, avec sa [spécification](https://github.com/modelcontextprotocol/modelcontextprotocol).
- [Agent Skills](https://github.com/anthropics/skills) - Des dossiers d’instructions et de scripts qu’un agent charge quand une tâche le demande.
- [Claude Code hooks](https://docs.claude.com/en/docs/claude-code/hooks) - Des commandes exécutées à des moments fixes du tour d’un agent, pour des vérifications qui ne doivent pas dépendre de la mémoire du modèle.

<a id="planning-and-spec-driven-development"></a>
## Planification et développement piloté par les spécifications

- [Spec Kit](https://github.com/github/spec-kit) - La boîte à outils de GitHub pour rédiger une spécification, un plan et des tâches avant qu’un agent écrive du code.
- [OpenSpec](https://github.com/Fission-AI/OpenSpec) - Développement piloté par les spécifications où chaque changement est proposé, relu et archivé sous forme de fichiers dans le dépôt.
- [BMAD Method](https://github.com/bmad-code-org/BMAD-METHOD) - Des rôles agiles tenus par des agents, de l’analyste et l’architecte au développeur et au testeur.
- [Agent OS](https://github.com/buildermethods/agent-os) - Consigne les standards et spécifications d’une base de code dans des fichiers sur lesquels travaillent les agents.
- [Superpowers](https://github.com/obra/superpowers) - Une bibliothèque de skills qui guide un agent à travers le brainstorming, la planification, le TDD et la relecture.

<a id="task-tracking-for-agents"></a>
## Suivi des tâches pour agents

- [Task Master](https://github.com/eyaltoledano/claude-task-master) - Transforme un document produit en tâches dépendantes qu’un agent traite une par une.
- [Beads](https://github.com/gastownhall/beads) - Un gestionnaire de tickets dans le dépôt, conçu pour que les agents créent, prennent et clôturent le travail.
- [Backlog.md](https://github.com/MrLesk/Backlog.md) - Un tableau de tâches en Markdown dans Git, partagé par les personnes et les agents.

<a id="reusable-prompts-skills-and-subagents"></a>
## Prompts, skills et sous-agents réutilisables

- [Awesome Copilot](https://github.com/github/awesome-copilot) - Instructions, prompts, agents et skills de la communauté pour GitHub Copilot.
- [Awesome CursorRules](https://github.com/PatrickJS/awesome-cursorrules) - Fichiers de règles pour Cursor, classés par langage et framework.
- [Agents by wshobson](https://github.com/wshobson/agents) - Plugins, sous-agents et commandes écrits une fois en Markdown et générés pour plusieurs agents de code.
- [Awesome Claude Code Subagents](https://github.com/VoltAgent/awesome-claude-code-subagents) - Plus d’une centaine de définitions de sous-agents spécialisés.
- [Claude Cookbooks](https://github.com/anthropics/claude-cookbooks) - Des notebooks de patterns, dont des workflows d’agents et l’usage d’outils.

<a id="review-and-approval"></a>
## Relecture et validation

- [HumanLayer](https://github.com/humanlayer/humanlayer) - Des workflows pour agents de code sur des problèmes difficiles, avec des étapes de recherche, de plan et d’implémentation relues par une personne.
- [PR-Agent](https://github.com/The-PR-Agent/pr-agent) - Un relecteur open source qui commente les pull requests, en complément de la relecture humaine.
- [Claude Code Security Review](https://github.com/anthropics/claude-code-security-review) - Une GitHub Action qui examine chaque changement à la recherche de problèmes de sécurité.

<a id="running-agents-side-by-side"></a>
## Plusieurs agents côte à côte

- [Claude Squad](https://github.com/smtg-ai/claude-squad) - Plusieurs agents en terminal à la fois, chacun dans son propre worktree Git, pilotés depuis un seul terminal.
- [Container Use](https://github.com/dagger/container-use) - Un conteneur et une branche par agent, pour que plusieurs travaillent sur un projet sans se marcher dessus.
- [Crystal](https://github.com/stravu/crystal) - Une application de bureau pour des sessions d’agents en parallèle dans des worktrees, afin de comparer les approches (désormais Nimbalyst).
- [Ruflo](https://github.com/ruvnet/ruflo) - Coordonne des essaims d’agents à mémoire partagée autour de Claude Code et d’autres agents.

<a id="agents-in-ci"></a>
## Agents en CI

- [Claude Code Action](https://github.com/anthropics/claude-code-action) - Lance Claude Code depuis les issues et pull requests dans GitHub Actions.
- [OpenHands](https://github.com/OpenHands/OpenHands) - Une plateforme ouverte pour agents de code, en local, dans le cloud ou sans interface en CI.
- [SWE-agent](https://github.com/SWE-agent/SWE-agent) - Prend une issue GitHub et tente de la corriger, avec le modèle de langage de votre choix.

<a id="frameworks-with-a-person-in-the-loop"></a>
## Frameworks avec une personne dans la boucle

- [LangGraph](https://github.com/langchain-ai/langgraph) - Des agents sous forme de graphes qui peuvent [se mettre en pause pour une personne](https://langchain-ai.github.io/langgraph/concepts/human_in_the_loop/) et reprendre depuis un état sauvegardé.
- [OpenAI Agents SDK](https://github.com/openai/openai-agents-python) - Un petit framework pour workflows multi-agents avec passages de relais et garde-fous.
- [CrewAI](https://github.com/crewAIInc/crewAI) - Orchestre des agents qui jouent des rôles, avec des tâches pouvant demander l’avis d’une personne.

<a id="related-lists"></a>
## Listes connexes

- [Awesome Claude Code](https://github.com/hesreallyhim/awesome-claude-code) - Skills, hooks, commandes et outils pour Claude Code.

<a id="contributing"></a>
## Contribuer

Les contributions sont les bienvenues. Lisez d’abord les [règles de contribution](contributing.md) .
