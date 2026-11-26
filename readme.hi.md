# Awesome Agent Workflows [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> AI कोडिंग एजेंटों के साथ काम करने के दोहराए जा सकने वाले तरीके: योजना और स्पेक, टास्क कतारें, दोबारा इस्तेमाल होने वाले प्रॉम्प्ट और स्किल, समीक्षा पड़ाव और ऐसे चरण जो किसी व्यक्ति का इंतज़ार करते हैं।

यह सूची एजेंट के बारे में कम और उसके आसपास के काम के बारे में ज़्यादा है: कोई काम कैसे लिखा जाता है, बाँटा जाता है, सौंपा जाता है, जाँचा जाता है और मंज़ूर होता है। जब तक अलग से न लिखा हो, प्रविष्टियाँ ओपन सोर्स हैं या मुफ़्त में पढ़ी जा सकती हैं।

<!-- lang-bar -->
**🔗 वेबसाइट: [https://thirstyeggplant.github.io/awesome-agent-workflows/hi/](https://thirstyeggplant.github.io/awesome-agent-workflows/hi/)**

🌐 [English](readme.md) · [简体中文](readme.zh-CN.md) · [Español](readme.es.md) · [日本語](readme.ja.md) · [한국어](readme.ko.md) · [Português (BR)](readme.pt-BR.md) · [Français](readme.fr.md) · [Deutsch](readme.de.md) · **हिन्दी** · [বাংলা](readme.bn.md) · [Bahasa Indonesia](readme.id.md) · [العربية](readme.ar.md)
<!-- /lang-bar -->

<sub>यह अंग्रेज़ी संस्करण का अनुवाद है। टूल और वेबसाइटों के नाम मूल रूप में रखे गए हैं।</sub>

<a id="contents"></a>
## विषय-सूची

- [विशेष](#featured)
- [सिद्धांत और गाइड](#principles-and-guides)
- [निर्देश फ़ाइलें और मानक](#instruction-files-and-standards)
- [योजना और स्पेक-आधारित डेवलपमेंट](#planning-and-spec-driven-development)
- [एजेंटों के लिए टास्क ट्रैकिंग](#task-tracking-for-agents)
- [दोबारा उपयोग होने वाले प्रॉम्प्ट, स्किल और सबएजेंट](#reusable-prompts-skills-and-subagents)
- [समीक्षा और मंज़ूरी](#review-and-approval)
- [एजेंटों को साथ-साथ चलाना](#running-agents-side-by-side)
- [CI में एजेंट](#agents-in-ci)
- [जिन फ़्रेमवर्क में इंसान शामिल रहता है](#frameworks-with-a-person-in-the-loop)
- [संबंधित सूचियाँ](#related-lists)

<a id="featured"></a>
## विशेष

- [Aubergine](https://github.com/thirstyeggplant/aubergine) - ब्राउज़र में कैनवास पर टर्मिनल, ऐसे वर्कफ़्लो के साथ जिनके चरण मालिक की मंज़ूरी का इंतज़ार कर सकते हैं, एक टास्क कतार और इस्तेमाल से पहले जाँचे जाने वाले ड्राफ़्ट। *(इस सूची के मालिकों द्वारा बनाया गया।)*

<a id="principles-and-guides"></a>
## सिद्धांत और गाइड

- [असरदार एजेंट बनाना](https://www.anthropic.com/engineering/building-effective-agents) - वर्कफ़्लो और एजेंटों के लिए Anthropic के पैटर्न, प्रॉम्प्ट चेनिंग से लेकर ऑर्केस्ट्रेटर और वर्कर तक।
- [Claude Code के सर्वोत्तम तरीके](https://www.anthropic.com/engineering/claude-code-best-practices) - खोजें, योजना बनाएँ, कोड करें और commit करें, ऐसे पड़ावों के साथ जहाँ इंसान बीच में आ सके।
- [12-Factor Agents](https://github.com/humanlayer/12-factor-agents) - प्रोडक्शन लायक़ भरोसेमंद एजेंटों के सिद्धांत, जिनमें लोगों से संपर्क को टूल कॉल की तरह करना भी शामिल है।

<a id="instruction-files-and-standards"></a>
## निर्देश फ़ाइलें और मानक

- [AGENTS.md](https://agents.md) - रिपॉज़िटरी में एक सादी Markdown फ़ाइल, जो किसी भी कोडिंग एजेंट को बताती है कि बिल्ड, टेस्ट कैसे करें और नियमों का पालन कैसे करें।
- [Model Context Protocol](https://modelcontextprotocol.io) - एजेंटों को टूल और संदर्भ देने का खुला प्रोटोकॉल, साथ में इसका [विनिर्देश](https://github.com/modelcontextprotocol/modelcontextprotocol).
- [Agent Skills](https://github.com/anthropics/skills) - निर्देशों और स्क्रिप्ट के फ़ोल्डर, जिन्हें एजेंट ज़रूरत पड़ने पर लोड करता है।
- [Claude Code hooks](https://docs.claude.com/en/docs/claude-code/hooks) - एजेंट की बारी के तय बिंदुओं पर चलने वाले कमांड, उन जाँचों के लिए जो मॉडल की याददाश्त पर निर्भर नहीं होनी चाहिए।

<a id="planning-and-spec-driven-development"></a>
## योजना और स्पेक-आधारित डेवलपमेंट

- [Spec Kit](https://github.com/github/spec-kit) - एजेंट के कोड लिखने से पहले स्पेक, योजना और टास्क लिखने के लिए GitHub का टूलकिट।
- [OpenSpec](https://github.com/Fission-AI/OpenSpec) - स्पेक-आधारित डेवलपमेंट, जिसमें हर बदलाव रिपॉज़िटरी में फ़ाइलों के रूप में प्रस्तावित, समीक्षित और संग्रहित होता है।
- [BMAD Method](https://github.com/bmad-code-org/BMAD-METHOD) - एजेंटों द्वारा निभाई जाने वाली एजाइल भूमिकाएँ, एनालिस्ट और आर्किटेक्ट से लेकर डेवलपर और QA तक।
- [Agent OS](https://github.com/buildermethods/agent-os) - कोडबेस के मानकों और स्पेक को ऐसी फ़ाइलों में लिखता है जिनसे एजेंट काम करते हैं।
- [Superpowers](https://github.com/obra/superpowers) - एक स्किल लाइब्रेरी जो एजेंट को विचार-मंथन, योजना, टेस्ट-ड्रिवन डेवलपमेंट और समीक्षा से गुज़ारती है।

<a id="task-tracking-for-agents"></a>
## एजेंटों के लिए टास्क ट्रैकिंग

- [Task Master](https://github.com/eyaltoledano/claude-task-master) - प्रोडक्ट दस्तावेज़ को आपस में जुड़े टास्क में बदलता है, जिन्हें एजेंट एक-एक करके पूरा करता है।
- [Beads](https://github.com/gastownhall/beads) - रिपॉज़िटरी में रखा इश्यू ट्रैकर, जो एजेंटों के लिए काम दर्ज करने, उठाने और बंद करने के लिए बना है।
- [Backlog.md](https://github.com/MrLesk/Backlog.md) - Git में एक Markdown टास्क बोर्ड, जिसे लोग और एजेंट साझा करते हैं।

<a id="reusable-prompts-skills-and-subagents"></a>
## दोबारा उपयोग होने वाले प्रॉम्प्ट, स्किल और सबएजेंट

- [Awesome Copilot](https://github.com/github/awesome-copilot) - GitHub Copilot के लिए समुदाय के निर्देश, प्रॉम्प्ट, एजेंट और स्किल।
- [Awesome CursorRules](https://github.com/PatrickJS/awesome-cursorrules) - Cursor के लिए नियम फ़ाइलें, भाषा और फ़्रेमवर्क के अनुसार।
- [Agents by wshobson](https://github.com/wshobson/agents) - प्लगइन, सबएजेंट और कमांड जो एक बार Markdown में लिखे जाते हैं और कई कोडिंग एजेंटों के लिए बनाए जाते हैं।
- [Awesome Claude Code Subagents](https://github.com/VoltAgent/awesome-claude-code-subagents) - सौ से ज़्यादा विशेष सबएजेंट परिभाषाएँ।
- [Claude Cookbooks](https://github.com/anthropics/claude-cookbooks) - पैटर्न वाली नोटबुक, जिनमें एजेंट वर्कफ़्लो और टूल का उपयोग शामिल है।

<a id="review-and-approval"></a>
## समीक्षा और मंज़ूरी

- [HumanLayer](https://github.com/humanlayer/humanlayer) - कठिन समस्याओं पर कोडिंग एजेंटों के वर्कफ़्लो, जिनमें शोध, योजना और कार्यान्वयन के चरणों की समीक्षा इंसान करता है।
- [PR-Agent](https://github.com/The-PR-Agent/pr-agent) - एक ओपन सोर्स रिव्यूअर जो pull request पर टिप्पणी करता है, इंसानी समीक्षा के साथ दूसरी जाँच।
- [Claude Code Security Review](https://github.com/anthropics/claude-code-security-review) - एक GitHub Action जो हर बदलाव में सुरक्षा समस्याएँ जाँचता है।

<a id="running-agents-side-by-side"></a>
## एजेंटों को साथ-साथ चलाना

- [Claude Squad](https://github.com/smtg-ai/claude-squad) - एक साथ कई टर्मिनल एजेंट, हर एक अपने Git worktree में, एक ही टर्मिनल से संभाले जाते हैं।
- [Container Use](https://github.com/dagger/container-use) - हर एजेंट के लिए एक कंटेनर और एक ब्रांच, ताकि कई एजेंट बिना टकराए एक प्रोजेक्ट पर काम करें।
- [Crystal](https://github.com/stravu/crystal) - worktree में समानांतर एजेंट सत्रों के लिए डेस्कटॉप ऐप, तरीकों की तुलना के लिए (अब Nimbalyst)।
- [Ruflo](https://github.com/ruvnet/ruflo) - Claude Code और दूसरे एजेंटों के इर्द-गिर्द साझा मेमोरी वाले एजेंट झुंडों का तालमेल करता है।

<a id="agents-in-ci"></a>
## CI में एजेंट

- [Claude Code Action](https://github.com/anthropics/claude-code-action) - GitHub Actions में issue और pull request से Claude Code चलाता है।
- [OpenHands](https://github.com/OpenHands/OpenHands) - कोडिंग एजेंटों के लिए खुला प्लेटफ़ॉर्म जो लोकल, क्लाउड में या CI में बिना इंटरफ़ेस के चलता है।
- [SWE-agent](https://github.com/SWE-agent/SWE-agent) - GitHub issue लेकर आपके चुने हुए भाषा मॉडल से उसे ठीक करने की कोशिश करता है।

<a id="frameworks-with-a-person-in-the-loop"></a>
## जिन फ़्रेमवर्क में इंसान शामिल रहता है

- [LangGraph](https://github.com/langchain-ai/langgraph) - ग्राफ़ के रूप में एजेंट, जो [किसी व्यक्ति के लिए रुक](https://langchain-ai.github.io/langgraph/concepts/human_in_the_loop/) सकते हैं और सहेजी गई स्थिति से फिर शुरू हो सकते हैं।
- [OpenAI Agents SDK](https://github.com/openai/openai-agents-python) - हैंडऑफ़ और गार्डरेल वाले मल्टी-एजेंट वर्कफ़्लो के लिए छोटा फ़्रेमवर्क।
- [CrewAI](https://github.com/crewAIInc/crewAI) - भूमिकाएँ निभाने वाले एजेंटों का संचालन करता है, ऐसे टास्क के साथ जो इंसान से इनपुट माँग सकते हैं।

<a id="related-lists"></a>
## संबंधित सूचियाँ

- [Awesome Claude Code](https://github.com/hesreallyhim/awesome-claude-code) - Claude Code के लिए स्किल, हुक, कमांड और टूल।

<a id="contributing"></a>
## योगदान

योगदान का स्वागत है। पहले [योगदान दिशानिर्देश](contributing.md) पढ़ें।
