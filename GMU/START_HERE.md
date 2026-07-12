# START HERE — Welcome to Gidan Mulki Universe (GMU)

If you're new to this project, read this document first, start to finish, before opening anything else in the repository. It's written so that someone with zero prior context — a new writer, artist, editor, or producer joining the team — can understand what this is, where things stand, and what to actually do next. Nothing here assumes you've read anything else.

---

## 1. What Is This, In One Paragraph

Gidan Mulki Universe (GMU) is an original fictional TV/film franchise — a political epic set in an African-inspired world, being built using AI tools to accelerate writing, art, and video production while a human team makes every real creative decision. Think of it like building a TV show the way a studio would: a locked story bible, character designs, location designs, and scripts, all produced before any actual footage is generated. This repository is the single source of truth for all of it — every document, decision, and design lives here, versioned and organized, so nothing gets lost or contradicted as the team grows.

## 2. The 60-Second Story So Far

The show is called **Gidan Mulki** — that title is locked, it's not changing. It's set in a fictional world called **Afrasah**, in a region called the Sahel Crescent, inspired by the trade, scholarship, and statecraft of real Sahelian civilizations without copying any single one of them.

Three powers share this world: the **Sultanate of Zamar** (rules by law and scholarship — its throne can only pass to someone approved by a council of scholars called the Diwan al-Ilm), the **Kingdom of Kasar Dutse** (a mountain warrior kingdom that controls the trade passes), and the **River Confederacy of Kwara** (merchant city-states that profit off everyone else's business, loyal to nobody).

Season One's story: Zamar's Sultan dies suddenly with no approved heir. His two children — **Fatima**, a scholar, and **Malik**, a soldier — have forty days to win the council's approval, and they love each other, which is what makes it a tragedy and not just a power grab. The mountain king and the merchant power both start circling, looking to profit from the chaos. Episode One ends with the murder of a beloved old advisor who was getting too close to a secret about how the Sultan really died — and the person closest to that secret, an advisor named Yusuf, isn't who everyone thinks he is.

**The full season is now written, start to finish — as 20 shorter chapters instead of 10 full episodes.** On 2026-07-11 the season was restructured so each ~20–38 minute episode became two ~15–20 minute chapters, better suited to an AI-generation pipeline (roughly half the shots to produce and review per release unit). No story content changed — every scene and line of dialogue carried over unchanged, just repackaged with a cliffhanger at every chapter break instead of only every episode break. The investigation into that murder (Chapters 03–04) leads through military pressure and a border skirmish (Chapters 05–06, 09–10), a merchant power revealed to be financing both royal siblings at once (Chapters 07–08), a public legitimacy crisis with the kingdom's clergy (Chapters 11–12), an outright territorial seizure by the mountain kingdom (Chapters 13–14), a quieter stretch following ordinary soldiers and villagers living with the consequences (Chapters 15–16), the exposure of Yusuf's true loyalty to a mysterious, unnamed "fourth power" operating behind all three kingdoms (Chapters 17–18), and a season finale where Fatima is crowned Zamar's first female ruler — at a real, lasting cost (Chapters 19–20). A season finale twist leaves a hook for Season Two.

That's the whole premise. Everything else in this repository is either building the world that story happens in, or turning that story into actual produced episodes.

## 3. How This Repository Is Organized (Plain-Language Tour)

Everything lives inside the `GMU/` folder. Here's what each part is, in order of how a new team member would actually use them:

**`01_CHARTER/`** — The project's constitution. One document (GMU-001) that says what this show is trying to be, what "done" looks like, and the creative rules every decision has to follow. Read this if you want to understand *why* a decision was made.

**`03_SERIES_BIBLE/`** — The story itself. Premise, themes, and a beat-by-beat outline of what happens in every episode of Season One.

**`04_WORLD_BIBLE/`** — Everything about the fictional world: the three kingdoms, the timeline, how the succession law works, and the world's religious basis (Zamar's dominant faith is explicitly Islam — see GMU-004 Section 1). **All fifteen sub-folders are now drafted** (2026-07-12): religion, military, political, culture, architecture, costume, economics, atlas (written geography), language (a constructed ceremonial "Old Tongue"), calendar, music, food, clothing, transportation (cavalry, river barges, the mercenary fleet, palanquins, desert caravans, everyday transport), and the Master Encyclopedia (55 entries). Each is scoped to "just enough, just in time" rather than exhaustive — deeper detail within any of them still gets added only when a specific future episode needs it.

