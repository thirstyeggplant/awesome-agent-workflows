# Awesome Agent Workflows [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

<div dir="rtl">


> طرق قابلة للتكرار للعمل مع وكلاء البرمجة بالذكاء الاصطناعي: خطط ومواصفات، وطوابير مهام، وأوامر ومهارات قابلة لإعادة الاستخدام، ونقاط مراجعة، وخطوات تنتظر إنسانًا.

تتناول هذه القائمة العمل المحيط بالوكيل لا الوكيل نفسه: كيف تُكتب المهمة وتُقسَّم وتُسلَّم وتُراجَع وتُعتمد. العناصر مفتوحة المصدر أو متاحة للقراءة مجانًا ما لم يُذكر غير ذلك.

<!-- lang-bar -->
**🔗 الموقع: [https://thirstyeggplant.github.io/awesome-agent-workflows/ar/](https://thirstyeggplant.github.io/awesome-agent-workflows/ar/)**

🌐 [English](readme.md) · [简体中文](readme.zh-CN.md) · [Español](readme.es.md) · [日本語](readme.ja.md) · [한국어](readme.ko.md) · [Português (BR)](readme.pt-BR.md) · [Français](readme.fr.md) · [Deutsch](readme.de.md) · [हिन्दी](readme.hi.md) · [বাংলা](readme.bn.md) · [Bahasa Indonesia](readme.id.md) · **العربية**
<!-- /lang-bar -->

<sub>هذه ترجمة للنسخة الإنجليزية. أُبقيت أسماء الأدوات والمواقع بلغتها الأصلية.</sub>

<a id="contents"></a>
## المحتويات

- [مميّز](#featured)
- [مبادئ وأدلة](#principles-and-guides)
- [ملفات التعليمات والمعايير](#instruction-files-and-standards)
- [التخطيط والتطوير القائم على المواصفات](#planning-and-spec-driven-development)
- [تتبّع المهام للوكلاء](#task-tracking-for-agents)
- [أوامر ومهارات ووكلاء فرعيون قابلة لإعادة الاستخدام](#reusable-prompts-skills-and-subagents)
- [المراجعة والاعتماد](#review-and-approval)
- [تشغيل الوكلاء جنبًا إلى جنب](#running-agents-side-by-side)
- [الوكلاء في التكامل المستمر](#agents-in-ci)
- [أطر عمل يشارك فيها إنسان](#frameworks-with-a-person-in-the-loop)
- [قوائم ذات صلة](#related-lists)

<a id="featured"></a>
## مميّز

- [Aubergine](https://github.com/thirstyeggplant/aubergine) - طرفيات على لوحة داخل المتصفح، مع مسارات عمل يمكن لخطواتها انتظار موافقة المالك، وطابور مهام، ومسودات تُراجَع قبل الاستخدام. *(يطوّره القائمون على هذه القائمة.)*

<a id="principles-and-guides"></a>
## مبادئ وأدلة

- [بناء وكلاء فعّالين](https://www.anthropic.com/engineering/building-effective-agents) - أنماط Anthropic لمسارات العمل والوكلاء، من تسلسل الأوامر إلى المنسّق والعمّال.
- [أفضل ممارسات Claude Code](https://www.anthropic.com/engineering/claude-code-best-practices) - استكشف وخطّط واكتب الشيفرة ثم نفّذ commit، مع نقاط تحقق يمكن لإنسان التدخل فيها.
- [12-Factor Agents](https://github.com/humanlayer/12-factor-agents) - مبادئ لوكلاء موثوقين بما يكفي للإنتاج، منها التواصل مع البشر عبر استدعاء أداة.

<a id="instruction-files-and-standards"></a>
## ملفات التعليمات والمعايير

- [AGENTS.md](https://agents.md) - ملف Markdown بسيط في المستودع يخبر أي وكيل برمجة بكيفية البناء والاختبار واتباع أعراف المشروع.
- [Model Context Protocol](https://modelcontextprotocol.io) - البروتوكول المفتوح لتزويد الوكلاء بالأدوات والسياق، مع [المواصفة](https://github.com/modelcontextprotocol/modelcontextprotocol).
- [Agent Skills](https://github.com/anthropics/skills) - مجلدات من التعليمات والسكربتات يحمّلها الوكيل عندما تتطلبها المهمة.
- [Claude Code hooks](https://docs.claude.com/en/docs/claude-code/hooks) - أوامر تعمل في نقاط ثابتة من دور الوكيل، لفحوص لا ينبغي أن تعتمد على تذكّر النموذج.

<a id="planning-and-spec-driven-development"></a>
## التخطيط والتطوير القائم على المواصفات

- [Spec Kit](https://github.com/github/spec-kit) - أدوات GitHub لكتابة مواصفة وخطة ومهام قبل أن يكتب الوكيل الشيفرة.
- [OpenSpec](https://github.com/Fission-AI/OpenSpec) - تطوير قائم على المواصفات، يُقترح فيه كل تغيير ويُراجَع ويُؤرشف كملفات في المستودع.
- [BMAD Method](https://github.com/bmad-code-org/BMAD-METHOD) - أدوار رشيقة يؤديها الوكلاء، من المحلل والمعماري إلى المطوّر ومختبر الجودة.
- [Agent OS](https://github.com/buildermethods/agent-os) - يدوّن معايير قاعدة الشيفرة ومواصفاتها في ملفات يعمل الوكلاء وفقها.
- [Superpowers](https://github.com/obra/superpowers) - مكتبة مهارات ترشد الوكيل عبر العصف الذهني والتخطيط والتطوير المقاد بالاختبارات والمراجعة.

<a id="task-tracking-for-agents"></a>
## تتبّع المهام للوكلاء

- [Task Master](https://github.com/eyaltoledano/claude-task-master) - يحوّل وثيقة المنتج إلى مهام مترابطة ينجزها الوكيل واحدة تلو الأخرى.
- [Beads](https://github.com/gastownhall/beads) - متتبّع مشكلات محفوظ في المستودع، مصمم ليُنشئ الوكلاء العمل ويتولّوه ويغلقوه.
- [Backlog.md](https://github.com/MrLesk/Backlog.md) - لوحة مهام بصيغة Markdown داخل Git يتشاركها البشر والوكلاء.

<a id="reusable-prompts-skills-and-subagents"></a>
## أوامر ومهارات ووكلاء فرعيون قابلة لإعادة الاستخدام

- [Awesome Copilot](https://github.com/github/awesome-copilot) - تعليمات وأوامر ووكلاء ومهارات من المجتمع لـ GitHub Copilot.
- [Awesome CursorRules](https://github.com/PatrickJS/awesome-cursorrules) - ملفات قواعد لـ Cursor مرتبة حسب اللغة وإطار العمل.
- [Agents by wshobson](https://github.com/wshobson/agents) - إضافات ووكلاء فرعيون وأوامر تُكتب مرة واحدة بـ Markdown وتُولَّد لعدة وكلاء برمجة.
- [Awesome Claude Code Subagents](https://github.com/VoltAgent/awesome-claude-code-subagents) - أكثر من مئة تعريف لوكلاء فرعيين متخصصين.
- [Claude Cookbooks](https://github.com/anthropics/claude-cookbooks) - دفاتر أنماط، تشمل مسارات عمل الوكلاء واستخدام الأدوات.

<a id="review-and-approval"></a>
## المراجعة والاعتماد

- [HumanLayer](https://github.com/humanlayer/humanlayer) - مسارات عمل لوكلاء البرمجة في المشكلات الصعبة، بخطوات بحث وتخطيط وتنفيذ يراجعها إنسان.
- [PR-Agent](https://github.com/The-PR-Agent/pr-agent) - مراجِع مفتوح المصدر يعلّق على طلبات الدمج، كفحص ثانٍ بجانب مراجعة الإنسان.
- [Claude Code Security Review](https://github.com/anthropics/claude-code-security-review) - إجراء GitHub يراجع كل تغيير بحثًا عن مشكلات أمنية.

<a id="running-agents-side-by-side"></a>
## تشغيل الوكلاء جنبًا إلى جنب

- [Claude Squad](https://github.com/smtg-ai/claude-squad) - عدة وكلاء طرفية في آن واحد، لكلٍّ منهم worktree خاص في Git، تُدار من طرفية واحدة.
- [Container Use](https://github.com/dagger/container-use) - حاوية وفرع لكل وكيل، ليعمل عدة وكلاء على مشروع واحد دون تصادم.
- [Crystal](https://github.com/stravu/crystal) - تطبيق سطح مكتب لجلسات وكلاء متوازية في worktrees لمقارنة الأساليب (اسمه الآن Nimbalyst).
- [Ruflo](https://github.com/ruvnet/ruflo) - ينسّق أسرابًا من الوكلاء بذاكرة مشتركة حول Claude Code ووكلاء آخرين.

<a id="agents-in-ci"></a>
## الوكلاء في التكامل المستمر

- [Claude Code Action](https://github.com/anthropics/claude-code-action) - يشغّل Claude Code من المشكلات وطلبات الدمج في GitHub Actions.
- [OpenHands](https://github.com/OpenHands/OpenHands) - منصة مفتوحة لوكلاء البرمجة تعمل محليًا أو في السحابة أو دون واجهة في التكامل المستمر.
- [SWE-agent](https://github.com/SWE-agent/SWE-agent) - يأخذ مشكلة من GitHub ويحاول إصلاحها بنموذج اللغة الذي تختاره.

<a id="frameworks-with-a-person-in-the-loop"></a>
## أطر عمل يشارك فيها إنسان

- [LangGraph](https://github.com/langchain-ai/langgraph) - وكلاء على شكل رسوم بيانية يمكنها أن [تتوقف مؤقتًا لإنسان](https://langchain-ai.github.io/langgraph/concepts/human_in_the_loop/) ثم تستأنف من حالة محفوظة.
- [OpenAI Agents SDK](https://github.com/openai/openai-agents-python) - إطار عمل صغير لمسارات عمل متعددة الوكلاء مع تسليم المهام وضوابط الحماية.
- [CrewAI](https://github.com/crewAIInc/crewAI) - ينسّق وكلاء يؤدون أدوارًا، بمهام يمكنها طلب مدخلات من إنسان.

<a id="related-lists"></a>
## قوائم ذات صلة

- [Awesome Claude Code](https://github.com/hesreallyhim/awesome-claude-code) - مهارات وخطافات وأوامر وأدوات لـ Claude Code.

<a id="contributing"></a>
## المساهمة

المساهمات مرحّب بها. اقرأ أولًا [إرشادات المساهمة](contributing.md) .


</div>
