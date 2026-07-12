Document ID: GMU-011
Document Name: Cowork AI Tools Guide — Zero-Experience Walkthrough
Classification: Reference (Production Asset)
Version: 1.0
Status: In Progress
Owner: Huzaifa Yakub
Last Edited: 2026-07-12
Canon Status: N/A
Approval Status: Pending
Dependencies: GMU-002 (Creative & Brand Bible), GMU-005 (Character Bible), GMU-006 (AI Production Bible), GMU-007 (Prompt Library)

---

# GMU-011 — Cowork AI Tools Guide

This is the beginner-level companion to GMU-006 (AI Production Bible). GMU-006 covers the *external* pipeline (Midjourney/FLUX, Kling/Veo, ElevenLabs, Suno, DaVinci Resolve) for finished production assets. This document covers the tools available **right here inside this Cowork chat**, with zero assumed experience — exactly what to type, where the source material comes from, and where the output goes.

Two things are true at once, and both matter:

- The tools in this document (canvas-design, algorithmic-art, Adobe for creativity) work *right now*, with no signup, inside this conversation.
- They are **not** a substitute for GMU-006's Midjourney/FLUX step for locked, photorealistic, cross-episode-consistent character and location references. Use this document for concept sketches, posters, marketing pieces, sigils/patterns, and quick visual exploration. Use GMU-006 for the actual "locked reference" images every video generation depends on.

---

## 0. The Golden Rule: Never Write a Prompt From Scratch

GMU already has every visual description you need, pre-written and locked to the project's style, in three places:

| Need | Go here first |
|---|---|
| A specific character's look | `05_CHARACTER_BIBLE/AI_MODEL_LIBRARY/<Name>_assets.md` — bottom section, "AI Image Generation Prompt" |
| A specific location's look | `19_CONCEPT_ART/GMU-50X_....md` — each scene has its own "AI image prompt" callout |
| The master style rules that apply to everything | `18_PROMPTS/GMU-007_Prompt_Library.md` — Section 1 (master style block), Section 9 (negative prompt / guardrails) |

**Rule of thumb:** copy the existing prompt out of the file, paste it into whichever tool below you're using, and only then adjust it for the specific new thing you want (a pose, an angle, a mood). Never describe a character or location freehand from memory — that's exactly how visual drift happens across 20 chapters, and GMU-007 exists to prevent it.

---

## 1. Tool A — `canvas-design` (built in, use this the most)

**What it actually does:** generates an original static image (PNG or PDF) — posters, character portraits, location art, cover art, sigils — following real design/composition principles rather than a raw diffusion-model guess. It does not pull from an external image-generation API; it's a Claude-native design skill.

**Best for in GMU:** poster-style character art, single illustrative location pieces, kingdom sigils/patterns, cover art, pitch-deck visuals, anything where "one strong illustrative image" is the goal rather than a strict photoreal turnaround sheet.

**Not ideal for:** the strict multi-angle "front / three-quarter / side profile" reference turnarounds GMU-006 needs for video-generation consistency — those specifically require an external photoreal tool (Midjourney/FLUX) per GMU-006 Section 2.

### Step by step (character example — Fatima)