**`05_CHARACTER_BIBLE/`** — Every named character: who they are, what they want, how they talk. Inside it, `AI_MODEL_LIBRARY/` has a **design sheet for every named character across all 10 episodes** (13 total) — physical description, costume, and a ready-to-use AI image prompt, so anyone generating art gets the same face every time.

**`06_SEASON_ONE/`** — The actual scripts. All 20 chapter folders (`CHAPTER_01/` through `CHAPTER_20/`) now have a finished, complete screenplay — the entire first season is written. (The original 10 episode folders, `07_EPISODE_01/` through `16_EPISODE_10/`, still exist but now just contain short retired notices pointing to the chapters that replaced them — don't use those for production.)

**`17_AI_PRODUCTION/`** — The AI Production Bible (GMU-006): a complete step-by-step manual for actually producing the season, with tool-by-tool guidance for every stage (reference images, voice, video, music, editing) and current 2026 pricing. **As of 2026-07-12, this folder also has a full staff-handoff execution layer**: GMU-011 (Cowork-native design tools), GMU-012 (zero-experience walkthrough of the external tools), and GMU-013 through GMU-018 — fully assembled, ready-to-paste checklists for every phase, ending in GMU-018's master timeline that maps each phase to a role and hands off between them. If your job is to actually execute production rather than plan it, start at GMU-018, not Section 6 below.

**`18_PROMPTS/`** — The reusable AI prompt system (GMU-007): master visual style, per-kingdom/faith environment templates, character consistency formulas, battle/cinematography guidance, voice and music direction, and negative-prompt guardrails. Read this before generating anything freehand — it's the shared "house style" every other prompt in the repo already follows.

**`19_CONCEPT_ART/`** — Design briefs for every location used across all 10 episodes (10 briefs total: the palace, the city, the university, the cavalry grounds, Tsauri Keep, the Great Sanctuary of the Covenant, the Kwarafi Merchant House, the border village of Kantin Rafi, the Old Customs House), each with an AI image prompt, so every room looks consistent across scenes.

**`20_STORYBOARDS/`** — Every chapter's script broken down into individual camera shots — the actual unit of work for generating video. All 20 chapters now have complete shot lists (701 shots total, exact count).

**Everything else** (`21_SOUNDTRACK/`, `22_MARKETING/`, etc.) is scaffolded with folders and placeholder documents but genuinely empty — nobody's done that work yet. Don't be alarmed to open one of these and find almost nothing; that's accurate, not broken.

For the full technical folder map, see `README.md` in this same root folder — it's the more compact, reference-style version of this same information.

## 4. How to Read Any Document in This Repo

Every document starts with the same header block. Here's what each line means in plain terms:

- **Document ID** — a unique code (like `GMU-401`) so documents can reference each other without ambiguity.
- **Status** — where the document is in its life: `Not Started`, `Draft`, `In Progress`, `In Review`, or `Approved`. If it doesn't say `Approved`, treat it as subject to change.
- **Canon Status** — `Provisional` means "this is our current best answer but hasn't been formally locked"; `Canon` means "this is now fixed, don't contradict it without a real reason." Most of this repo is still Provisional. A small number of decisions (the show's title, the succession law, the core cast, the religious basis) are already locked Canon.
- **Dependencies** — what other documents this one relies on. If you're about to change something, check who depends on it first — that's how big projects avoid quietly contradicting themselves.

You don't need to memorize this — just know that these six lines at the top of every file tell you how much you should trust what follows.

## 5. Where Things Actually Stand Right Now

Here's the honest status, not the aspirational one:

**Finished and ready to use — the entire Season One production package:** The Charter (locked). The show's title (locked). The core world (3 kingdoms, timeline, central conflict, religious basis). **All 20 Season One chapter screenplays** (~15–20 min each) — the entire season is written, from the Sultan's death through the coronation finale, restructured from the original 10 full-length episodes for easier production. **All 20 chapters' shot-by-shot storyboards** (701 shots across 113 scenes, exact count). **All 13 named characters' design sheets** (physical reference, costume, AI image prompt, voice direction). **All 10 locations' concept art briefs.** A full **Prompt Library** (GMU-007) with reusable templates for visual style, environments, character consistency, battle scenes, cinematography, voice, and music. The Creative & Brand Bible (logo, typography, locked color codes for all three kingdoms, seals, architecture, costume, cinematography, and lighting rules).

**Also finished (2026-07-11):** A full **AI Production Bible** (GMU-006) — a complete step-by-step manual walking through every production stage with concrete, current tool guidance (Midjourney/FLUX, ElevenLabs, Kling/Veo, Suno/ElevenLabs Music, DaVinci Resolve) and rough cost estimates. **All fifteen World Bible sub-bibles**: Religion (GMU-305, researched against real Islamic scholarship), Military (GMU-308), Political (GMU-309), Culture (GMU-304), Architecture (GMU-306), Costume (GMU-307), Economic (GMU-310), Atlas (GMU-311), Language (GMU-312), Calendar (GMU-313), Music (GMU-314, replacing GMU-007 §8's old placeholder-only direction), Food (GMU-315), Clothing (GMU-316), Transportation (GMU-317, added 2026-07-12), and the Master Encyclopedia (GMU-320 schema, 55 entries).

**Also finished (2026-07-12):** The staff-execution layer — GMU-011 through GMU-018 in `17_AI_PRODUCTION/` — turns GMU-006's strategy into literal, ready-to-hand-off checklists: every character/location image prompt pre-assembled, every voice casting entry, a fully worked Chapter 01 video-shot packet, music/editing/QA steps, and a master timeline assigning each phase to a role. The repository is also now live on GitHub at `https://github.com/huzex87/gmu`.

**Not started yet:** Deeper Master Encyclopedia population beyond its current 55 entries, higher-fidelity Atlas maps (a first illustrated map exists, `GMU_Atlas_Map.svg`), and Season Two material. Any actual generated image, video, voice, or music — everything up to this point is *design and planning*, not produced content. No external production tools (image/video/voice AI) have been set up yet.

If someone asks "is the show made yet," the honest answer is: no footage exists. What exists is a complete, professional-grade Season One production package — every script, every character design, every location design, a full reusable prompt system, and every shot list — ready to be fed into image and video tools from the very first shot to the last.

## 6. How to Actually Produce Season One — Step by Step

**Updated 2026-07-12: the fastest path into this section is no longer the 8 steps below — it's `17_AI_PRODUCTION/GMU-018_Master_Production_Timeline.md`.** That document does everything Steps 1–8 below describe, except every prompt is already fully assembled and ready to paste, every checklist is ready to hand directly to a specific staff member (an Art Lead, a Voice Lead, a Video Lead, etc.), and it tells you exactly who hands off to whom. The 8 steps below are kept as the plain-language overview of *why* the pipeline is ordered this way — read them for context, then go execute from GMU-018 and its linked documents (GMU-013 through GMU-017) rather than working from memory.

This is the part that matters if your job is to make this real. Every script, character, location, prompt, and shot list for all 20 chapters is done — this is now purely an execution pipeline. The quick version is below; for the full step-by-step manual with current tool pricing, specific settings (e.g., Midjourney's `--cref`/`--oref`, Kling's Elements 3.0), and a rough cost estimate, read `17_AI_PRODUCTION/GMU-006_AI_Production_Bible.md`. Follow this order — each step depends on the one before it. Repeat Steps 5–8 per chapter once Steps 1–4 are done once for the whole season.

**Step 1 — Set up the tools.** None of these are connected yet. You'll need accounts for: an AI image generator (FLUX or Midjourney) for concept art and character/location references, an AI video generator (Google Veo or Kling AI — Kling recommended as the lower-cost default, see GMU-006 §4), a voice tool (ElevenLabs, Creator tier or higher), and a music tool — **Suno (Pro/Premier plan) or ElevenLabs Music, not Udio**, which as of 2026 no longer allows downloading generated tracks (see GMU-006 §1) — and video editing software (DaVinci Resolve Studio recommended, but any professional editor works). Read `18_PROMPTS/GMU-007_Prompt_Library.md` first — every prompt in this repo already follows its conventions, and it'll save you from reinventing phrasing per-asset.

**Step 2 — Generate and lock character reference images.** Go to `05_CHARACTER_BIBLE/AI_MODEL_LIBRARY/`, open each of the 13 character files, and run their AI image prompt through your chosen image tool. Generate a few options per character, pick the best one, and save it back into that character's folder as the official reference — this becomes the thing every future shot of that character gets checked against, across all 10 episodes.

**Step 3 — Generate and lock location reference images.** Same process, using all 10 briefs in `19_CONCEPT_ART/` (GMU-501–510). Do this for every setting before generating any video — consistent locations matter as much as consistent faces, especially since several locations (the Palace, the border pass, Tsauri Keep) recur across many episodes.

**Step 4 — Cast and generate voices.** For every character with dialogue across the season, choose or clone a voice in ElevenLabs matching the voice direction notes in each character sheet. Use GMU-007 §7's casting-log template to record the binding once you've chosen.

**Step 5 — Generate video, shot by shot, per chapter.** Open the relevant shot list in `20_STORYBOARDS/` (e.g. `CHAPTER_01/Chapter_01_Shot_List.md` for Chapter 1, `CHAPTER_02/Chapter_02_Shot_List.md` for Chapter 2, and so on through Chapter 20). Work through each chapter's shots in order, feeding your locked character and location images as references into your video tool. Each B-chapter's Production Notes section (carried forward from the original episode-level notes) flags which scenes matter most — get those right first, even if you generate other scenes out of order. Recommended order: Chapters 01–02 and 19–20 first (Episode 1's material is the most detailed; the finale is the visual culmination), then the rest in story order.

**Step 6 — Score and sound design.** Use `04_WORLD_BIBLE/MUSIC/GMU-314_Music_Bible.md` for concrete per-kingdom instrumentation and occasion-based repertoire (battle, wedding, funeral, market, devotional), or GMU-007 §8 for the shorter mood-only summary.

**Step 7 — Edit.** Assemble each chapter's generated shots in order in your editing software, following the scene order in that chapter's screenplay (`06_SEASON_ONE/`), add the dialogue audio, music, and sound design, and do a final color pass matching the palette described in each location's concept brief.

**Step 8 — Review against the Charter's quality bar.** Before calling any chapter finished, check it against Section 12 of the Charter (`01_CHARTER/GMU-001_Project_Charter.md`): consistent architecture, consistent costumes, consistent color language, clear narrative, distinct character voices. That's the bar this project set for itself — apply it per episode, not just once for the season.

## 7. Who Does What (Roles Needed)

You don't need all of these to be different people — one person can wear several hats, especially early on. But here's the full breakdown of what a fully-staffed version of this looks like, and which files each role lives in:

| Role | What They Do | Main Files They Use |
|---|---|---|
| **Showrunner / Story Lead** | Owns the Charter, the Series Bible, and all creative decisions. Final say on canon. | `01_CHARTER/`, `03_SERIES_BIBLE/`, `00_PROJECT/` |
| **World-builder** | Expands the World Bible's sub-bibles (religion, military, economy, etc.) as episodes need them. | `04_WORLD_BIBLE/` |
| **Screenwriter** | Writes and revises episode scripts. | `06_SEASON_ONE/`, `05_CHARACTER_BIBLE/` |
| **Concept Artist** | Generates and refines character and location reference images from the design sheets. | `05_CHARACTER_BIBLE/AI_MODEL_LIBRARY/`, `19_CONCEPT_ART/` |
| **AI Prompt Engineer** | Maintains and improves the prompt library as more gets produced. | `18_PROMPTS/`, all design sheet files |
| **Storyboard Artist** | Breaks scripts into shot lists like the one already done for Episode 1. | `20_STORYBOARDS/` |
| **Voice Director** | Casts and directs AI voice generation per character. | `05_CHARACTER_BIBLE/AI_MODEL_LIBRARY/` (voice direction notes) |
| **Video Generation Operator** | Runs the actual shot-by-shot AI video generation. | `20_STORYBOARDS/`, locked reference images |
| **Composer / Sound Designer** | Scores and sound-designs each episode. | `21_SOUNDTRACK/` |
| **Editor** | Assembles final cuts. | All generated assets |
| **Producer / Coordinator** | Keeps the repository organized, tracks document status, makes sure nothing contradicts anything else. | Everything — especially `00_PROJECT/GMU-000_Repository_Standards.md` |

## 8. Glossary — In-World Terms

**Diwan al-Ilm** — Zamar's ruling council of Islamic scholars (Ulama) and jurists. No one can become Sultan of Zamar without their approval. Modeled on the real historical Islamic governance concept of Ahl al-Hall wal-Aqd.

**The Faith of the Covenant** — Zamar's local name for its dominant religion, which is explicitly Islam (see GMU-004 World Bible Section 1 for the full decision). Its scripture is the Qur'an, its legal-moral framework is Shari'ah, and its scholarly clergy (the Ulama) sit on the Diwan. "The Covenant" and "Diwan al-Ilm" are this specific fictional Sultanate's own historical names for its Islamic institutions — not a separate, invented religion.

**CU (Years of the Covenant)** — the in-world calendar system. The story currently takes place in 427 CU.

**Zamar** — the scholarly kingdom, ruled by law rather than pure bloodline. Colors: indigo, gold, white.

**Kasar Dutse** — the mountain warrior kingdom controlling the trade passes. Colors: deep red, iron-grey, black.

**Kwara (River Confederacy)** — the merchant power, loyal to money rather than any throne. Colors: emerald, white, silver.

**Afrasah** — the name of the fictional continent the whole story takes place on.

**Birnin Zamar** — Zamar's capital city.

**Tsauri Keep** — Kasar Dutse's capital fortress.

## 9. Glossary — Repository / Production Terms

**Document ID** — a unique reference code for every file (e.g., GMU-401), so files can point to each other precisely.

**Canon** — a decision or fact that's now locked and shouldn't be casually changed.

**Provisional** — a decision that's the current best answer but could still change.

**Bible** — industry term for a reference document that defines something (a "Character Bible," a "World Bible") — not a religious text, just production jargon.

**Beat sheet** — a scene-by-scene or episode-by-episode outline of what happens, written before the full script.

**Concept art** — early reference images used to lock down what something looks like before it's used in actual footage.

**Storyboard / shot list** — a script broken down into individual camera shots, the actual unit of work for filming or generating video.

## 10. Frequently Asked Questions

**Can I change something that's marked Canon?** Only with a real reason, and only by updating the document properly (bump its version number, note what changed and why, and check what else depends on it — see `00_PROJECT/GMU-000_Repository_Standards.md` for the full process). Don't just overwrite it.

**I want to add a new character or location — where does it go?** Follow the existing pattern: a character sheet goes in `05_CHARACTER_BIBLE/AI_MODEL_LIBRARY/`, following the format of the existing nine files. A new location goes in `19_CONCEPT_ART/`. Give it the next available Document ID in that range (see the ID ranges listed in `00_PROJECT/GMU-000_Repository_Standards.md`).

**Something in the World Bible or Series Bible seems incomplete — is that a mistake?** No. This project deliberately only writes detail when an actual episode needs it, instead of writing thousands of pages speculatively before any story exists. If you need something that isn't written yet, write it, but write only as much as your specific scene actually requires.

**Who approves things?** Until the team formally assigns roles, the Showrunner/Story Lead role (see Section 7) owns final creative sign-off on anything marked Canon.

**Where do I ask questions if I'm still stuck?** Check the root `README.md` for the more technical/compact version of this same map, and check each folder's own `README.md` — most folders have one explaining exactly what belongs there.

## 11. Where to Go Next

If you're joining as a creative (writer, artist, world-builder): read `01_CHARTER/GMU-001_Project_Charter.md` next, then `03_SERIES_BIBLE/GMU-003_Series_Bible.md`.

If you're joining as production (artist, video, voice, editor): skip straight to `17_AI_PRODUCTION/GMU-018_Master_Production_Timeline.md` — it'll tell you exactly which of GMU-013 through GMU-017 is yours to execute. Section 6 above is background context, not the execution document anymore.

If you're joining as a producer/coordinator: read `00_PROJECT/GMU-000_Repository_Standards.md` next — that's the rulebook for keeping this whole system consistent as more people touch it.
