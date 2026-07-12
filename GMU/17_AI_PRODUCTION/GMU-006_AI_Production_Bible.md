Document ID: GMU-006
Document Name: AI Production Bible
Classification: Reference
Version: 1.0 Draft
Status: In Progress
Owner: Huzaifa Yakub
Last Edited: 2026-07-11
Canon Status: N/A
Approval Status: Pending
Dependencies: GMU-002 (Creative & Brand Bible), GMU-005 (Character Bible), GMU-007 (Prompt Library), GMU-008 (Screenplays Index)

---

# GMU-006 — AI Production Bible

The step-by-step manual for turning the completed Season One production package (20 chapter screenplays, 13 character sheets, 10 location briefs, the Prompt Library, and 701 storyboarded shots) into actual footage. Everything upstream of this document is finished; this is the execution playbook. Tool recommendations below reflect each tool's actual capabilities and pricing as of July 2026 — re-verify before committing budget, since this space moves fast and pricing/features change often.

## 0. Pipeline Overview

```
Character/Location Prompts (done: GMU-401–414, GMU-501–510)
        ↓
PHASE 1 — Reference Images (Midjourney / FLUX)
        ↓
PHASE 2 — Voice Casting (ElevenLabs)
        ↓
PHASE 3 — Shot-by-Shot Video Generation (Kling / Veo), per chapter (GMU-771–790)
        ↓
PHASE 4 — Music & Sound Design (Suno / ElevenLabs Music)
        ↓
PHASE 5 — Editing & Assembly (DaVinci Resolve)
        ↓
PHASE 6 — Quality Gate (GMU-001 §12 Charter standard)
        ↓
Finished Chapter
```

Repeat Phases 3–6 per chapter once Phases 1–2 are done once for the whole season. Phase 1 (character images) only needs to happen once per character across all 20 chapters — this is the single highest-leverage step in the whole pipeline, since every later phase depends on it staying consistent.

## 1. Phase 0 — Tool Accounts and Budget Tiers

None of these are provisioned yet. Recommended minimum tier per tool, based on actual current pricing:

| Tool | Purpose | Recommended tier | Why |
|---|---|---|---|
| Midjourney or FLUX (Black Forest Labs) | Character/location reference images | Midjourney Standard, or FLUX.2/Kontext via API | Both now support strong multi-reference character consistency (Section 2) |
| ElevenLabs | Voice casting/generation | **Creator ($22/mo)** minimum | Free and Starter ($5/mo) only unlock Instant Voice Cloning (IVC), which degrades over long passages. Creator unlocks Professional Voice Cloning (PVC), which holds up across a recurring character's full season — worth the jump given every principal character speaks across all 20 chapters |
| Kling AI or Google Veo | Shot-by-shot video generation | Kling 3.0 Pro (pay-per-second) as primary, Veo 3.1 for specific high-stakes shots | See Section 4 for the tradeoff — Kling is roughly 2.4x cheaper per second and has a multi-shot storyboard mode that maps directly onto GMU's existing shot lists; Veo currently leads on prompt adherence and native 4K |
| Suno | Music/score | **Pro or Premier plan** — commercial release rights are NOT included on the free tier, and this doesn't retroactively apply if you upgrade later after generating on free | Generate everything under a paid plan from the start |
| DaVinci Resolve | Editing | Free version is sufficient for Season One; Studio version only needed for specific advanced color/noise-reduction tools | GMU-002 recommends Studio but Free will not block production |

