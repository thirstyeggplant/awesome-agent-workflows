# Awesome Agent Workflows [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> Wiederholbare Arbeitsweisen mit KI-Coding-Agenten: Pläne und Spezifikationen, Aufgabenwarteschlangen, wiederverwendbare Prompts und Skills, Prüfpunkte und Schritte, die auf einen Menschen warten.

Diese Liste dreht sich um die Arbeit rund um einen Agenten, nicht um den Agenten selbst: wie eine Aufgabe aufgeschrieben, aufgeteilt, übergeben, geprüft und freigegeben wird. Einträge sind Open Source oder frei lesbar, sofern nicht anders vermerkt.

<!-- lang-bar -->
**🔗 Website: [https://thirstyeggplant.github.io/awesome-agent-workflows/de/](https://thirstyeggplant.github.io/awesome-agent-workflows/de/)**

🌐 [English](readme.md) · [简体中文](readme.zh-CN.md) · [Español](readme.es.md) · [日本語](readme.ja.md) · [한국어](readme.ko.md) · [Português (BR)](readme.pt-BR.md) · [Français](readme.fr.md) · **Deutsch** · [हिन्दी](readme.hi.md) · [বাংলা](readme.bn.md) · [Bahasa Indonesia](readme.id.md) · [العربية](readme.ar.md)
<!-- /lang-bar -->

<sub>Übersetzung der englischen Fassung. Namen von Tools und Websites bleiben im Original.</sub>

<a id="contents"></a>
## Inhalt

- [Empfohlen](#featured)
- [Prinzipien und Leitfäden](#principles-and-guides)
- [Anweisungsdateien und Standards](#instruction-files-and-standards)
- [Planung und spezifikationsgetriebene Entwicklung](#planning-and-spec-driven-development)
- [Aufgabenverwaltung für Agenten](#task-tracking-for-agents)
- [Wiederverwendbare Prompts, Skills und Subagenten](#reusable-prompts-skills-and-subagents)
- [Prüfung und Freigabe](#review-and-approval)
- [Agenten nebeneinander ausführen](#running-agents-side-by-side)
- [Agenten in CI](#agents-in-ci)
- [Frameworks mit einem Menschen im Ablauf](#frameworks-with-a-person-in-the-loop)
- [Verwandte Listen](#related-lists)

<a id="featured"></a>
## Empfohlen

- [Aubergine](https://github.com/thirstyeggplant/aubergine) - Terminals auf einer Leinwand im Browser, mit Workflows, deren Schritte auf die Freigabe des Besitzers warten können, einer Aufgabenwarteschlange und Entwürfen, die vor der Nutzung geprüft werden. *(Wird von den Betreibern dieser Liste gepflegt.)*

<a id="principles-and-guides"></a>
## Prinzipien und Leitfäden

- [Effektive Agenten bauen](https://www.anthropic.com/engineering/building-effective-agents) - Anthropics Muster für Workflows und Agenten, von Prompt-Verkettung bis Orchestrator und Worker.
- [Best Practices für Claude Code](https://www.anthropic.com/engineering/claude-code-best-practices) - Erkunden, planen, programmieren und committen, mit Prüfpunkten, an denen ein Mensch eingreifen kann.
- [12-Factor Agents](https://github.com/humanlayer/12-factor-agents) - Prinzipien für Agenten, die zuverlässig genug für den Produktivbetrieb sind, einschließlich Menschen per Tool-Aufruf zu kontaktieren.

<a id="instruction-files-and-standards"></a>
## Anweisungsdateien und Standards

- [AGENTS.md](https://agents.md) - Eine einfache Markdown-Datei im Repository, die jedem Coding-Agenten sagt, wie man baut, testet und die Konventionen einhält.
- [Model Context Protocol](https://modelcontextprotocol.io) - Das offene Protokoll, um Agenten Tools und Kontext zu geben, samt seiner [Spezifikation](https://github.com/modelcontextprotocol/modelcontextprotocol).
- [Agent Skills](https://github.com/anthropics/skills) - Ordner mit Anweisungen und Skripten, die ein Agent lädt, wenn eine Aufgabe sie braucht.
- [Claude Code hooks](https://docs.claude.com/en/docs/claude-code/hooks) - Befehle, die an festen Punkten eines Agentenzugs laufen – für Prüfungen, die nicht vom Gedächtnis des Modells abhängen sollen.

<a id="planning-and-spec-driven-development"></a>
## Planung und spezifikationsgetriebene Entwicklung

- [Spec Kit](https://github.com/github/spec-kit) - GitHubs Toolkit, um Spezifikation, Plan und Aufgaben zu schreiben, bevor ein Agent Code schreibt.
- [OpenSpec](https://github.com/Fission-AI/OpenSpec) - Spezifikationsgetriebene Entwicklung, bei der jede Änderung als Dateien im Repository vorgeschlagen, geprüft und archiviert wird.
- [BMAD Method](https://github.com/bmad-code-org/BMAD-METHOD) - Agile Rollen, gespielt von Agenten – von Analyst und Architekt bis Entwickler und QA.
- [Agent OS](https://github.com/buildermethods/agent-os) - Schreibt die Standards und Spezifikationen einer Codebasis in Dateien, nach denen Agenten arbeiten.
- [Superpowers](https://github.com/obra/superpowers) - Eine Skill-Bibliothek, die einen Agenten durch Brainstorming, Planung, testgetriebene Entwicklung und Review führt.

<a id="task-tracking-for-agents"></a>
## Aufgabenverwaltung für Agenten

- [Task Master](https://github.com/eyaltoledano/claude-task-master) - Macht aus einem Produktdokument abhängige Aufgaben, die ein Agent nacheinander abarbeitet.
- [Beads](https://github.com/gastownhall/beads) - Ein Issue-Tracker im Repository, gemacht für Agenten, die Arbeit anlegen, übernehmen und abschließen.
- [Backlog.md](https://github.com/MrLesk/Backlog.md) - Ein Markdown-Aufgabenboard in Git, das Menschen und Agenten gemeinsam nutzen.

<a id="reusable-prompts-skills-and-subagents"></a>
## Wiederverwendbare Prompts, Skills und Subagenten

- [Awesome Copilot](https://github.com/github/awesome-copilot) - Anweisungen, Prompts, Agenten und Skills der Community für GitHub Copilot.
- [Awesome CursorRules](https://github.com/PatrickJS/awesome-cursorrules) - Regeldateien für Cursor, sortiert nach Sprache und Framework.
- [Agents by wshobson](https://github.com/wshobson/agents) - Plugins, Subagenten und Befehle, einmal in Markdown geschrieben und für mehrere Coding-Agenten erzeugt.
- [Awesome Claude Code Subagents](https://github.com/VoltAgent/awesome-claude-code-subagents) - Mehr als hundert spezialisierte Subagenten-Definitionen.
- [Claude Cookbooks](https://github.com/anthropics/claude-cookbooks) - Notebooks mit Mustern, darunter Agenten-Workflows und Tool-Nutzung.

<a id="review-and-approval"></a>
## Prüfung und Freigabe

- [HumanLayer](https://github.com/humanlayer/humanlayer) - Workflows für Coding-Agenten bei schwierigen Problemen, mit Recherche-, Plan- und Umsetzungsschritten, die ein Mensch prüft.
- [PR-Agent](https://github.com/The-PR-Agent/pr-agent) - Ein Open-Source-Reviewer, der Pull Requests kommentiert – ein zweiter Durchgang neben dem menschlichen Review.
- [Claude Code Security Review](https://github.com/anthropics/claude-code-security-review) - Eine GitHub Action, die jede Änderung auf Sicherheitsprobleme prüft.

<a id="running-agents-side-by-side"></a>
## Agenten nebeneinander ausführen

- [Claude Squad](https://github.com/smtg-ai/claude-squad) - Mehrere Terminal-Agenten gleichzeitig, jeder in seinem eigenen Git-Worktree, gesteuert aus einem Terminal.
- [Container Use](https://github.com/dagger/container-use) - Ein Container und ein Branch pro Agent, damit mehrere am selben Projekt arbeiten können, ohne sich ins Gehege zu kommen.
- [Crystal](https://github.com/stravu/crystal) - Eine Desktop-App für parallele Agentensitzungen in Worktrees, um Ansätze zu vergleichen (jetzt Nimbalyst).
- [Ruflo](https://github.com/ruvnet/ruflo) - Koordiniert Schwärme von Agenten mit gemeinsamem Gedächtnis rund um Claude Code und andere Agenten.

<a id="agents-in-ci"></a>
## Agenten in CI

- [Claude Code Action](https://github.com/anthropics/claude-code-action) - Führt Claude Code aus Issues und Pull Requests in GitHub Actions aus.
- [OpenHands](https://github.com/OpenHands/OpenHands) - Eine offene Plattform für Coding-Agenten, lokal, in der Cloud oder headless in CI.
- [SWE-agent](https://github.com/SWE-agent/SWE-agent) - Nimmt ein GitHub-Issue und versucht es zu beheben, mit dem Sprachmodell deiner Wahl.

<a id="frameworks-with-a-person-in-the-loop"></a>
## Frameworks mit einem Menschen im Ablauf

- [LangGraph](https://github.com/langchain-ai/langgraph) - Agenten als Graphen, die [für einen Menschen pausieren](https://langchain-ai.github.io/langgraph/concepts/human_in_the_loop/) und aus gespeichertem Zustand weiterlaufen können.
- [OpenAI Agents SDK](https://github.com/openai/openai-agents-python) - Ein schlankes Framework für Multi-Agenten-Workflows mit Übergaben und Leitplanken.
- [CrewAI](https://github.com/crewAIInc/crewAI) - Orchestriert Agenten mit Rollen, deren Aufgaben einen Menschen um Eingaben bitten können.

<a id="related-lists"></a>
## Verwandte Listen

- [Awesome Claude Code](https://github.com/hesreallyhim/awesome-claude-code) - Skills, Hooks, Befehle und Tools für Claude Code.

<a id="contributing"></a>
## Mitwirken

Beiträge sind willkommen. Lies zuerst die [Beitragsrichtlinien](contributing.md) .
