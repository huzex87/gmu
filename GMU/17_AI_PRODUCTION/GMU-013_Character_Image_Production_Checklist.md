Document ID: GMU-013
Document Name: Character Image Production Checklist — Ready-to-Paste
Classification: Reference (Production Asset / Staff Handoff Packet)
Version: 1.0
Status: In Progress
Owner: Huzaifa Yakub
Last Edited: 2026-07-12
Canon Status: N/A
Approval Status: Pending
Dependencies: GMU-005 (Character Bible), GMU-007 (Prompt Library), GMU-006 (AI Production Bible), GMU-012 (Zero-Experience Execution Guide)

---

# GMU-013 — Character Image Production Checklist

**Hand this document to whoever is generating character reference images.** Every prompt below is already fully assembled — the character's design-sheet description plus GMU-007's master style block, combined and ready to paste exactly as written. No editing, no lookups, no decisions required. Work top to bottom; the order is the project's actual priority order. Check off each character as you lock their reference.

## Before You Start

1. Account needed: Midjourney (Standard plan) — see GMU-012 Part A for signup. FLUX is an acceptable substitute; see the note at the end of this document.
2. Every prompt below already ends with the master style block. Do not add your own extra description — if a result doesn't look right, regenerate with the same prompt rather than rewriting it, so every character stays traceable to one exact source prompt.
3. **Universal negative prompt** — add this to every single generation (in Midjourney, append `--no` followed by this list; in FLUX, use it as the negative-prompt field):
   > no anachronistic clothing or technology, no modern text or logos, no generic "fantasy Africa" tropes, no orientalist exoticization, no exaggerated or caricatured facial features, no inconsistent character faces between shots, no morphing or warping artifacts, no oversaturated or cartoonish color grading

## The Procedure (identical for every character below)

1. Copy the character's **PROMPT TO PASTE** block exactly as written.
2. Paste into Midjourney's generation box. Add the universal negative prompt from above (`--no ...`).
3. Press Enter. Wait for the 4-image grid.
4. Pick the strongest result. Click it → **Upscale**.
5. Right-click the upscaled image → **Save image as...** → save to your computer.
6. Rename the saved file to the **EXACT FILENAME** given for that character.
7. Move/copy the renamed file into the **EXACT FOLDER** given (all characters save into the same folder: `05_CHARACTER_BIBLE/AI_MODEL_LIBRARY/`).
8. Copy the image's URL in Midjourney (right-click the image → Copy Link) and paste it into the **LOCK URL** line at the bottom of that character's entry below — you'll need this for every future generation of the same character (see "Locking Consistency" below).
9. Check the box, move to the next character.

## Locking Consistency (do this after every character's first accepted image)

