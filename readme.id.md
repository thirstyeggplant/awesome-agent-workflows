# Awesome Agent Workflows [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> Cara kerja yang bisa diulang bersama agen coding AI: rencana dan spesifikasi, antrean tugas, prompt dan skill yang bisa dipakai ulang, titik tinjauan, dan langkah yang menunggu manusia.

Daftar ini membahas pekerjaan di sekitar agen, bukan agennya sendiri: bagaimana tugas ditulis, dipecah, diserahkan, diperiksa, dan disetujui. Entri bersifat open source atau bebas dibaca kecuali disebutkan lain.

<!-- lang-bar -->
**🔗 Situs web: [https://thirstyeggplant.github.io/awesome-agent-workflows/id/](https://thirstyeggplant.github.io/awesome-agent-workflows/id/)**

🌐 [English](readme.md) · [简体中文](readme.zh-CN.md) · [Español](readme.es.md) · [日本語](readme.ja.md) · [한국어](readme.ko.md) · [Português (BR)](readme.pt-BR.md) · [Français](readme.fr.md) · [Deutsch](readme.de.md) · [हिन्दी](readme.hi.md) · [বাংলা](readme.bn.md) · **Bahasa Indonesia** · [العربية](readme.ar.md)
<!-- /lang-bar -->

<sub>Terjemahan dari versi bahasa Inggris. Nama alat dan situs dibiarkan seperti aslinya.</sub>

<a id="contents"></a>
## Daftar isi

- [Unggulan](#featured)
- [Prinsip dan panduan](#principles-and-guides)
- [File instruksi dan standar](#instruction-files-and-standards)
- [Perencanaan dan pengembangan berbasis spesifikasi](#planning-and-spec-driven-development)
- [Pelacakan tugas untuk agen](#task-tracking-for-agents)
- [Prompt, skill, dan subagen yang bisa dipakai ulang](#reusable-prompts-skills-and-subagents)
- [Tinjauan dan persetujuan](#review-and-approval)
- [Menjalankan agen berdampingan](#running-agents-side-by-side)
- [Agen di CI](#agents-in-ci)
- [Framework dengan manusia dalam alur](#frameworks-with-a-person-in-the-loop)
- [Daftar terkait](#related-lists)

<a id="featured"></a>
## Unggulan

- [Aubergine](https://github.com/thirstyeggplant/aubergine) - Terminal di kanvas dalam browser, dengan alur kerja yang langkahnya bisa menunggu persetujuan pemilik, antrean tugas, dan draf yang ditinjau sebelum dipakai. *(Dikelola oleh pemilik daftar ini.)*

<a id="principles-and-guides"></a>
## Prinsip dan panduan

- [Membangun agen yang efektif](https://www.anthropic.com/engineering/building-effective-agents) - Pola dari Anthropic untuk alur kerja dan agen, dari rantai prompt hingga orkestrator dan pekerja.
- [Praktik terbaik Claude Code](https://www.anthropic.com/engineering/claude-code-best-practices) - Jelajahi, rencanakan, tulis kode, dan commit, dengan titik periksa tempat manusia bisa masuk.
- [12-Factor Agents](https://github.com/humanlayer/12-factor-agents) - Prinsip agar agen cukup andal untuk produksi, termasuk menghubungi manusia sebagai pemanggilan alat.

<a id="instruction-files-and-standards"></a>
## File instruksi dan standar

- [AGENTS.md](https://agents.md) - File Markdown biasa di repositori yang memberi tahu agen coding mana pun cara build, menguji, dan mengikuti konvensinya.
- [Model Context Protocol](https://modelcontextprotocol.io) - Protokol terbuka untuk memberi agen alat dan konteks, beserta [spesifikasi](https://github.com/modelcontextprotocol/modelcontextprotocol).
- [Agent Skills](https://github.com/anthropics/skills) - Folder berisi instruksi dan skrip yang dimuat agen saat tugas membutuhkannya.
- [Claude Code hooks](https://docs.claude.com/en/docs/claude-code/hooks) - Perintah yang berjalan di titik tetap giliran agen, untuk pemeriksaan yang tidak boleh bergantung pada ingatan model.

<a id="planning-and-spec-driven-development"></a>
## Perencanaan dan pengembangan berbasis spesifikasi

- [Spec Kit](https://github.com/github/spec-kit) - Toolkit GitHub untuk menulis spesifikasi, rencana, dan tugas sebelum agen menulis kode.
- [OpenSpec](https://github.com/Fission-AI/OpenSpec) - Pengembangan berbasis spesifikasi: setiap perubahan diusulkan, ditinjau, dan diarsipkan sebagai file di repositori.
- [BMAD Method](https://github.com/bmad-code-org/BMAD-METHOD) - Peran agile yang dijalankan agen, dari analis dan arsitek hingga developer dan QA.
- [Agent OS](https://github.com/buildermethods/agent-os) - Menuliskan standar dan spesifikasi codebase ke file yang menjadi acuan kerja agen.
- [Superpowers](https://github.com/obra/superpowers) - Pustaka skill yang memandu agen melalui curah gagasan, perencanaan, TDD, dan tinjauan.

<a id="task-tracking-for-agents"></a>
## Pelacakan tugas untuk agen

- [Task Master](https://github.com/eyaltoledano/claude-task-master) - Mengubah dokumen produk menjadi tugas-tugas yang saling bergantung untuk dikerjakan agen satu per satu.
- [Beads](https://github.com/gastownhall/beads) - Pelacak isu di dalam repositori, dibuat agar agen bisa membuat, mengambil, dan menutup pekerjaan.
- [Backlog.md](https://github.com/MrLesk/Backlog.md) - Papan tugas Markdown di Git yang dipakai bersama oleh manusia dan agen.

<a id="reusable-prompts-skills-and-subagents"></a>
## Prompt, skill, dan subagen yang bisa dipakai ulang

- [Awesome Copilot](https://github.com/github/awesome-copilot) - Instruksi, prompt, agen, dan skill komunitas untuk GitHub Copilot.
- [Awesome CursorRules](https://github.com/PatrickJS/awesome-cursorrules) - File aturan untuk Cursor, dikelompokkan per bahasa dan framework.
- [Agents by wshobson](https://github.com/wshobson/agents) - Plugin, subagen, dan perintah yang ditulis sekali dalam Markdown lalu dibuat untuk beberapa agen coding.
- [Awesome Claude Code Subagents](https://github.com/VoltAgent/awesome-claude-code-subagents) - Lebih dari seratus definisi subagen khusus.
- [Claude Cookbooks](https://github.com/anthropics/claude-cookbooks) - Notebook berisi pola, termasuk alur kerja agen dan penggunaan alat.

<a id="review-and-approval"></a>
## Tinjauan dan persetujuan

- [HumanLayer](https://github.com/humanlayer/humanlayer) - Alur kerja untuk agen coding pada masalah sulit, dengan langkah riset, rencana, dan implementasi yang ditinjau manusia.
- [PR-Agent](https://github.com/The-PR-Agent/pr-agent) - Peninjau open source yang mengomentari pull request, sebagai pemeriksaan kedua di samping tinjauan manusia.
- [Claude Code Security Review](https://github.com/anthropics/claude-code-security-review) - GitHub Action yang meninjau setiap perubahan untuk mencari masalah keamanan.

<a id="running-agents-side-by-side"></a>
## Menjalankan agen berdampingan

- [Claude Squad](https://github.com/smtg-ai/claude-squad) - Beberapa agen terminal sekaligus, masing-masing di Git worktree sendiri, dikelola dari satu terminal.
- [Container Use](https://github.com/dagger/container-use) - Satu kontainer dan satu branch per agen, agar beberapa agen bisa mengerjakan satu proyek tanpa bentrok.
- [Crystal](https://github.com/stravu/crystal) - Aplikasi desktop untuk sesi agen paralel di worktree, guna membandingkan pendekatan (kini Nimbalyst).
- [Ruflo](https://github.com/ruvnet/ruflo) - Mengoordinasikan kawanan agen dengan memori bersama di sekitar Claude Code dan agen lain.

<a id="agents-in-ci"></a>
## Agen di CI

- [Claude Code Action](https://github.com/anthropics/claude-code-action) - Menjalankan Claude Code dari issue dan pull request di GitHub Actions.
- [OpenHands](https://github.com/OpenHands/OpenHands) - Platform terbuka untuk agen coding yang berjalan lokal, di cloud, atau tanpa antarmuka di CI.
- [SWE-agent](https://github.com/SWE-agent/SWE-agent) - Mengambil issue GitHub dan mencoba memperbaikinya dengan model bahasa pilihan Anda.

<a id="frameworks-with-a-person-in-the-loop"></a>
## Framework dengan manusia dalam alur

- [LangGraph](https://github.com/langchain-ai/langgraph) - Agen berbentuk graf yang bisa [berhenti sejenak untuk manusia](https://langchain-ai.github.io/langgraph/concepts/human_in_the_loop/) lalu melanjutkan dari keadaan tersimpan.
- [OpenAI Agents SDK](https://github.com/openai/openai-agents-python) - Framework kecil untuk alur kerja multi-agen dengan serah terima dan pembatas.
- [CrewAI](https://github.com/crewAIInc/crewAI) - Mengatur agen yang menjalankan peran, dengan tugas yang bisa meminta masukan dari manusia.

<a id="related-lists"></a>
## Daftar terkait

- [Awesome Claude Code](https://github.com/hesreallyhim/awesome-claude-code) - Skill, hook, perintah, dan alat untuk Claude Code.

<a id="contributing"></a>
## Berkontribusi

Kontribusi sangat diterima. Baca dulu [panduan kontribusi](contributing.md) .
