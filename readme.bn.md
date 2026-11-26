# Awesome Agent Workflows [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> AI কোডিং এজেন্টের সাথে কাজ করার পুনরাবৃত্তিযোগ্য উপায়: পরিকল্পনা ও স্পেক, টাস্ক কিউ, পুনর্ব্যবহারযোগ্য প্রম্পট ও স্কিল, রিভিউ চেকপয়েন্ট এবং এমন ধাপ যা একজন মানুষের অপেক্ষায় থাকে।

এই তালিকা এজেন্ট নিয়ে নয়, বরং এজেন্টের চারপাশের কাজ নিয়ে: একটি কাজ কীভাবে লেখা হয়, ভাগ করা হয়, হস্তান্তর করা হয়, যাচাই ও অনুমোদন করা হয়। আলাদা করে উল্লেখ না থাকলে সব এন্ট্রি ওপেন সোর্স বা বিনামূল্যে পড়া যায়।

<!-- lang-bar -->
**🔗 ওয়েবসাইট: [https://thirstyeggplant.github.io/awesome-agent-workflows/bn/](https://thirstyeggplant.github.io/awesome-agent-workflows/bn/)**

🌐 [English](readme.md) · [简体中文](readme.zh-CN.md) · [Español](readme.es.md) · [日本語](readme.ja.md) · [한국어](readme.ko.md) · [Português (BR)](readme.pt-BR.md) · [Français](readme.fr.md) · [Deutsch](readme.de.md) · [हिन्दी](readme.hi.md) · **বাংলা** · [Bahasa Indonesia](readme.id.md) · [العربية](readme.ar.md)
<!-- /lang-bar -->

<sub>এটি ইংরেজি সংস্করণের অনুবাদ। টুল ও ওয়েবসাইটের নাম মূল ভাষায় রাখা হয়েছে।</sub>

<a id="contents"></a>
## সূচিপত্র

- [বিশেষ](#featured)
- [নীতি ও নির্দেশিকা](#principles-and-guides)
- [নির্দেশ ফাইল ও মানদণ্ড](#instruction-files-and-standards)
- [পরিকল্পনা ও স্পেক-ভিত্তিক ডেভেলপমেন্ট](#planning-and-spec-driven-development)
- [এজেন্টের জন্য টাস্ক ট্র্যাকিং](#task-tracking-for-agents)
- [পুনর্ব্যবহারযোগ্য প্রম্পট, স্কিল ও সাবএজেন্ট](#reusable-prompts-skills-and-subagents)
- [রিভিউ ও অনুমোদন](#review-and-approval)
- [পাশাপাশি এজেন্ট চালানো](#running-agents-side-by-side)
- [CI-তে এজেন্ট](#agents-in-ci)
- [যে ফ্রেমওয়ার্কে মানুষ যুক্ত থাকে](#frameworks-with-a-person-in-the-loop)
- [সম্পর্কিত তালিকা](#related-lists)

<a id="featured"></a>
## বিশেষ

- [Aubergine](https://github.com/thirstyeggplant/aubergine) - ব্রাউজারে ক্যানভাসের ওপর টার্মিনাল, এমন ওয়ার্কফ্লোসহ যার ধাপ মালিকের অনুমোদনের অপেক্ষা করতে পারে, একটি টাস্ক কিউ এবং ব্যবহারের আগে রিভিউ করা ড্রাফট। *(এই তালিকার মালিকদের তৈরি।)*

<a id="principles-and-guides"></a>
## নীতি ও নির্দেশিকা

- [কার্যকর এজেন্ট তৈরি](https://www.anthropic.com/engineering/building-effective-agents) - ওয়ার্কফ্লো ও এজেন্টের জন্য Anthropic-এর প্যাটার্ন, প্রম্পট চেইনিং থেকে অর্কেস্ট্রেটর ও ওয়ার্কার পর্যন্ত।
- [Claude Code-এর সেরা চর্চা](https://www.anthropic.com/engineering/claude-code-best-practices) - অনুসন্ধান, পরিকল্পনা, কোড ও commit, এমন চেকপয়েন্টসহ যেখানে মানুষ ঢুকতে পারে।
- [12-Factor Agents](https://github.com/humanlayer/12-factor-agents) - প্রোডাকশনে চালানোর মতো নির্ভরযোগ্য এজেন্টের নীতি, যার মধ্যে মানুষের সাথে যোগাযোগকে টুল কল হিসেবে ধরা অন্তর্ভুক্ত।

<a id="instruction-files-and-standards"></a>
## নির্দেশ ফাইল ও মানদণ্ড

- [AGENTS.md](https://agents.md) - রিপোজিটরিতে একটি সাধারণ Markdown ফাইল, যা যেকোনো কোডিং এজেন্টকে বিল্ড, টেস্ট ও নিয়ম মানার উপায় বলে দেয়।
- [Model Context Protocol](https://modelcontextprotocol.io) - এজেন্টদের টুল ও প্রসঙ্গ দেওয়ার উন্মুক্ত প্রোটোকল, সঙ্গে এর [স্পেসিফিকেশন](https://github.com/modelcontextprotocol/modelcontextprotocol).
- [Agent Skills](https://github.com/anthropics/skills) - নির্দেশনা ও স্ক্রিপ্টের ফোল্ডার, যা দরকার হলে এজেন্ট লোড করে।
- [Claude Code hooks](https://docs.claude.com/en/docs/claude-code/hooks) - এজেন্টের পালার নির্দিষ্ট সময়ে চলা কমান্ড, এমন যাচাইয়ের জন্য যা মডেলের মনে রাখার ওপর নির্ভর করা উচিত নয়।

<a id="planning-and-spec-driven-development"></a>
## পরিকল্পনা ও স্পেক-ভিত্তিক ডেভেলপমেন্ট

- [Spec Kit](https://github.com/github/spec-kit) - এজেন্ট কোড লেখার আগে স্পেক, পরিকল্পনা ও টাস্ক লেখার জন্য GitHub-এর টুলকিট।
- [OpenSpec](https://github.com/Fission-AI/OpenSpec) - স্পেক-ভিত্তিক ডেভেলপমেন্ট, যেখানে প্রতিটি পরিবর্তন রিপোজিটরির ফাইল হিসেবে প্রস্তাব, রিভিউ ও সংরক্ষণ করা হয়।
- [BMAD Method](https://github.com/bmad-code-org/BMAD-METHOD) - অ্যানালিস্ট ও আর্কিটেক্ট থেকে ডেভেলপার ও QA পর্যন্ত, এজেন্টদের পালন করা অ্যাজাইল ভূমিকা।
- [Agent OS](https://github.com/buildermethods/agent-os) - কোডবেসের মানদণ্ড ও স্পেক এমন ফাইলে লেখে যা দেখে এজেন্টরা কাজ করে।
- [Superpowers](https://github.com/obra/superpowers) - একটি স্কিল লাইব্রেরি যা এজেন্টকে ব্রেইনস্টর্মিং, পরিকল্পনা, টেস্ট-ড্রিভেন ডেভেলপমেন্ট ও রিভিউয়ের মধ্য দিয়ে নিয়ে যায়।

<a id="task-tracking-for-agents"></a>
## এজেন্টের জন্য টাস্ক ট্র্যাকিং

- [Task Master](https://github.com/eyaltoledano/claude-task-master) - প্রোডাক্ট ডকুমেন্টকে পরস্পর নির্ভর টাস্কে ভাগ করে, যা এজেন্ট একে একে শেষ করে।
- [Beads](https://github.com/gastownhall/beads) - রিপোজিটরিতে রাখা একটি ইস্যু ট্র্যাকার, এজেন্টদের কাজ খোলা, নেওয়া ও বন্ধ করার জন্য তৈরি।
- [Backlog.md](https://github.com/MrLesk/Backlog.md) - Git-এ একটি Markdown টাস্ক বোর্ড, যা মানুষ ও এজেন্ট মিলে ব্যবহার করে।

<a id="reusable-prompts-skills-and-subagents"></a>
## পুনর্ব্যবহারযোগ্য প্রম্পট, স্কিল ও সাবএজেন্ট

- [Awesome Copilot](https://github.com/github/awesome-copilot) - GitHub Copilot-এর জন্য কমিউনিটির নির্দেশনা, প্রম্পট, এজেন্ট ও স্কিল।
- [Awesome CursorRules](https://github.com/PatrickJS/awesome-cursorrules) - ভাষা ও ফ্রেমওয়ার্ক অনুযায়ী সাজানো Cursor-এর রুল ফাইল।
- [Agents by wshobson](https://github.com/wshobson/agents) - একবার Markdown-এ লেখা প্লাগইন, সাবএজেন্ট ও কমান্ড, যা একাধিক কোডিং এজেন্টের জন্য তৈরি হয়।
- [Awesome Claude Code Subagents](https://github.com/VoltAgent/awesome-claude-code-subagents) - শতাধিক বিশেষায়িত সাবএজেন্টের সংজ্ঞা।
- [Claude Cookbooks](https://github.com/anthropics/claude-cookbooks) - প্যাটার্নের নোটবুক, এজেন্ট ওয়ার্কফ্লো ও টুল ব্যবহারসহ।

<a id="review-and-approval"></a>
## রিভিউ ও অনুমোদন

- [HumanLayer](https://github.com/humanlayer/humanlayer) - কঠিন সমস্যায় কোডিং এজেন্টের ওয়ার্কফ্লো, যেখানে গবেষণা, পরিকল্পনা ও বাস্তবায়নের ধাপ মানুষ রিভিউ করে।
- [PR-Agent](https://github.com/The-PR-Agent/pr-agent) - একটি ওপেন সোর্স রিভিউয়ার যা pull request-এ মন্তব্য করে, মানুষের রিভিউয়ের পাশে দ্বিতীয় যাচাই।
- [Claude Code Security Review](https://github.com/anthropics/claude-code-security-review) - একটি GitHub Action যা প্রতিটি পরিবর্তনে নিরাপত্তা সমস্যা খোঁজে।

<a id="running-agents-side-by-side"></a>
## পাশাপাশি এজেন্ট চালানো

- [Claude Squad](https://github.com/smtg-ai/claude-squad) - একসাথে কয়েকটি টার্মিনাল এজেন্ট, প্রত্যেকে নিজের Git worktree-তে, একটি টার্মিনাল থেকে পরিচালিত।
- [Container Use](https://github.com/dagger/container-use) - প্রতিটি এজেন্টের জন্য একটি কন্টেইনার ও একটি ব্রাঞ্চ, যাতে একাধিক এজেন্ট সংঘর্ষ ছাড়াই এক প্রজেক্টে কাজ করতে পারে।
- [Crystal](https://github.com/stravu/crystal) - worktree-তে সমান্তরাল এজেন্ট সেশনের ডেস্কটপ অ্যাপ, পদ্ধতি তুলনার জন্য (এখন Nimbalyst)।
- [Ruflo](https://github.com/ruvnet/ruflo) - Claude Code ও অন্যান্য এজেন্ট ঘিরে শেয়ার্ড মেমরির এজেন্ট দলকে সমন্বয় করে।

<a id="agents-in-ci"></a>
## CI-তে এজেন্ট

- [Claude Code Action](https://github.com/anthropics/claude-code-action) - GitHub Actions-এ issue ও pull request থেকে Claude Code চালায়।
- [OpenHands](https://github.com/OpenHands/OpenHands) - কোডিং এজেন্টের জন্য উন্মুক্ত প্ল্যাটফর্ম, যা লোকালি, ক্লাউডে বা CI-তে ইন্টারফেস ছাড়া চলে।
- [SWE-agent](https://github.com/SWE-agent/SWE-agent) - একটি GitHub issue নিয়ে আপনার পছন্দের ভাষা মডেল দিয়ে সমাধানের চেষ্টা করে।

<a id="frameworks-with-a-person-in-the-loop"></a>
## যে ফ্রেমওয়ার্কে মানুষ যুক্ত থাকে

- [LangGraph](https://github.com/langchain-ai/langgraph) - গ্রাফ হিসেবে এজেন্ট, যা [একজন মানুষের জন্য থেমে](https://langchain-ai.github.io/langgraph/concepts/human_in_the_loop/) থাকতে পারে এবং সংরক্ষিত অবস্থা থেকে আবার চালু হতে পারে।
- [OpenAI Agents SDK](https://github.com/openai/openai-agents-python) - হ্যান্ডঅফ ও গার্ডরেলসহ মাল্টি-এজেন্ট ওয়ার্কফ্লোর ছোট ফ্রেমওয়ার্ক।
- [CrewAI](https://github.com/crewAIInc/crewAI) - ভূমিকা পালনকারী এজেন্টদের পরিচালনা করে, এমন টাস্কসহ যা মানুষের কাছে ইনপুট চাইতে পারে।

<a id="related-lists"></a>
## সম্পর্কিত তালিকা

- [Awesome Claude Code](https://github.com/hesreallyhim/awesome-claude-code) - Claude Code-এর জন্য স্কিল, হুক, কমান্ড ও টুল।

<a id="contributing"></a>
## অবদান

অবদান স্বাগত। আগে [অবদানের নির্দেশিকা](contributing.md) পড়ে নিন।
