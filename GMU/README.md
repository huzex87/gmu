# GIDAN MULKI UNIVERSE (GMU)
### Master Repository — GMU Studio

> **New to this project? Read `START_HERE.md` first.** It's a plain-language onboarding guide — what this is, where things stand, and exactly how to produce Episode 1 — written for anyone joining with zero prior context. This README is the compact technical reference; START_HERE.md is the walkthrough.

**Working Tagline:** "Power is Earned. Legacy is Chosen."

This is the canonical source-of-truth repository for the Gidan Mulki Universe franchise: a premium AI-native cinematic universe inspired by the civilizations, architecture, governance, scholarship, commerce, and cultural richness of the Sahel.

---

## Project Status

| Field | Value |
|---|---|
| Status | Active Development |
| Stage | Pre-Production |
| Phase | Phase 0 — Foundation (core drafts in progress) |
| Version | 0.0.2 Alpha |
| Date Started | 9 July 2026 |
| Estimated Documentation | 3,500–5,000 pages |
| Estimated Assets | 25,000+ |
| Estimated Timeline | 12–18 months |

**Latest progress: Season One is now fully production-ready as 20 chapters, with a complete production manual and a fully drafted worldbuilding suite behind it.** Branding decision locked ("GIDAN MULKI" is the flagship title — see GMU-001 Addendum). World Bible core (3 kingdoms, timeline, central conflict, explicit religious basis), Series Bible (themes + full 10-episode beat sheet), and **all 20 Season One chapter screenplays** (~15–20 min each, from "The Sultan's Silence" through the finale "The Crown's Price") are complete. **2026-07-11: restructured from 10 full-length episodes (~20–38 min each) into 20 shorter chapters** to better fit an AI-assisted production pipeline — every scene and line of dialogue is preserved unchanged, this was a structural split only (see GMU-008 for the full episode-to-chapter mapping; the original 10 episode files remain in the repo as retired stubs pointing to their replacement chapters). Every chapter now also has: a **Character Bible entry and AI Model Library design sheet** for every named character (13 total, including 5 added for Episodes 3–10 — Halima, Rafiu, Nafisa, Abubakar, and Yusuf's post-reveal update); a **concept art brief** for every location (10 total, GMU-501–510); a full **reusable Prompt Library** (GMU-007); and a **complete shot-by-shot storyboard** for every chapter (GMU-771–790, 701 shots across 113 scenes total). The **Creative & Brand Bible (GMU-002)** formalizes the visual system all of this was built against. **All fifteen World Bible sub-bibles are now drafted (2026-07-12)** — Religion (GMU-305, research-grounded against real Islamic scholarship), Military (GMU-308), Political (GMU-309), Culture (GMU-304), Architecture (GMU-306), Costume (GMU-307), Economic (GMU-310), Atlas (GMU-311), Language (GMU-312, the ceremonial "Old Tongue"), Calendar (GMU-313), Music (GMU-314), Food (GMU-315), Clothing (GMU-316), Transportation (GMU-317, added 2026-07-12 — cavalry, river barges, the mercenary fleet, palanquins, desert caravans, and everyday transport), and the Master Encyclopedia (GMU-320 schema, 55 entries spanning Places, People, Objects, Events, Culture, Flora/Fauna, and Institutions, including the full founding-era timeline as dedicated Event entries), and a first illustrated Atlas map (`GMU_Atlas_Map.svg`). **2026-07-11: GMU-009 (Marketing Plan) and GMU-010 (Franchise Plan) are now drafted** — positioning, target markets, pitch deck/investor materials plans, and a full multi-media expansion roadmap (publishing, digital, gaming, education, commercial licensing) built against GMU-001's real Scope and Strategic Objectives. The **AI Production Bible (GMU-006)** is a complete step-by-step production manual — tool-by-tool guidance covering every stage from account setup through the Charter quality gate, including current 2026 pricing and a correction removing Udio as a viable music tool (see GMU-006 §1 and GMU-007 §8). **2026-07-12: `17_AI_PRODUCTION/` now also has a full staff-execution layer** — GMU-011 (Cowork-native tools guide), GMU-012 (zero-experience click-level walkthrough of the external pipeline), and GMU-013 through GMU-018 (fully assembled, ready-to-paste checklists: every character/location image prompt, every voice casting entry, a complete Chapter 01 video-shot packet, music/editing/QA steps, and a master timeline mapping who-does-what-when across a multi-person team). A plain-language team onboarding guide lives at `START_HERE.md` — read that first if you're new. The entire season is now ready to hand to external production tools and staff per GMU-018's playbook — actual image/video/voice/music generation still requires those tools, which aren't provisioned yet.

---

## How This Repository Is Organized

This repo mirrors the numbered folder plan established in the GMU founding conversation, with the Phase I worldbuilding expansion nested inside `04_WORLD_BIBLE/` rather than sprawled across the top level, so the structure stays navigable as it grows.

```
GMU/
├── 00_PROJECT/              Charter-adjacent strategy docs, repo standards
├── 01_CHARTER/               GMU-001 — Project Charter (Canon, Approved for Draft Development)
├── 02_CREATIVE_BIBLE/        GMU-002 — Creative & Brand Bible
├── 03_SERIES_BIBLE/          GMU-003 — Series Bible
├── 04_WORLD_BIBLE/           GMU-004 — World Bible + all worldbuilding sub-bibles (all 15 drafted)
│   ├── CULTURE_BIBLE/        GMU-304 — Culture Bible (drafted)
│   ├── RELIGION_BIBLE/       GMU-305 — Religion Bible (drafted, research-backed)
│   ├── ARCHITECTURE_BIBLE/   GMU-306 — Architecture Bible (drafted)
│   ├── COSTUME_BIBLE/        GMU-307 — Costume Bible (drafted)
│   ├── MILITARY_BIBLE/       GMU-308 — Military Bible (drafted)
│   ├── POLITICAL_BIBLE/      GMU-309 — Political Bible (drafted)
│   ├── ECONOMIC_BIBLE/       GMU-310 — Economic Bible (drafted)
│   ├── MASTER_ENCYCLOPEDIA/  GMU-320 — Schema + 55 entries (Places, People, Objects, Events, Culture, Flora/Fauna, Institutions)
│   ├── ATLAS/                GMU-311 — Atlas (drafted, text + illustrated map)
│   ├── LANGUAGE/             GMU-312 — Ceremonial court language, "the Old Tongue" (drafted)
│   ├── CALENDAR/             GMU-313 — Calendar (drafted)
│   ├── MUSIC/                GMU-314 — Music Bible (drafted)
│   ├── FOOD/                 GMU-315 — Food Bible (drafted)
│   ├── CLOTHING/             GMU-316 — Clothing Bible (drafted)
│   └── TRANSPORTATION/       GMU-317 — Transportation Bible (drafted 2026-07-12)
├── 05_CHARACTER_BIBLE/       GMU-005 — Character Bible
│   └── AI_MODEL_LIBRARY/     Per-character face/voice/costume/prompt asset catalog
├── 06_SEASON_ONE/            GMU-008 — Screenplays index + 20 chapter folders (+ 10 retired episode stubs)
│   ├── CHAPTER_01/ … CHAPTER_20/  (current, canonical)
│   ├── 07_EPISODE_01/ … 16_EPISODE_10/  (retired — see each file, points to its replacement chapters)
├── 17_AI_PRODUCTION/         GMU-006 — AI Production Bible, + GMU-011–018 staff execution packs (added 2026-07-12)
├── 18_PROMPTS/               GMU-007 — Prompt Library
├── 19_CONCEPT_ART/
├── 20_STORYBOARDS/
├── 21_SOUNDTRACK/
├── 22_MARKETING/             GMU-009 — Marketing Plan (drafted)
├── 23_PITCH/
├── 24_INVESTORS/
├── 25_BRAND/                 Finalized brand assets (post Creative Bible sign-off)
├── 26_LEGAL/
└── 27_ARCHIVE/
```

## Phase 0 Deliverables (Foundation)

| ID | Document | Est. Pages | Status |
|---|---|---|---|
| GMU-001 | Project Charter | 60 | **Approved for Draft Development** |
| GMU-002 | Creative & Brand Bible | 250 | **In Progress** — logo, typography, kingdom color codes, seals, architecture, costume, cinematography, lighting drafted for all three kingdoms including Kwara (closed 2026-07-11); music/title sequence still provisional |
| GMU-003 | Series Bible | 200 | **In Progress** — premise, themes, full S1 beat sheet drafted, fully realized into screenplay |
| GMU-004 | World Bible (+ sub-bibles) | 350+ | **In Progress** — 3 kingdoms, timeline, central conflict, religious basis (Islam) drafted; **all 15 sub-bibles now drafted** (2026-07-12, Transportation added) |
| GMU-005 | Character Bible | 450 | **In Progress** — 13 cast profiles drafted (6 principal + 7 supporting); all 13 + background roles have AI Model Library design sheets |
| GMU-006 | AI Production Bible | 400 | **In Progress** — full step-by-step manual drafted 2026-07-11, tool-by-tool per production stage, current 2026 pricing/capabilities |
| GMU-007 | Prompt Library | 500 | **In Progress** — core templates drafted (visual style, per-kingdom/faith environments, character consistency, battle/cinematography, voice, music, negative prompts); corrected 2026-07-11 to remove Udio |
| GMU-008 | Screenplays (Season One) | 700 | **Draft — Complete, Production-Ready** — all 20 chapters (~15–20 min each, restructured from 10 episodes), full character/location/prompt/storyboard package |
| GMU-009 | Marketing Plan | 200 | **In Progress** — positioning, target markets, pitch deck/investor materials plans, social strategy, launch sequencing drafted 2026-07-11 |
| GMU-010 | Franchise Plan | 250 | **In Progress** — multi-media expansion roadmap, Year 1/2/3 sequencing, company formation plan, IP strategy drafted 2026-07-11 |

## Production Execution Packs (added 2026-07-12)

Beyond GMU-006's strategy-level playbook, `17_AI_PRODUCTION/` now has a full staff-handoff layer — every document below is ready to execute immediately, no further planning needed:

| ID | Document | Purpose |
|---|---|---|
| GMU-011 | Cowork AI Tools Guide | How to use Claude's built-in design skills (canvas-design, algorithmic-art) directly in this workspace, for quick concept art distinct from the external Midjourney/FLUX pipeline |
| GMU-012 | Zero-Experience Execution Guide | Click-level walkthrough of every external tool in GMU-006's pipeline (Midjourney, ElevenLabs, Kling/Veo, Suno, DaVinci Resolve), written for someone with no prior experience |
| GMU-013 | Character Image Production Checklist | All 13 characters, every prompt already fully assembled and ready to paste |
| GMU-014 | Location Image Production Checklist | All 10 location briefs (28 room/scene prompts), ready to paste |
| GMU-015 | Voice Casting Master Checklist | All 13 characters' voice direction + ElevenLabs casting log template |
| GMU-016 | Video Generation Procedure + Chapter 01 Packet | Chapter 01's full 24-shot packet fully assembled, plus the exact formula to replicate for Chapters 02–20 |
| GMU-017 | Music, Editing & QA Checklist | Suno prompts per kingdom/mood, DaVinci Resolve assembly steps, per-chapter quality gate |
| GMU-018 | Master End-to-End Production Timeline | The single starting point — maps every phase above to a role (Art Lead, Voice Lead, Video Lead, Music Lead, Editor) with explicit handoff points |

See `00_PROJECT/GMU-000_Repository_Standards.md` for the metadata standard every document must carry, and `01_CHARTER/GMU-001_Project_Charter.md` for the canon rules, creative principles, and governance model this project runs on.

## Branding Decision — Resolved

"GIDAN MULKI" is locked as the flagship franchise and series title (see GMU-001 Addendum). Alternatives considered and rejected: *The Crown of Zamar*, *Empire of Zamar*, *The Last Sultan*, *The Twelve Kingdoms*, *Legacy of Zamar*. "Afrasah" is retained as the in-world continent name (GMU-004), not a franchise-title candidate. GMU-002 (Creative & Brand Bible) is now unblocked to build the logo system and brand identity around this name.

## Recommended External Infrastructure (not yet provisioned)

| Purpose | Tool |
|---|---|
| Knowledge Base | Notion |
| Version Control | GitHub (Private org) |
| Documentation | Google Drive |
| Design | Canva / Figma |
| AI Images | FLUX + Midjourney |
| AI Video | Google Veo, Kling AI |
| Voice | ElevenLabs |
| Music | Suno (Pro/Premier plan for commercial rights), ElevenLabs Music — **not Udio**, which as of 2026 no longer allows downloading/exporting generated tracks (see GMU-006 §1) |
| Editing | DaVinci Resolve Studio |

This local repository is the offline source of truth in the meantime — push it to a private GitHub org (`GMU Studio`) when ready, split by repo (`gmu-charter`, `gmu-world-bible`, `gmu-season-one`, etc.) once the org is created. **Update 2026-07-12:** the repository is now live at `https://github.com/huzex87/gmu` as a single unified repo rather than split — that split can still happen later if the project scales enough to warrant it.

*(Note: this closing sentence was found truncated mid-word at "`gmu-`" during the 2026-07-12 update — completed above; no other content in this file was affected.)*