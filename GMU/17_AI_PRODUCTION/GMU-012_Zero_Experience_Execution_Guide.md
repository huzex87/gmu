Document ID: GMU-012
Document Name: Zero-Experience Execution Guide — External AI Tools
Classification: Reference (Production Asset)
Version: 1.0
Status: In Progress
Owner: Huzaifa Yakub
Last Edited: 2026-07-12
Canon Status: N/A
Approval Status: Pending
Dependencies: GMU-006 (AI Production Bible), GMU-007 (Prompt Library), GMU-005 (Character Bible), GMU-002 (Creative & Brand Bible)

---

# GMU-012 — Zero-Experience Execution Guide

GMU-006 (AI Production Bible) is the strategy document — it tells you *which* tool to use for *which* phase, and *why*, but it assumes you already know how to operate Midjourney, ElevenLabs, Kling, Suno, and DaVinci Resolve. This document assumes you know none of that. It walks every phase of GMU-006's pipeline as literal, ordered, click-level steps: what to sign up for, what to click, what to paste, what to download, and exactly where the result gets saved in this repository.

**One honest caveat before you start:** these are fast-moving commercial products. Exact button labels, menu positions, and pricing can shift between when this was written (July 2026) and when you actually sit down to use them. The account-creation URLs, overall workflow shape, and file conventions below will stay correct even if a specific button has moved — if something looks different from the description, look for the nearest equivalent (e.g., "Generate" might say "Create" instead) rather than assuming the whole step is wrong.

**Do this in order.** Phase 1 (images) must be fully done for all 13 characters + 10 locations before you touch Phase 3 (video) on any chapter — this is GMU-006's single most important sequencing rule, and skipping it is the #1 way projects like this end up with visibly inconsistent characters across episodes.

---

## PART A — Account Setup (do this once, before anything else)

Work through this table top to bottom. Each row is a real account you need to create. Nothing here costs money until you explicitly choose a paid tier during signup — you can create every account first and upgrade only when you reach that phase.

| # | Tool | Sign up at | What it's for | Tier to pick (per GMU-006 §1) |
|---|---|---|---|---|
| 1 | Midjourney | midjourney.com → "Sign Up" | Character/location reference images | Standard plan (monthly) |
| 2 | FLUX (Black Forest Labs) | Either bfl.ai directly, or via a hosting playground like fal.ai or replicate.com (both let you run FLUX models without coding) | Alternative/supplement to Midjourney for images | Pay-as-you-go via the playground you choose — no subscription needed to start |
| 3 | ElevenLabs | elevenlabs.io → "Sign Up" | Voice casting/cloning for dialogue | Creator ($22/mo) — free tier will not work for this project (see GMU-006 §1) |
| 4 | Kling AI | klingai.com → "Sign Up" | Primary video generation tool | Pro tier, pay-per-second |
| 5 | Google Veo | Via Google AI Studio (aistudio.google.com) or Vertex AI — requires a Google account you likely already have | Secondary video tool, for the season's highest-priority shots only | Pay-as-you-go |
| 6 | Suno | suno.com → "Sign Up" | Music/score | Pro or Premier plan — commercial rights require a paid plan (free tier's output cannot be used) |
| 7 | DaVinci Resolve | blackmagicdesign.com/products/davinciresolve → "Download" | Final editing/assembly | Free version (Studio only needed for advanced color tools, not required for Season One) |

**Practical tip for a solo creator on a budget:** you don't need all seven accounts open simultaneously. Create #1 (Midjourney) and #3 (ElevenLabs) first — those are the two phases with the least room to cut costs, and getting them right first protects everything downstream. Add #4/#5 (video) only once Phase 1 images are fully locked, since video is by far the most expensive phase (see GMU-006 §10's cost estimate) and there's no point paying for it before the reference images it depends on exist.

---

## PART B — Phase 1: Character & Location Reference Images

**Goal, in plain terms:** end up with one accepted, "final" image per character (13 of them) and per location (10 of them), saved into this repository with the exact filename convention GMU-006 already defined, so every later tool can reference them.

### B.1 — Generating your first character image (worked example: Fatima)