For any *future* image of the same character (a different pose, a different chapter's scene, a variant costume), take that character's base prompt below, add whatever new detail you need (e.g., a variant note already provided), then append:
`--cref [the LOCK URL you saved in step 8] --cw 90`

This forces Midjourney to hold the character's face and costume steady. Never describe a locked character freehand from memory once you have a LOCK URL.

---

## CHARACTER 1 of 13 — Fatima bint Adamu (GMU-401) — HIGHEST PRIORITY

- [x] Locked — generated 2026-07-13 via Higgsfield (Nano Banana Pro, 4K, image-referenced against the user's approved GMU-401 design sheet, skin tone lightened per director note, wardrobe/signet ring/sash matched exactly)

**PROMPT TO PASTE:**
> Portrait and full-body reference turnaround of a tall, composed West African woman in her late twenties, dark eyes, tight braided hair under a simple indigo headwrap, wearing a floor-length deep indigo scholar's robe with geometric gold trim at cuffs and hem, a gold sash worn diagonally across the chest, minimal jewelry, a single signet ring. Calm, deliberate posture, faint appraising expression. Sahel-inspired royal-scholarly setting, warm indigo and gold color palette, cinematic lighting, photorealistic, consistent character reference sheet, neutral studio background, front view / three-quarter view / side profile, photorealistic, cinematic quality, natural volumetric lighting, rich but grounded color grading, Sahel-inspired West African aesthetic, culturally specific and respectful detail, sharp fine detail on fabric texture, no anachronistic elements, no modern text or logos.

**EXACT FILENAME:** `Fatima_bint_Adamu_REFERENCE_v1.png`
**EXACT FOLDER:** `05_CHARACTER_BIBLE/AI_MODEL_LIBRARY/`
**LOCK URL (fill in after generating):** Higgsfield job `aa2f817c-1982-458f-b087-1e872bf4038b` (upscaled to 4K via job `a6251237-7ead-44a2-9596-c7b608dd6d57`). Reference this job_id as a `medias` input (role `image`) on any future Higgsfield generation of Fatima to hold her face/costume steady — the Higgsfield equivalent of `--cref`.

**Note on tool substitution:** This checklist was originally written for Midjourney/FLUX. Character 1 was actually produced with the user's connected Higgsfield account instead — model Nano Banana Pro (Google), text+image-referenced generation, 4 review options generated then the user's pick upscaled to 4K. The `--no`/`--cref` Midjourney syntax in these prompts was translated to plain-language negative/consistency instructions for Higgsfield; the underlying creative description was not altered.

**VARIANT — Mourning overlay (Act Two onward, generate second, save separately):**
- [x] Locked (variant) — generated 2026-07-13 via Higgsfield Nano Banana 2 image-edit (job `ecc50e67-3ef5-4418-a35e-13972029948e`, upscaled to 4K via job `d38976e9-5b14-4164-9d5c-7cc55c3fc551`), edited directly from her locked base image for face/costume consistency

**PROMPT TO PASTE (variant):**
> Portrait and full-body reference turnaround of a tall, composed West African woman in her late twenties, dark eyes, tight braided hair under a simple indigo headwrap, wearing a floor-length deep indigo scholar's robe with geometric gold trim at cuffs and hem, a gold sash worn diagonally across the chest, layered under a rough-textured, unbleached off-white mourning wrap over the indigo robe, headwrap uncovered by the wrap's edge, minimal jewelry, a single signet ring. Calm, deliberate posture, faint appraising expression. Sahel-inspired royal-scholarly setting, warm indigo and gold color palette, cinematic lighting, photorealistic, consistent character reference sheet, neutral studio background, front view / three-quarter view / side profile, natural volumetric lighting, rich but grounded color grading, no anachronistic elements, no modern text or logos. --cref [Fatima's LOCK URL from above] --cw 90

**EXACT FILENAME (variant):** `Fatima_bint_Adamu_REFERENCE_v1_mourning.png`
**EXACT FOLDER:** `05_CHARACTER_BIBLE/AI_MODEL_LIBRARY/`

---

## CHARACTER 2 of 13 — Malik ibn Adamu (GMU-402) — HIGHEST PRIORITY

- [x] Locked — generated 2026-07-13 via Higgsfield (Nano Banana Pro base, then Nano Banana 2 image-edit pass to add princely regalia — signet ring with Zamar sigil, house-crest collar pin, gold cord shoulder trim, edge-piping — matching Fatima's established heraldic language, per director note)

**PROMPT TO PASTE:**
> Portrait and full-body reference turnaround of a West African man in his mid-twenties, athletic cavalry-officer build, close-cropped hair, small training scars on the knuckles and jaw, warm and open expression. Wearing practical dust-colored leather training gear with forearm guards. Second variant: dark Zamar cavalry command tunic with gold braid at shoulders and cuffs. Sahel-inspired military setting, warm lighting, photorealistic, consistent character reference sheet, neutral studio background, front view / three-quarter view / side profile, cinematic quality, natural volumetric lighting, rich but grounded color grading, Sahel-inspired West African aesthetic, sharp fine detail on fabric texture, no anachronistic elements, no modern text or logos.

**EXACT FILENAME:** `Malik_ibn_Adamu_REFERENCE_v1.png`
**EXACT FOLDER:** `05_CHARACTER_BIBLE/AI_MODEL_LIBRARY/`
**LOCK URL:** Final regalia'd version: Higgsfield job `f56229d4-18f3-4499-80a8-2cd31ce82c53` (upscaled to 4K via job `f400d09a-4d79-4cb3-96cb-0480bfc4664b`). This is the canonical file, edited from base job `11309ccb-372e-4134-b10d-07f8dc15a7cf`. Reference the final job_id as a `medias` input (role `image`) on any future generation of Malik to hold his face/costume/regalia steady.

**VARIANT — Mourning wrap + red sash (Act Two onward):**
- [x] Locked (variant) — generated 2026-07-13 via Higgsfield Nano Banana 2 image-edit (job `8ac83812-be49-4432-9fc1-ace35d5558a5`, upscaled to 4K via job `48cea261-beda-4dba-8e59-e007d1310037`), edited directly from his locked regalia'd base image for face/costume consistency

**PROMPT TO PASTE (variant):**
> Portrait and full-body reference turnaround of a West African man in his mid-twenties, athletic cavalry-officer build, close-cropped hair, small training scars on the knuckles and jaw. Wearing dark Zamar cavalry command tunic with gold braid at shoulders and cuffs, layered under a rough-textured, unbleached off-white mourning wrap over the cavalry tunic, a single narrow red sash crossing the chest. Sahel-inspired military setting, warm lighting, photorealistic, consistent character reference sheet, neutral studio background, front view / three-quarter view / side profile, no anachronistic elements, no modern text or logos. --cref [Malik's LOCK URL from above] --cw 90

**EXACT FILENAME (variant):** `Malik_ibn_Adamu_REFERENCE_v1_mourning.png`
**EXACT FOLDER:** `05_CHARACTER_BIBLE/AI_MODEL_LIBRARY/`

---

## CHARACTER 3 of 13 — Elder Bashir (GMU-407) — HIGHEST PRIORITY (episode's emotional pivot)

- [x] Locked — generated 2026-07-13 via Higgsfield (Nano Banana Pro base, then Nano Banana 2 image-edit pass to elevate him to a royal elder statesman look — Hausa-style rawani turban, richer embroidered robe, ring, and a ceremonial pendant of Diwan rank — per director note)

**PROMPT TO PASTE:**
> Portrait and full-body reference turnaround of an elderly West African man in his seventies, gentle warm eyes, neat white beard, slightly stooped posture, moves slowly. Wearing unornamented muted warm-toned Diwan scholar's robes with no rank sash. Sahel-inspired scholarly setting, warm candlelit interior lighting, photorealistic, consistent character reference sheet, neutral studio background, front view / three-quarter view / side profile, cinematic quality, natural volumetric lighting, rich but grounded color grading, Sahel-inspired West African aesthetic, sharp fine detail on fabric texture, no anachronistic elements, no modern text or logos.

**EXACT FILENAME:** `Elder_Bashir_REFERENCE_v1.png`
**EXACT FOLDER:** `05_CHARACTER_BIBLE/AI_MODEL_LIBRARY/`
**LOCK URL:** Final royal-elder version: Higgsfield job `53478cac-46a5-4a17-a9ef-85dd31bd448d` (upscaled to 4K via job `14fa149d-a548-4e41-897a-6bb2b5966c0f`). This is the canonical file, edited from base job `1ff1c313-f004-4417-88d3-3ecd51391fe6`. Reference the final job_id as a `medias` input (role `image`) on any future generation of Bashir (including the death-scene variant, which should probably drop the turban/regalia for the somber staging — director's call) to hold his face steady.

**VARIANT — Death-scene staging (Act Four, generate second):**
- [x] Locked (variant) — generated 2026-07-13 via Higgsfield Nano Banana 2 image-edit (job `4fb031ac-b421-41eb-abc8-eae49169dca8`, upscaled to 4K via job `3ed51978-e63d-4a04-8db0-7d80d4c95076`), edited from his locked royal-elder base image with the turban/ceremonial pendant removed for this private, non-ceremonial scene (director's call, per note above)

**PROMPT TO PASTE (variant):**
> Elderly West African man in his seventies, neat white beard, slumped forward peacefully over a desk, unornamented muted warm-toned Diwan scholar's robes. Cold dawn light through a window, an overturned inkwell as the only visible disturbance in frame, non-graphic and respectful staging, quiet and still, photorealistic, cinematic, no anachronistic elements, no modern text or logos, no gratuitous graphic detail. --cref [Bashir's LOCK URL from above] --cw 85

**EXACT FILENAME (variant):** `Elder_Bashir_REFERENCE_v1_deathscene.png`
**EXACT FOLDER:** `05_CHARACTER_BIBLE/AI_MODEL_LIBRARY/`

---

## CHARACTER 4 of 13 — King Garba Ironhand (GMU-403) — HIGH PRIORITY

- [ ] Locked

**SPECIAL GUARDRAIL — read before generating:** resist any "warlord" caricature. He should read as dignified and restrained, not menacing. If a result looks aggressive/villainous, regenerate — do not accept it.

**PROMPT TO PASTE:**
> Portrait and full-body reference turnaround of a weathered West/Central African man in his mid-fifties, grey-streaked short beard, old scar through the left eyebrow, solid heavyset build, standing with total stillness and quiet authority. Wearing deep red and iron-grey layered garments with minimal ornament, a small crossed-spear pin at the collar, a heavy iron-grey cloak. Windswept mountain fortress setting, overcast dramatic lighting, photorealistic, consistent character reference sheet, neutral studio background, front view / three-quarter view / side profile, dignified and restrained not menacing, cinematic quality, natural volumetric lighting, rich but grounded color grading, sharp fine detail on fabric texture, no anachronistic elements, no modern text or logos, no caricatured or villainous facial features.

**EXACT FILENAME:** `Garba_Ironhand_REFERENCE_v1.png`
**EXACT FOLDER:** `05_CHARACTER_BIBLE/AI_MODEL_LIBRARY/`
**LOCK URL:** _______________________________

---

## CHARACTER 5 of 13 — Speaker Amina Bello Kwarafi (GMU-404) — HIGH PRIORITY

- [ ] Locked

**PROMPT TO PASTE:**
> Portrait and full-body reference turnaround of a composed West African woman in her mid-forties, straight-backed, understated but clearly expensive tailored emerald and white clothing with a subtle sheen, minimal fine-metalwork jewelry, a small silver river-fish pin at the collar, neat controlled hairstyle, pleasant unreadable expression. Sahel-inspired merchant-aristocrat setting, cool clean lighting, photorealistic, consistent character reference sheet, neutral studio background, front view / three-quarter view / side profile, cinematic quality, natural volumetric lighting, rich but grounded color grading, sharp fine detail on fabric texture, no anachronistic elements, no modern text or logos.

**EXACT FILENAME:** `Amina_Bello_Kwarafi_REFERENCE_v1.png`
**EXACT FOLDER:** `05_CHARACTER_BIBLE/AI_MODEL_LIBRARY/`
**LOCK URL:** _______________________________

---

## CHARACTER 6 of 13 — Yusuf al-Kanem (GMU-405) — HIGH PRIORITY

- [ ] Locked

**SPECIAL GUARDRAIL — read before generating:** resist any AI tool's tendency to add "mysterious" or "sinister" visual flourishes — shadowed lighting, narrowed eyes, dramatic framing. He must look ordinary and trustworthy, even slightly more reassuring than average. If a result looks even slightly villainous or mysterious, regenerate.

**PROMPT TO PASTE:**
> Portrait and full-body reference turnaround of a middle-aged West African man in his fifties, deliberately unremarkable and forgettable features, medium build, neutral well-groomed appearance, soft reassuring expression. Wearing plain Zamar court dress in muted grey-blue and brown tones with no rank ornamentation. Sahel-inspired palace administrative setting, flat even lighting (deliberately less dramatic than other character portraits), photorealistic, consistent character reference sheet, neutral studio background, front view / three-quarter view / side profile, ordinary and trustworthy not sinister, no shadowed or dramatic lighting, no anachronistic elements, no modern text or logos.

**EXACT FILENAME:** `Yusuf_al-Kanem_REFERENCE_v1.png`
**EXACT FOLDER:** `05_CHARACTER_BIBLE/AI_MODEL_LIBRARY/`
**LOCK URL:** _______________________________

---

## CHARACTER 7 of 13 — Queen Mother Halima (GMU-411) — HIGH PRIORITY

- [ ] Locked

**PROMPT TO PASTE:**
> Portrait and full-body reference turnaround of a composed West African woman in her mid-fifties, upright bearing, warm but exacting expression, dark eyes with fine lines suggesting both grief and control. Wearing restrained deep indigo robes with muted gold trim, mourning-adjacent tones, minimal royal ornamentation compared to ceremonial court dress. Sahel-inspired royal setting, soft even lighting, photorealistic, consistent character reference sheet, neutral studio background, front view / three-quarter view / side profile, cinematic quality, natural volumetric lighting, rich but grounded color grading, no anachronistic elements, no modern text or logos.

**EXACT FILENAME:** `Halima_REFERENCE_v1.png`
**EXACT FOLDER:** `05_CHARACTER_BIBLE/AI_MODEL_LIBRARY/`
**LOCK URL:** _______________________________

**VARIANT — Episode 6 public-address (generate second):**
- [ ] Locked (variant)

**PROMPT TO PASTE (variant):**
> Composed West African woman in her mid-fifties, upright bearing, wearing restrained deep indigo robes with muted gold trim, a simple unadorned gold circlet, more structured robe silhouette, standing on a raised dais addressing a crowd, composed public bearing, warm even daylight, photorealistic, cinematic, no anachronistic elements, no modern text or logos. --cref [Halima's LOCK URL from above] --cw 90

**EXACT FILENAME (variant):** `Halima_REFERENCE_v1_publicaddress.png`
**EXACT FOLDER:** `05_CHARACTER_BIBLE/AI_MODEL_LIBRARY/`

---

## CHARACTER 8 of 13 — High Cleric Nafisa (GMU-413) — MEDIUM-HIGH PRIORITY

- [ ] Locked

**SPECIAL GUARDRAIL — read before generating:** do NOT default her costume to Zamar's indigo/gold. The Faith of the Covenant is visually independent of all three kingdoms — use only the neutral tones specified below.

**PROMPT TO PASTE:**
> Portrait and full-body reference turnaround of an austere, dignified West African woman in her sixties, upright bearing, calm precise expression, deep-set thoughtful eyes. Wearing unornamented formal Islamic scholarly robes in deep neutral tones (off-white, soft grey, muted olive) with understated geometric embroidery, distinct from any royal court's colors — no indigo, no gold, no kingdom-specific palette. Sahel-inspired religious/scholarly setting, soft dignified lighting, photorealistic, consistent character reference sheet, neutral studio background, front view / three-quarter view / side profile, no anachronistic elements, no modern text or logos, no invented religious iconography not grounded in real Islamic visual tradition.

**EXACT FILENAME:** `High_Cleric_Nafisa_REFERENCE_v1.png`
**EXACT FOLDER:** `05_CHARACTER_BIBLE/AI_MODEL_LIBRARY/`
**LOCK URL:** _______________________________

---

## CHARACTER 9 of 13 — Elder Kamal (GMU-409) — MEDIUM PRIORITY (rises at Chapter/Episode 9)

- [ ] Locked

**PROMPT TO PASTE:**
> Portrait and full-body reference turnaround of a West African man in his sixties, composed and exacting, neatly groomed beard, upright posture, stern default expression with a hint of dry humor. Wearing formal Diwan scholar's robes with visible senior rank trim and a presiding sash. Sahel-inspired university council-chamber setting, warm formal lighting, photorealistic, consistent character reference sheet, neutral studio background, front view / three-quarter view / side profile, cinematic quality, natural volumetric lighting, sharp fine detail on fabric texture, no anachronistic elements, no modern text or logos.

**EXACT FILENAME:** `Elder_Kamal_REFERENCE_v1.png`
**EXACT FOLDER:** `05_CHARACTER_BIBLE/AI_MODEL_LIBRARY/`
**LOCK URL:** _______________________________

---

## CHARACTER 10 of 13 — General Tahir (GMU-408) — MEDIUM PRIORITY

- [ ] Locked

**PROMPT TO PASTE:**
> Portrait and full-body reference turnaround of a West African man in his sixties, hard-featured, greying short hair, economical controlled posture, career-soldier bearing. Wearing senior Zamar cavalry command uniform, dark tunic with heavy gold braid at shoulders and cuffs, older practical cut. Sahel-inspired military command-tent setting, warm interior lighting, photorealistic, consistent character reference sheet, neutral studio background, front view / three-quarter view / side profile, cinematic quality, natural volumetric lighting, no anachronistic elements, no modern text or logos.

**EXACT FILENAME:** `General_Tahir_REFERENCE_v1.png`
**EXACT FOLDER:** `05_CHARACTER_BIBLE/AI_MODEL_LIBRARY/`
**LOCK URL:** _______________________________

---

## CHARACTER 11 of 13 — Commander Rafiu (GMU-412) — MEDIUM PRIORITY

- [ ] Locked

**PROMPT TO PASTE:**
> Portrait and full-body reference turnaround of a weathered West African man in his late fifties, deep-set eyes, sun-worn skin, the build of a career field soldier rather than a court officer. Wearing plain, visibly worn Zamar cavalry command insignia in muted indigo and faded gold, practical rather than ceremonial. Sahel-inspired military setting, natural outdoor lighting, photorealistic, consistent character reference sheet, neutral studio background, front view / three-quarter view / side profile, sharp fine detail on fabric texture, no anachronistic elements, no modern text or logos.

**EXACT FILENAME:** `Commander_Rafiu_REFERENCE_v1.png`
**EXACT FOLDER:** `05_CHARACTER_BIBLE/AI_MODEL_LIBRARY/`
**LOCK URL:** _______________________________

---

## CHARACTER 12 of 13 — Danladi (GMU-406) — MEDIUM PRIORITY (rises at Chapter/Episode 8)

- [ ] Locked

**PROMPT TO PASTE:**
> Portrait and full-body reference turnaround of a young West African man, 24, wiry build, junior cavalry uniform with minimal insignia, collar open, off-duty and slightly informal, open and searching expression. Sahel-inspired setting, natural daylight, photorealistic, consistent character reference sheet, neutral studio background, front view / three-quarter view / side profile, cinematic quality, natural volumetric lighting, no anachronistic elements, no modern text or logos.

**EXACT FILENAME:** `Danladi_REFERENCE_v1.png`
**EXACT FOLDER:** `05_CHARACTER_BIBLE/AI_MODEL_LIBRARY/`
**LOCK URL:** _______________________________

---

## CHARACTER 13 of 13 — Abubakar (GMU-414) — LOW-MEDIUM PRIORITY (identified Episode/Chapter 7)

- [ ] Locked

**SPECIAL GUARDRAIL — read before generating:** same as Yusuf — resist any "sinister" visual flourishes. He should look warm and slightly anxious, never menacing.

**PROMPT TO PASTE:**
> Portrait and full-body reference turnaround of an unremarkable middle-aged West African man in his forties, plain features, medium build, deferential household-staff bearing with a faint underlying nervousness. Wearing plain Zamar household staff attire, no rank markers or ornamentation. Sahel-inspired palace domestic setting, flat even lighting, photorealistic, consistent character reference sheet, neutral studio background, front view / three-quarter view / side profile, warm and anxious not sinister, no anachronistic elements, no modern text or logos.

**EXACT FILENAME:** `Abubakar_REFERENCE_v1.png`
**EXACT FOLDER:** `05_CHARACTER_BIBLE/AI_MODEL_LIBRARY/`
**LOCK URL:** _______________________________

---

## Background/Incidental Characters (GMU-410) — NO LOCKED REFERENCE NEEDED

These 9 roles (Servant Girl, Rider, Soldier, Messenger, unnamed Generals, War-Captain, Young Clergyman, Steward, Old Woman) each appear in one scene only and do not need a locked reference image. When one of them appears in a Phase 3 video shot, describe them fresh each time using the short description in `05_CHARACTER_BIBLE/AI_MODEL_LIBRARY/Background_and_Incidental_Characters.md` — do not spend Phase 1 budget/time locking these.

---

## When This Checklist Is Complete

All 13 boxes above checked (15 files total counting the 2 variants for Fatima and Malik, plus the death-scene and public-address variants for Bashir and Halima — 17 files total) means Phase 1 characters are done. Hand this document, with all boxes checked, to whoever owns Phase 2 (voice — see GMU-015) and Phase 3 (video — see GMU-016), since both phases require every one of these files to exist first.

**Using FLUX instead of Midjourney:** same prompts, same filenames. Instead of `--cref [URL] --cw 90`, upload your accepted reference image directly as an input reference image in FLUX's playground/API alongside the next prompt.

## Status

Draft — ready to execute. All 13 prompts extracted verbatim from `05_CHARACTER_BIBLE/AI_MODEL_LIBRARY/` and combined with GMU-007's master style block; no new creative decisions were made in assembling this checklist. Fill in LOCK URLs as you go — this document becomes the permanent record of which exact accepted image is canon for each character.
