# Awesome Agent Workflows [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> Repeatable ways of working with AI coding agents: plans and specs, task queues, reusable prompts and skills, review checkpoints, and steps that wait for a person.

This list is about the work around an agent rather than the agent itself: how a task is written down, broken up, handed over, checked and approved. Entries are open source or freely readable unless marked otherwise.

## Contents

- [Principles and guides](#principles-and-guides)
- [Instruction files and standards](#instruction-files-and-standards)
- [Planning and spec-driven development](#planning-and-spec-driven-development)
- [Task tracking for agents](#task-tracking-for-agents)
- [Reusable prompts, skills and subagents](#reusable-prompts-skills-and-subagents)
- [Review and approval](#review-and-approval)
- [Running agents side by side](#running-agents-side-by-side)
- [Agents in CI](#agents-in-ci)
- [Frameworks with a person in the loop](#frameworks-with-a-person-in-the-loop)
- [Related lists](#related-lists)

## Principles and guides

- [Building effective agents](https://www.anthropic.com/engineering/building-effective-agents) - Anthropic's patterns for workflows and agents, from prompt chaining to orchestrator and workers.
- [Claude Code best practices](https://www.anthropic.com/engineering/claude-code-best-practices) - Explore, plan, code and commit, with checkpoints a person can step into.
- [12-Factor Agents](https://github.com/humanlayer/12-factor-agents) - Principles for agents reliable enough for production, including contacting people as a tool call.

## Instruction files and standards

- [AGENTS.md](https://agents.md) - A plain Markdown file in a repository that tells any coding agent how to build, test and follow its conventions.
- [Model Context Protocol](https://modelcontextprotocol.io) - The open protocol for giving agents tools and context, with its [specification](https://github.com/modelcontextprotocol/modelcontextprotocol).
- [Agent Skills](https://github.com/anthropics/skills) - Folders of instructions and scripts that an agent loads when a task calls for them.
- [Claude Code hooks](https://docs.claude.com/en/docs/claude-code/hooks) - Commands that run at fixed points of an agent's turn, for checks that should not depend on the model remembering.

## Planning and spec-driven development

- [Spec Kit](https://github.com/github/spec-kit) - GitHub's toolkit for writing a specification, a plan and tasks before an agent writes code.
- [OpenSpec](https://github.com/Fission-AI/OpenSpec) - Spec-driven development where each change is proposed, reviewed and archived as files in the repository.
- [BMAD Method](https://github.com/bmad-code-org/BMAD-METHOD) - Agile roles played by agents, from analyst and architect to developer and QA.
- [Agent OS](https://github.com/buildermethods/agent-os) - Writes a codebase's standards and specs into files agents work from.
- [Superpowers](https://github.com/obra/superpowers) - A skills library that walks an agent through brainstorming, planning, test-driven development and review.

## Task tracking for agents

- [Task Master](https://github.com/eyaltoledano/claude-task-master) - Turns a product document into dependent tasks that an agent works through one at a time.
- [Beads](https://github.com/gastownhall/beads) - An issue tracker kept in the repository, made for agents to file, pick up and close work.
- [Backlog.md](https://github.com/MrLesk/Backlog.md) - A Markdown task board in Git that people and agents share.

## Reusable prompts, skills and subagents

- [Awesome Copilot](https://github.com/github/awesome-copilot) - Community instructions, prompts, agents and skills for GitHub Copilot.
- [Awesome CursorRules](https://github.com/PatrickJS/awesome-cursorrules) - Rule files for Cursor, sorted by language and framework.
- [Agents by wshobson](https://github.com/wshobson/agents) - Plugins, subagents and commands written once in Markdown and generated for several coding agents.
- [Awesome Claude Code Subagents](https://github.com/VoltAgent/awesome-claude-code-subagents) - More than a hundred specialised subagent definitions.
- [Claude Cookbooks](https://github.com/anthropics/claude-cookbooks) - Notebooks of patterns, including agent workflows and tool use.

## Review and approval

- [HumanLayer](https://github.com/humanlayer/humanlayer) - Workflows for coding agents on hard problems, with research, plan and implement steps a person reviews.
- [PR-Agent](https://github.com/The-PR-Agent/pr-agent) - An open source reviewer that comments on pull requests, a second pass beside a person's review.
- [Claude Code Security Review](https://github.com/anthropics/claude-code-security-review) - A GitHub Action that reviews each change for security problems.

## Running agents side by side

- [Aubergine](https://github.com/thirstyeggplant/aubergine) - Terminals on a canvas in the browser, with workflows whose steps can wait for the owner's approval, a task queue and drafts reviewed before use. *(Maintained by the owners of this list.)*
- [Claude Squad](https://github.com/smtg-ai/claude-squad) - Several terminal agents at once, each in its own Git worktree, managed from one terminal.
- [Container Use](https://github.com/dagger/container-use) - A container and a branch per agent, so several can work on one project without colliding.
- [Crystal](https://github.com/stravu/crystal) - A desktop app for parallel agent sessions in worktrees, to compare approaches (now Nimbalyst).
- [Ruflo](https://github.com/ruvnet/ruflo) - Coordinates swarms of agents with shared memory around Claude Code and other agents.

## Agents in CI

- [Claude Code Action](https://github.com/anthropics/claude-code-action) - Runs Claude Code from issues and pull requests in GitHub Actions.
- [OpenHands](https://github.com/OpenHands/OpenHands) - An open platform for coding agents that runs locally, in the cloud or headless in CI.
- [SWE-agent](https://github.com/SWE-agent/SWE-agent) - Takes a GitHub issue and tries to fix it, with the language model of your choice.

## Frameworks with a person in the loop

- [LangGraph](https://github.com/langchain-ai/langgraph) - Agents as graphs that can [pause for a person](https://langchain-ai.github.io/langgraph/concepts/human_in_the_loop/) and resume from saved state.
- [OpenAI Agents SDK](https://github.com/openai/openai-agents-python) - A small framework for multi-agent workflows with handoffs and guardrails.
- [CrewAI](https://github.com/crewAIInc/crewAI) - Orchestrates agents that play roles, with tasks that can ask a person for input.

## Related lists

- [Awesome Claude Code](https://github.com/hesreallyhim/awesome-claude-code) - Skills, hooks, commands and tools for Claude Code.

## Contributing

Contributions are welcome. Read the [contribution guidelines](contributing.md) first.