1. Open `05_CHARACTER_BIBLE/AI_MODEL_LIBRARY/Fatima_bint_Adamu_assets.md` in this repository. Scroll to the section titled **"AI Image Generation Prompt (Reference / Turnaround)"**. Select and copy the entire paragraph starting with "Portrait and full-body reference turnaround of a tall, composed West African woman..."
2. Open Midjourney (midjourney.com, log in, click into the web-based image generator — it no longer requires Discord for most accounts as of 2026, though Discord remains an option if you prefer it).
3. Find the prompt input box (usually a text field near the top or bottom of the screen, often with a "/imagine" placeholder or simply an empty text box with a paper-airplane/arrow send icon).
4. Paste the copied paragraph into that box.
5. Press Enter / click the send icon. Midjourney will generate a grid of 4 images (this takes roughly 30–60 seconds).
6. Look at all 4. Pick the one that best matches: tall build, indigo headwrap, indigo robe with gold trim, calm composed expression, dark eyes. None will be perfect on the first try — that's expected.
7. Click on your chosen image to open it larger, then click the **Upscale** (or "U" / magnifying-glass) option to get the full-resolution version.
8. Right-click the upscaled image → **Save image as...** (or use the app's own Download button if present) → save it to your computer's Downloads folder for now, naming it something you'll recognize, e.g. `fatima_attempt1.png`.

### B.2 — Locking consistency for every future Fatima image

This is the step that prevents her face/costume from drifting between Chapter 1 and Chapter 20.

1. Once you've picked your accepted Fatima image (Step B.1.7), note its image URL in Midjourney (right-click the image → Copy Link, or use the app's "Copy image URL" option).
2. For every future prompt involving Fatima (a different pose, a different chapter's scene), add `--cref [paste the URL you just copied]` to the end of the prompt text, then also add `--cw 90` (character-weight 90 out of 100 — high value means it holds her face/costume very strictly; drop it to `--cw 60` or so only if you deliberately want more variation, e.g., a very different angle).
3. Example: to generate Fatima in her mourning-overlay variant (described lower in her character sheet under "Mourning variant prompt addition"), you'd paste her base prompt + the mourning addition text + `--cref [her locked image URL] --cw 90`.

### B.3 — Renaming and saving into the repository

1. Rename your downloaded file to match GMU-006's convention exactly: `Fatima_bint_Adamu_REFERENCE_v1.png`.
2. Tell me in this chat: "save this image into Fatima's folder" and attach/drop the file into the conversation, or place it directly into `05_CHARACTER_BIBLE/AI_MODEL_LIBRARY/` in your connected GMU folder yourself via File Explorer (drag-and-drop works, since that folder is directly on your computer). Either way works — I can also help verify the filename/location once it's there.
3. If Fatima needs a second locked look (per her sheet's mourning variant), repeat B.1–B.3 but save it as `Fatima_bint_Adamu_REFERENCE_v1_mourning.png` rather than overwriting the base file.

### B.4 — Repeat for the remaining 12 characters and 10 locations

Same process every time, just swap the source file:

- **Characters:** cycle through every file in `05_CHARACTER_BIBLE/AI_MODEL_LIBRARY/` — Malik_ibn_Adamu, Garba_Ironhand, Amina_Bello_Kwarafi, Elder_Kamal, Elder_Bashir, High_Cleric_Nafisa, General_Tahir, Halima, Commander_Rafiu, Danladi, Abubakar, Yusuf_al-Kanem, plus the Background_and_Incidental_Characters file for anyone recurring enough to need a locked look.
- **Locations:** cycle through every file in `19_CONCEPT_ART/` (GMU-501 through GMU-510) — each has its own "AI image prompt" callouts per room/scene within the file. A single location file may need 2–5 separate locked images (e.g., GMU-502 Palace of Zamar covers 7 interior rooms + main gate — each of those needs its own reference).

**Using FLUX instead of/alongside Midjourney (optional):** if you'd rather use FLUX (via fal.ai or replicate.com), the process is the same conceptually — paste the same character-sheet prompt, generate, pick the best result — but the consistency-lock mechanism is different: instead of `--cref`, you upload your accepted reference image directly as an input image alongside your next prompt (FLUX.2/Kontext accepts up to 8–10 reference images at once per GMU-006 §2, which is actually more flexible than Midjourney if you want to lock face + costume + a specific prop simultaneously).

### B.5 — When Phase 1 is "done"

You'll know you're finished with this phase when every file in `AI_MODEL_LIBRARY/` and `19_CONCEPT_ART/` has a matching `_REFERENCE_v1.png` sitting next to it. Don't start Phase 3 (video) before this is fully true — per GMU-006's explicit sequencing rule.

---

## PART C — Phase 2: Voice Casting (ElevenLabs)

### C.1 — First-time setup

1. Log into elevenlabs.io, upgrade to the Creator plan ($22/mo) under Settings → Subscription (this unlocks Professional Voice Cloning, which you need — see GMU-006 §3).
2. Find the **Voice Library** (usually in the left sidebar) — this is ElevenLabs' collection of stock voices you can browse and preview before committing to any character.

### C.2 — Casting a character (worked example: Fatima)

1. Open `05_CHARACTER_BIBLE/AI_MODEL_LIBRARY/Fatima_bint_Adamu_assets.md`, scroll to **"Voice Direction"** — read it (measured pace, low-to-mid register, minimal vocal fry, controlled precision under anger, reserved warmth).
2. In ElevenLabs' Voice Library, use the filter/search options (gender, age, accent if available) to narrow down candidates, then click through 3–5 stock voices and use the built-in preview player (type a test sentence, hit play) to audition each against Fatima's direction notes.
3. Once you find a strong match, click **Add to my voices** (or equivalent) — this makes it available for generation.
4. If you have an actual voice actor's recorded sample and the rights to use it, instead go to **Voice Lab → Create Voice → Professional Voice Cloning**, upload the required training audio (ElevenLabs will tell you the minimum amount — expect this to be more than IVC required), and wait for training to complete (can take from minutes to a day or more depending on ElevenLabs' current PVC queue).

### C.3 — Log the binding immediately

This step is easy to skip and expensive to skip. As soon as you've picked Fatima's final voice:

1. Open `18_PROMPTS/GMU-007_Prompt_Library.md`, find **Section 7 (Voice Generation Prompts / Direction Templates)**.
2. Fill in the template for Fatima: her name, the Character Bible reference, the actual ElevenLabs Voice ID (found on the voice's detail page in ElevenLabs, usually a string of letters/numbers you can copy), the base Stability/Similarity/Style settings you used, and a one-line summary of her direction.
3. Tell me the details and I'll write this update into GMU-007 for you, so it's recorded permanently rather than living only in your memory or in ElevenLabs' own interface.

### C.4 — Generating actual dialogue lines

1. Open the relevant chapter's screenplay, e.g. `06_SEASON_ONE/CHAPTER_01/Chapter_01_Screenplay.md`.
2. For each of Fatima's lines in that chapter, go to ElevenLabs' **Text to Speech** page, select her locked voice, paste the line, adjust Stability/Similarity/Style sliders to match the scene's emotional beat (per the Voice Direction notes — e.g., "slightly more clipped precision" for the Amina negotiation scene), generate, and download the audio clip.
3. Repeat C.1–C.4 for all 13 principal/recurring characters. Background/incidental one-scene characters (GMU-410) can use faster Instant Voice Cloning or an unmodified stock voice — full PVC casting is only required for recurring cast.

---

## PART D — Phase 3: Shot-by-Shot Video Generation (the expensive phase)

Don't start this until Part B is fully complete for all characters and locations appearing in the chapter you're about to work on.

### D.1 — Find your shot list

1. Open `20_STORYBOARDS/CHAPTER_01/Chapter_01_Shot_List.md` (or whichever chapter you're starting with — GMU-006 recommends starting with Chapters 01–02, since they're the most heavily detailed).
2. Each row in that table describes one shot: its type (wide/medium/close), a description, and which characters/locations appear in it.

### D.2 — Generating one shot (Kling, recommended default)

1. Log into klingai.com, and locate the video generation workspace (usually labeled something like "Create" or "Generate").
2. Find **Elements** (Kling 3.0's character/reference-consistency feature) and upload the locked reference image(s) for every character and the location appearing in this specific shot — e.g., Fatima's `_REFERENCE_v1.png` plus the relevant `19_CONCEPT_ART` location reference.
3. In the prompt box, combine: the shot's Type/Description from the shot list table + GMU-007 Section 1's master style block (still-image version if generating a still, video-motion version if generating motion) + GMU-002's kingdom-specific lighting language for that scene's location (warm lattice-light for Zamar, cold stone-light for Kasar Dutse, etc., per GMU-007 Section 6).
4. Set the clip duration (Kling typically offers preset lengths, e.g. 5s/10s) matching what the shot list implies for that shot.
5. Click **Generate**. This costs money per second of output (~$0.168/sec on Kling 3.0 Pro) — Kling will show you the cost before you confirm.
6. Once generated, watch it back immediately. Compare it against the previous shot in the same scene (GMU-006 Step 3.2) — check the character's face, costume, and the location's colors haven't drifted.
7. If it looks right: download it, name it per convention `Chapter_01_Shot_<scene>.<shot>_v1.mp4` (matching the row/shot number from the shot list table), and save it — see Part D.4 below for where.
8. If it looks wrong: regenerate with an adjusted prompt (tighten the reference weight, re-describe the drifted detail) before moving to the next shot — don't let a bad shot sit and hope editing will fix it later.

### D.3 — Using Veo instead, for high-priority shots only

For the specific shots each chapter's Production Notes flag as highest-priority (e.g., Chapter 01's Teaser, the Chapter 19–20 coronation):

1. Go to Google AI Studio (aistudio.google.com) or Vertex AI, find Veo 3.1's generation interface.
2. Use its **"Ingredients to Video"** feature — it accepts up to 3 reference images at once (character + location + a key prop, e.g., Yusuf's signet), so you can lock all three in a single generation call.
3. Same prompt-construction approach as D.2.3. Veo costs more per second (~$0.40/sec) but currently leads on prompt adherence and native 4K — reserve it for shots where that difference actually matters to the finished product.

### D.4 — Where finished video clips go

There's no dedicated media folder for this yet in the repository — create one the first time you need it: inside each chapter's folder, e.g. `06_SEASON_ONE/CHAPTER_01/RENDERS/`, and save clips there named `Chapter_01_Shot_<scene>.<shot>_v1.mp4` per GMU-006 §9's naming convention. Tell me when you're ready to start Phase 3 and I'll create the `RENDERS/` subfolder structure for every chapter in advance so you're not creating folders mid-workflow.

### D.5 — Order to work in

Per GMU-006 §4: Chapters 01–02 first, then Chapters 19–20 (the finale), then the rest in story order. Within each chapter, generate the Production-Notes-flagged priority shots first, in case you run out of time or budget partway through.

---

## PART E — Phase 4: Music and Sound Design (Suno)

1. Log into suno.com, confirm you're on Pro or Premier (commercial rights requirement — GMU-006 §1).
2. Open `18_PROMPTS/GMU-007_Prompt_Library.md`, Section 8 — pick the mood/kingdom description matching the scene you're scoring (e.g., "Zamar theme: contemplative, string and wind instrumentation...").
3. In Suno's generation box, paste that description as your style/prompt input, and describe the specific cue length/purpose (e.g., "40-second contemplative cue for a quiet council scene, no vocals, fading out").
4. Generate (Suno typically gives you 2 variations per generation). Listen to both, pick the stronger one.
5. Download the audio file (Suno has a Download option on each generated track, usually MP3 or WAV).
6. Save it into `21_SOUNDTRACK/`, named descriptively, e.g. `Chapter_01_Zamar_Council_Cue_v1.mp3`.
7. Generate per-scene or per-chapter cues rather than one long score (GMU-006 §5's explicit recommendation) — this lets you swap one cue later without regenerating everything.
8. Optional: try the same prompt in ElevenLabs Music (elevenlabs.io → Music, if available on your plan) as a comparison, especially useful later if you need to edit just one section of an accepted cue (its Inpainting feature can fix a single bar without full regeneration).

---

## PART F — Phase 5: Editing and Assembly (DaVinci Resolve)

1. Download and install DaVinci Resolve free tier from blackmagicdesign.com.
2. Open it, click **New Project**, name it after the chapter, e.g. "GMU Chapter 01."
3. Go to the **Media** tab, import every clip from that chapter's `RENDERS/` folder (drag-and-drop from your file explorer into Resolve's Media Pool works) plus the dialogue clips from Part C and music cues from Part E.
4. Switch to the **Edit** tab, drag your video clips onto the timeline **in screenplay order** (not necessarily the order you generated them in — check `Chapter_01_Screenplay.md` for correct scene order).
5. Add audio layers in this priority: dialogue first (never let music/ambience obscure a spoken line), then music underneath, then sound design/ambience on top of that as a light layer.
6. Switch to the **Color** tab for a grading pass per scene — match each location's established palette (GMU-002 §11 and the specific GMU-50X brief for that location): warm amber tones for Zamar scenes, harsher cooler overcast tones for Kasar Dutse, reflected water-light for Kwara, clear unshadowed light for Covenant/Sanctuary scenes. AI-generated shots vary in color temperature even from identical prompts, so this pass is what actually locks the look consistent.
7. Apply title cards only once you have real cut footage to design against (GMU-002 §14 — compass-rose reveal, palette-cycling background).
8. Export via the **Deliver** tab once the chapter is fully assembled and graded.

---

## PART G — Phase 6: Quality Gate (before calling a chapter finished)

Before moving on to the next chapter, check the finished cut against GMU-001 §12's bar. Watch it once specifically looking for:

- Character faces/costumes staying consistent shot to shot (the single most common failure point)
- Consistent architecture and color language per location
- Clear narrative — does a first-time viewer understand what's happening without the screenplay in hand
- Distinct character voices — can you tell who's speaking without seeing them

Do this per chapter, every time — chapters produced early (when your reference images and prompt technique were newest/least refined) are exactly where drift is most likely to have crept in unnoticed.

---

## PART H — Your Actual First Day: A Concrete Checklist

If you want to start today with the smallest possible first step, do exactly this, in order:

1. Create a Midjourney account and subscribe to Standard.
2. Open `05_CHARACTER_BIBLE/AI_MODEL_LIBRARY/Fatima_bint_Adamu_assets.md`, copy her image prompt.
3. Generate, upscale, and download your best result (Part B.1).
4. Rename it `Fatima_bint_Adamu_REFERENCE_v1.png` and get it into `05_CHARACTER_BIBLE/AI_MODEL_LIBRARY/` — either drag it in yourself via File Explorer, or drop it into this chat and ask me to place it.
5. Come back and tell me how it looks — I'll help you evaluate it against her character sheet's description and decide whether to lock it or regenerate.

That one image is Fatima done for the entire season. Repeat for the other 12 characters and 10 locations at whatever pace suits you — there's no rush on Phase 1 beyond finishing it before Phase 3 starts.

---

## Quick Reference — Full Pipeline at a Glance

| Phase | Tool | Where prompts come from | Where output is saved |
|---|---|---|---|
| 1. Images | Midjourney / FLUX | `AI_MODEL_LIBRARY/*.md`, `19_CONCEPT_ART/*.md` | Same folders, `<name>_REFERENCE_v1.png` |
| 2. Voice | ElevenLabs | `AI_MODEL_LIBRARY/*.md` → Voice Direction section | Voice ID logged in `GMU-007 §7`; audio clips wherever you're staging them for editing |
| 3. Video | Kling / Veo | `20_STORYBOARDS/CHAPTER_XX/*.md` + locked Phase 1 images | `06_SEASON_ONE/CHAPTER_XX/RENDERS/` (create as needed) |
| 4. Music | Suno / ElevenLabs Music | `GMU-007 §8` | `21_SOUNDTRACK/` |
| 5. Editing | DaVinci Resolve | All of the above, per chapter | Exported chapter file (destination up to you — e.g. `27_ARCHIVE/` or your own export location) |
| 6. Quality Gate | — (manual review) | `GMU-001 §12` | — |

## Status

Draft — first version, written as the literal click-level companion to GMU-006's strategy-level pipeline. Update this document the first time you actually run through Part B end-to-end — real UI details (exact button names, current Midjourney web-app layout, etc.) should be corrected here based on what you actually see, since these products update their interfaces faster than this document can be kept current from research alone.