**Do not use Udio for this project.** As of 2026, Udio has become a closed "walled garden" platform — generated music cannot be downloaded or used in external projects, which makes it structurally incompatible with a video production pipeline. This reverses earlier guidance (GMU-007 §8, README's tool list) written before this platform change; treat Suno or ElevenLabs Music as the only viable AI-music options for GMU going forward, and flag GMU-007/README for a follow-up correction.

## 2. Phase 1 — Character & Location Reference Images

**Goal:** one locked, approved reference image (or small image set) per character and per location, that every later video generation gets checked against.

**Step 1.1 — Generate.** Open a character's sheet in `05_CHARACTER_BIBLE/AI_MODEL_LIBRARY/`, copy its "AI Image Generation Prompt" verbatim into your chosen tool. Generate 4–8 variations per character.

- **In Midjourney:** After your first accepted image, use `--cref [image URL]` on all subsequent generations of that same character to lock facial/body consistency, and tune `--cw` (0–100) — higher values hold the reference more strictly, lower values allow more scene-appropriate variation (expression, angle). For an even higher-fidelity lock across a full season, Midjourney's Omni Reference (`--oref` + `--ow`) is worth testing as an alternative to `--cref`.
- **In FLUX (Kontext/FLUX.2):** Upload the character's accepted image as a reference; FLUX.2 accepts multiple reference images at once (up to 8 via API, 10 in the playground) — useful for locking a character's face, costume, and a specific prop (e.g., Yusuf's signet) simultaneously in one generation call.

**Step 1.2 — Select and lock.** Pick the strongest result per character/location. Save it into that character's folder in `AI_MODEL_LIBRARY/` (or the location's folder in `19_CONCEPT_ART/`) as `<name>_REFERENCE_v1.png`. This file becomes the input for every future generation of that character — never re-describe a character from memory once a reference is locked.

**Step 1.3 — Costume variants.** Several characters need more than one locked look (Fatima's mourning overlay, Halima's public vs. private variant, Yusuf's post-reveal signet detail). Generate and lock these as `<name>_REFERENCE_v1_<variant>.png` rather than overwriting the base reference.

**Order of operations:** do all 13 characters and all 10 locations before starting Phase 3 (video) on any chapter — mixing "some references locked, some not" invites inconsistency that's expensive to fix later.

## 3. Phase 2 — Voice Casting

**Step 2.1 — Cast.** For each character with dialogue, either select a stock ElevenLabs voice matching that character's Voice Direction notes (every character sheet has one), or clone a voice if you have a specific actor's sample and rights to use it.

**Step 2.2 — Clone (if applicable).** Use Professional Voice Cloning (PVC) — available from the Creator tier up — for any principal or recurring character (essentially everyone in the 13-character roster, since all appear across multiple chapters). PVC requires more training audio than Instant Voice Cloning but holds up far better across a full season's worth of generated dialogue; IVC is acceptable only for genuinely one-scene background characters (GMU-410).

**Step 2.3 — Log the binding.** Fill in GMU-007 §7's casting-log template for every character once cast, recording the actual ElevenLabs voice ID against the character. This is the single most important record-keeping step in this phase — without it, nothing guarantees the same actor "voices" a character in Chapter 14 that voiced them in Chapter 2.

**Step 2.4 — Generate dialogue per chapter.** Once cast, generate each chapter's dialogue lines directly from that chapter's screenplay (`06_SEASON_ONE/CHAPTER_01/` through `CHAPTER_20/`), using each character's locked voice ID and the Voice Direction notes for tonal guidance (pace, register, emotional shifts called out per scene).

## 4. Phase 3 — Shot-by-Shot Video Generation

This is the most expensive and time-consuming phase — plan for it accordingly. Work one chapter at a time, following that chapter's shot list in `20_STORYBOARDS/CHAPTER_01/` through `CHAPTER_20/`.

**Tool choice — Kling vs. Veo:**

- **Kling 3.0 (Pro tier)** is the recommended default. It costs roughly $0.168/second with audio (versus Veo 3.1's roughly $0.40/second), and its "Elements 3.0" feature accepts a video or image reference and replicates a character with high fidelity across multiple scenes — well suited to GMU's need for the same 13 characters to recur across 701 shots. Kling also has a multi-shot storyboard mode with native audio sync across cuts, which maps unusually well onto GMU's existing scene-by-scene shot list structure — worth testing directly against a full scene (e.g., Chapter 01 Scene 3) rather than shot-by-shot, if the tool supports feeding it multiple consecutive shot descriptions at once.
- **Veo 3.1** is the recommended choice for the season's highest-stakes individual shots — the ones flagged in each chapter's Production Notes as highest priority (e.g., Chapter 01's Teaser, the Chapter 19–20 coronation sequence) — where its stronger prompt adherence, native audio, and 4K output justify the higher per-second cost. Its "Ingredients to Video" feature takes three reference images (useful for character + location + a key prop in one generation).

**Step 3.1 — Per shot.** For each shot row in the chapter's shot list, feed the tool: the shot's Type/Description (from the table), the relevant character reference image(s), the relevant location reference image, and the base style/lighting language from GMU-007 §§1–2 and GMU-002 §11 for that kingdom.

**Step 3.2 — Consistency check.** Compare each generated shot against the previous shot in the same scene before moving on — catching a drifted face or a wrong-colored banner immediately is far cheaper than catching it during editing, when regenerating means re-matching the whole surrounding sequence's continuity.

**Step 3.3 — Prioritize.** Every B-chapter's shot list carries forward its source episode's Production Notes, flagging the highest-priority shots for that content. Generate those first per chapter — if time or budget runs out partway through a chapter, the most important shots are already secured.

**Recommended chapter order:** Chapters 01–02 first (Episode 1's material, already the most heavily detailed and battle-tested prompt-wise), then Chapters 19–20 (the finale, the season's visual culmination and most likely to appear in any trailer or pitch reel), then the rest in story order.

## 5. Phase 4 — Music and Sound Design

**Step 4.1 — Score.** Use GMU-007 §8's per-kingdom/mood music direction as the prompt basis in Suno (Pro/Premier plan, for commercial rights). Generate per-scene or per-chapter cues rather than one long score, so specific cues can be swapped without regenerating an entire chapter's music.

**Step 4.2 — Alternative/supplement.** ElevenLabs Music is a licensed-training-data alternative worth testing alongside Suno, particularly for cases needing precise editing after generation — it added stem separation and an Inpainting API for editing specific sections in early 2026, useful for fixing a single bar of a cue without regenerating the whole piece.

**Step 4.3 — Sound design.** Ambient/foley sound design (crowd noise, cavalry, market ambience, wind at Tsauri Keep) isn't covered by GMU-007 yet — source stock/library sound effects or generate via whichever tool's SFX features are available, matching the scene's location and mood.

## 6. Phase 5 — Editing and Assembly

**Step 5.1 — Assemble in order.** Using DaVinci Resolve (Free tier is sufficient for Season One), assemble each chapter's generated shots in the order given by that chapter's screenplay, not necessarily the order they were generated in.

**Step 5.2 — Add audio layers.** Dialogue (Phase 2) → music (Phase 4) → sound design, in that priority order for the mix — dialogue clarity should never be sacrificed for music or ambience.

**Step 5.3 — Color pass.** Grade each scene to match its location's established palette (GMU-002 §11, GMU-501–510's individual briefs) — this is where GMU-002's kingdom-specific lighting philosophy (warm amber Zamar, harsh overcast Kasar Dutse, reflected water-light Kwara, clear unshadowed Covenant light) actually gets locked in, since AI-generated shots will vary in color temperature even from consistent prompts.

**Step 5.4 — Titles.** Apply GMU-002 §14's title-card direction (compass rose reveal, palette-cycling background) once a real title sequence has been cut, per that section's guidance to defer full production until footage exists to cut against.

## 7. Phase 6 — Quality Gate

Before calling any chapter finished, check it against GMU-001 §12's Charter quality bar: consistent architecture, consistent costumes, consistent color language, clear narrative, distinct character voices. Apply this per chapter, not just once for the season — a chapter generated early in the pipeline (when reference images were newer/less tested) is exactly where drift is most likely to show up on a second look.

## 8. Cross-Tool Consistency Strategy

The single hardest problem in this entire pipeline is keeping 13 characters and 10 locations visually identical across 20 chapters and 701 shots, generated by tools that don't share state with each other. Mitigate this by:

- Never regenerating a character's base reference image once locked (Section 2) — every downstream generation traces back to that one file.
- Keeping a single master folder of locked references (`05_CHARACTER_BIBLE/AI_MODEL_LIBRARY/*_REFERENCE_v1.png`, `19_CONCEPT_ART/*_REFERENCE_v1.png`) that every tool pulls from, rather than letting each generation session re-upload a slightly different source image.
- Logging which tool, model version, and reference-strength setting (e.g., Midjourney `--cw 80`) produced each character's accepted reference, so a later re-generation (if a tool updates its model mid-production) can be matched rather than drifting.
- Treating GMU-007 (Prompt Library) as the single source of truth for style language — if a generation doesn't match its written prompt template, fix the prompt or the settings, don't silently accept the drift.

## 9. Version Control for Generated Assets

Name locked assets predictably: `<CharacterOrLocationName>_REFERENCE_v<N>.<ext>` for stills, `Chapter_<NN>_Shot_<scene>.<shot>_v<N>.<ext>` for video clips. Keep every accepted version rather than overwriting — if v2 of a character reference turns out worse after generating ten shots against it, v1 needs to still exist to revert to.

## 10. Rough Cost Estimate (Season One, all 20 chapters)

Order-of-magnitude only — actual costs depend heavily on retry/regeneration rates, which are unpredictable until real production starts:

- **Images (Phase 1):** 23 assets (13 characters + 10 locations) × several generations each — low cost, likely under $50–100 total on any major tool's paid tier.
- **Voice (Phase 2):** ElevenLabs Creator plan ($22/mo) covers a season's worth of dialogue generation for most projects this size; upgrade to Pro ($99/mo) if character count or dialogue volume runs high.
- **Video (Phase 3):** the dominant cost. At Kling 3.0 Pro's ~$0.168/sec, a season averaging even 3 seconds per shot across 701 shots is roughly $350 before any regeneration; Veo-generated priority shots at ~$0.40/sec add more on top. Budget for 2–3x the base estimate to cover retries and consistency fixes.
- **Music (Phase 4):** Suno Pro/Premier plans run roughly $10–30/mo depending on tier.
- **Editing (Phase 5):** free if using DaVinci Resolve's free tier.

Treat this section as a planning estimate to revisit once Phase 1 actually starts — real per-tool pricing and your own retry rate will refine it fast.

## 11. Sources Consulted (tool capability/pricing research, July 2026)

- ["Character Reference" — Midjourney Docs](https://docs.midjourney.com/hc/en-us/articles/32162917505293-Character-Reference)
- ["How to use Midjourney --cref for consistent characters"](https://prompting.systems/blog/how-to-use-midjourney-cref-for-consistent-characters)
- ["Best AI for Character Consistency in 2026" — ToonyStory](https://toonystory.com/blog/best-ai-for-character-consistency-2026)
- ["Kling AI vs Veo 2026" — Elser AI Blog](https://www.elser.ai/blog/kling-ai-vs-veo-2026)
- ["AI Video Generator" — Kling 3.0](https://kling.ai/feature/ai-video-generator)
- ["Best AI Video Generators 2026" — AI/ML API Blog](https://aimlapi.com/blog/best-ai-video-generators-2026-veo-3-1-kling-sora-2-seedance-more-compared)
- ["The Complete Guide to ElevenLabs Plans" — Flexprice](https://flexprice.io/blog/elevenlabs-pricing-breakdown)
- ["ElevenLabs Pricing (2026)" — Magic Hour](https://magichour.ai/blog/elevenlabs-pricing)
- ["AI Music Licensing in 2026" — LicenseOrg](https://www.licenseorg.com/blog/ai-music-licensing-suno-elevenlabs)
- ["Suno Music in 2026" — Medium](https://medium.com/@J.S.Matkowski/suno-music-in-2026-what-creators-actually-own-what-they-only-license-and-why-the-lawsuits-still-7f7c3c455c0e)

## Status

In Progress. Full step-by-step pipeline drafted and tool-current as of July 2026. Flagged for follow-up: GMU-007 §8 and the root README's "Recommended External Infrastructure" table both still list Udio as a music option — both should be corrected to remove Udio given its 2026 platform change (Section 1 above), and README/START_HERE should note ElevenLabs Music as an alternative. Cost estimates (Section 10) are planning-stage only and should be revised once Phase 1 actually begins and real retry rates are known.