1. Open `05_CHARACTER_BIBLE/AI_MODEL_LIBRARY/Fatima_bint_Adamu_assets.md` and copy the paragraph under "AI Image Generation Prompt."
2. In this chat, type a message like:

   > Use the canvas-design skill to create a portrait illustration of Fatima bint Adamu for GMU. Use this description: [paste the copied paragraph]. Style: Sahel-inspired West African aesthetic, indigo (#2E3A6E) and gold (#C9A24B) palette, dignified and composed, no anachronistic elements. Save it as a PNG.

3. I'll generate the image and show it to you in the response. If something's off (wrong mood, wrong garment detail), just reply in plain language — "make the expression less warm, more guarded" — and I'll regenerate.
4. Once you're happy with it, say "save this to the GMU project" — I'll place it in the correct folder (see Section 4 below) and confirm the file path.

### Step by step (location example — Birnin Zamar River Port)

1. Open `19_CONCEPT_ART/GMU-501_Birnin_Zamar_City.md` and copy the "AI image prompt" line under "River Port (Teaser)."
2. Type:

   > Use canvas-design to create a wide establishing illustration for GMU: [paste the copied prompt]. Match the Zamar palette (indigo #2E3A6E, gold #C9A24B, off-white #F4EFE4) from GMU-002.

3. Review, refine, save — same as above.

### Step by step (kingdom sigil / pattern — no character bible entry needed)

Kingdom visual motifs are already defined in GMU-007 Section 2. Example for a Kasar Dutse banner motif:

> Use canvas-design to create a banner/sigil design for the Kingdom of Kasar Dutse: crossed-spear motif, deep red (#7A2323) and iron-grey (#5C5F62) on black (#1C1B19), minimal ornamentation, defensive/martial and honor-code austere rather than decorative. Flat design suitable for a banner or wax-seal.

---

## 2. Tool B — `algorithmic-art` (built in, use for patterns/textures/backgrounds)

**What it actually does:** generates original generative/code-based art (flow fields, particle systems, geometric pattern systems) — not photoreal, not portraiture. Good for abstract or pattern-based visuals.

**Best for in GMU:** repeating geometric tile/lattice patterns for Zamar architecture references, abstract kingdom-color background textures for marketing/pitch materials, decorative dividers for documents, title-card background textures for the interactive comic or a future title sequence.

**Not for:** characters, locations, anything representational — it will not produce a face or a building.

### Step by step

1. Type:

   > Use the algorithmic-art skill to generate a geometric lattice pattern in Zamar's colors (indigo #2E3A6E, gold #C9A24B, off-white #F4EFE4) — inspired by Islamic-scholarly architectural tile work per GMU-002/GMU-306 (Architecture Bible). I want it as a seamless-feeling background texture.

2. I'll build it and show you a preview. You can ask for parameter tweaks in plain language ("denser pattern," "less gold, more indigo," "slower/calmer motion if animated").
3. Confirm, then ask me to save it — same save flow as Section 4.

---

## 3. Tool C — Adobe for creativity (MCP connector, not yet connected — optional)

This is a separate class of tool from A and B: it's a **connector** to Adobe's actual creative apps/services (asset creation, brand-color-theme tools, animation), not a skill built into me. It requires a one-time authorization step before I can use it at all.

**When to bother connecting it:** only if you specifically want Adobe-ecosystem output (e.g., files that open directly in Photoshop/Illustrator/Firefly-based workflows, or you're already using Adobe tools for GMU's brand assets). If canvas-design and algorithmic-art already cover what you need, you can skip this entirely.

### How to connect it (do this yourself — I cannot do this step for you)

1. Open the Claude app.
2. Go to **Settings → Capabilities**.
3. Find **"Adobe for creativity"** in the connector list and click **Connect**.
4. You'll be sent through Adobe's own login/authorization screen — sign in with your Adobe account and approve the permissions Adobe asks for. This happens entirely on Adobe's site; I never see your Adobe password.
5. Come back to this chat and say "Adobe is connected" — I'll verify and start using it.

### How to use it once connected

Same golden-rule pattern as Tool A: pull the prompt/description from the character sheet or location brief first, then ask, e.g.:

> Using the Adobe connector, create a brand-aligned asset for [character/location] using this description: [paste from the bible]. Check it against our brand color theme first.

I'll call `asset_get_brand` / `asset_get_brand_color_themes` first to confirm it's reading the right palette, then generate.

---

## 4. Where Finished Images Actually Go

Follow GMU-006's existing naming convention exactly, so future video-generation steps can find the "locked" reference without confusion:

- **Character art** → save inside `05_CHARACTER_BIBLE/AI_MODEL_LIBRARY/`, named `<CharacterName>_REFERENCE_v1.png` (e.g., `Fatima_bint_Adamu_REFERENCE_v1.png`). If it's a poster/illustrative piece rather than a strict reference turnaround, name it `<CharacterName>_ILLUSTRATION_v1.png` instead so it's clear it's not the locked production reference.
- **Location art** → save inside `19_CONCEPT_ART/`, named `<LocationID>_REFERENCE_v1.png` (e.g., `GMU-501_RiverPort_REFERENCE_v1.png`) or `_ILLUSTRATION_v1.png` for non-reference pieces.
- **Sigils, patterns, marketing/pitch art** → save inside `22_MARKETING/` or `23_PITCH/` depending on purpose, or `25_BRAND/` only once GMU-002 is formally Approved (it's currently Draft, so nothing goes there yet — see the folder's own README).

Just tell me "save that to [folder]" or "save that as the reference for Fatima" and I'll place it correctly and confirm the exact path back to you — you don't need to move files yourself.

---

## 5. Full Worked Example, Start to Finish

Say you want a first illustrative portrait of Malik ibn Adamu.

1. **Find the source material.** I open `05_CHARACTER_BIBLE/AI_MODEL_LIBRARY/Malik_ibn_Adamu_assets.md` and pull the "AI Image Generation Prompt" paragraph. (You can also just ask me: "pull Malik's image prompt from his character sheet" — I'll fetch it for you, you don't have to open the file yourself.)
2. **Ask for the image**, in plain language:

   > Create an illustrative portrait of Malik using canvas-design. Pull his description from his character sheet and match it exactly. Zamar palette, dignified, not warlike.

3. **I generate it and show you the result** in this chat.
4. **You react in plain language:** "good likeness, but make the robe richer/more formal" or "approved."
5. **I save it** once you confirm, at `05_CHARACTER_BIBLE/AI_MODEL_LIBRARY/Malik_ibn_Adamu_ILLUSTRATION_v1.png`, and tell you the exact path.

That's the entire loop — find the existing description, ask in plain language, react, confirm, save. You never need to write a prompt from nothing, and you never need to touch a file path yourself unless you want to.

---

## 6. Quick Reference — Which Tool for Which Job

| You want... | Use |
|---|---|
| A single strong character portrait or poster | canvas-design |
| A single strong location illustration | canvas-design |
| A repeating pattern, texture, or abstract background | algorithmic-art |
| A kingdom sigil, banner, or wax-seal motif | canvas-design |
| Adobe-native files / Photoshop-Illustrator-Firefly workflow | Adobe connector (must connect first) |
| A **locked, photoreal, multi-angle reference** for video generation | Neither — follow GMU-006 Section 2 (Midjourney/FLUX, external, outside this chat) |
| Video/motion generation | Neither — GMU-006 Section 4 (Kling/Veo) |
| Voice casting | Neither — GMU-006 Section 3 (ElevenLabs) |
| Music/score | Neither — GMU-006 Section 5 (Suno/ElevenLabs Music) |

## Status

Draft — first version. Practical companion to GMU-006/GMU-007, written for zero prior tool experience. Update this file if canvas-design/algorithmic-art capabilities change, or once the Adobe connector is actually connected and its real output quality has been evaluated against GMU's photoreal bar.
