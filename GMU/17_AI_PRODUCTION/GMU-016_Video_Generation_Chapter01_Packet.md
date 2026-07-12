Document ID: GMU-016
Document Name: Video Generation Master Procedure + Chapter 01 Full Shot Packet
Classification: Reference (Production Asset / Staff Handoff Packet)
Version: 1.0
Status: In Progress
Owner: Huzaifa Yakub
Last Edited: 2026-07-12
Canon Status: N/A
Approval Status: Pending
Dependencies: GMU-013 + GMU-014 (must be 100% complete first), GMU-015 (must be complete before adding dialogue), GMU-007, GMU-771 (Chapter 01 Shot List)

---

# GMU-016 — Video Generation: Procedure + Chapter 01 Full Packet

**Hand this document to whoever owns video generation.** Do not start until GMU-013 (all 13 characters locked) and GMU-014 (all 28 locations locked) are 100% checked off — every shot below assumes those reference images already exist at the exact filenames given in those two documents.

Chapter 01 below is fully worked — every one of its 24 shots has a complete, ready-to-paste prompt, the exact reference images to feed the tool, and the exact output filename. This is your template. Section 3 at the bottom gives the exact mechanical formula to build the same kind of packet for Chapters 02–20 yourself, pulling directly from each chapter's own shot list in `20_STORYBOARDS/`.

## Before You Start

1. Create a Kling AI account (klingai.com), Pro tier, pay-per-second.
2. Optional: Google AI Studio / Vertex AI account for Veo 3.1 (only needed for the handful of shots flagged HIGH PRIORITY below).
3. Create the output folder now: `06_SEASON_ONE/CHAPTER_01/RENDERS/` (create the same `RENDERS/` subfolder inside every chapter folder as you get to it).
4. Universal negative prompt — apply to every generation:
   > no anachronistic clothing or technology, no modern text or logos, no generic "fantasy Africa" tropes, no exaggerated or caricatured facial features, no inconsistent character faces between shots, no morphing or warping artifacts, no oversaturated or cartoonish color grading, no gratuitous graphic violence

## The Procedure (identical for every shot below)

1. Open Kling's generation workspace, find **Elements** (character/reference-consistency feature).
2. Upload every file listed under **FEED THESE REFERENCE IMAGES** for that shot (from `05_CHARACTER_BIBLE/AI_MODEL_LIBRARY/` and `19_CONCEPT_ART/` — all locked in GMU-013/GMU-014).
3. Paste the **PROMPT TO PASTE** exactly as written into the prompt box.
4. Add the universal negative prompt.
5. Set clip duration matching the shot's scale (short/punchy for CU/INSERT shots — 3–5s; longer for WS/EST shots with camera movement — 5–10s).
6. Click Generate. Review immediately — compare against the previous shot in the same scene for face/costume/color drift.
7. If good: download, save as the **EXACT FILENAME** into `06_SEASON_ONE/CHAPTER_01/RENDERS/`. If drifted: regenerate before moving on.
8. Check the box, move to the next shot.

---

# CHAPTER 01 — "The Sultan's Silence" — Full Shot Packet (24 shots, 7 scenes)

## SCENE 1 — EXT. Birnin Zamar, River Port — Pre-Dawn (3 shots, no characters)

**FEED THESE REFERENCE IMAGES (all 3 shots in this scene):** `GMU-501_RiverPort_REFERENCE_v1.png`

### Shot 1.1 (EST WS)
- [ ] Done
**PROMPT TO PASTE:** Wide establishing shot, camera slowly drifting forward over calm water: misty pre-dawn river port in a Sahel-inspired capital city, fishing boats with lantern-lit bows working the water, city skyline in silhouette behind — domes, terraced white university walls, gold-tipped market minarets — a distant palace with one lit window high up. Warm lantern light against cool blue pre-dawn tones, atmospheric mist, cinematic, photorealistic, smooth natural motion, consistent lighting direction throughout the shot, 24fps film-like motion, no morphing or flickering artifacts.
**EXACT FILENAME:** `Chapter_01_Shot_1.1_v1.mp4`

### Shot 1.2 (MS)
- [ ] Done
**PROMPT TO PASTE:** Medium shot, gentle rocking camera motion: one or two fishing boats close enough to see lantern light reflecting on the water, quiet pre-dawn mist, warm lantern glow against cool blue tones, photorealistic, cinematic, smooth natural motion, consistent lighting direction, 24fps film-like motion, no morphing or flickering artifacts.
**EXACT FILENAME:** `Chapter_01_Shot_1.2_v1.mp4`

### Shot 1.3 (PUSH / INSERT) — HIGH PRIORITY (Teaser anchor shot, per GMU-006 §4)
- [ ] Done
**PROMPT TO PASTE:** Slow push-in camera move across the misty river-port skyline toward a single lit window high in the distant palace silhouette — the only "wrong" detail in an otherwise ordinary pre-dawn scene, camera movement deliberate and unhurried, warm lantern light against cool blue pre-dawn tones, atmospheric mist, photorealistic, cinematic, smooth natural motion, consistent lighting direction, 24fps film-like motion, no morphing or flickering artifacts.
**EXACT FILENAME:** `Chapter_01_Shot_1.3_v1.mp4`
**Recommend Veo 3.1 for this shot** (Teaser's most important image per GMU-006's priority guidance) — use its "Ingredients to Video" feature with the same reference image and prompt.

---

## SCENE 2 — INT. Palace of Zamar, Sultan's Chamber — Continuous (4 shots)

**FEED THESE REFERENCE IMAGES (all shots in this scene):** `GMU-502_Room1_SultansChamber_REFERENCE_v1.png`
**Continuity note (no locked character file needed):** Sultan Adamu III appears only as a hand — describe consistently every time as "an older man's hand, a signet ring loose on the finger." Servant Girl has no locked reference — describe consistently as "a sixteen-year-old palace servant girl in plain unbleached servant's dress, minimal ornament" per `Background_and_Incidental_Characters.md`.

### Shot 2.1 (ECU / INSERT)
- [ ] Done
**PROMPT TO PASTE:** Extreme close-up insert, static camera: an older man's hand resting on an open ledger, a signet ring loose on the finger, unfinished handwriting trailing off mid-sentence, completely still. Intimate royal study chamber, earth-toned walls with indigo and gold geometric tile inlay, carved lattice windows casting patterned morning light, photorealistic interior, Sahel-inspired palace architecture, smooth natural motion, consistent lighting direction, 24fps film-like motion, no morphing or flickering artifacts.
**EXACT FILENAME:** `Chapter_01_Shot_2.1_v1.mp4`

### Shot 2.2 (WS)
- [ ] Done
**PROMPT TO PASTE:** Wide shot: a sixteen-year-old palace servant girl in plain unbleached servant's dress entering the chamber carrying a morning tray. Intimate royal study chamber, earth-toned walls with indigo and gold geometric tile inlay, carved lattice windows casting patterned morning light, photorealistic interior, Sahel-inspired palace architecture, smooth natural motion, natural fabric physics, consistent lighting direction, 24fps film-like motion, no morphing or flickering artifacts.
**EXACT FILENAME:** `Chapter_01_Shot_2.2_v1.mp4`

### Shot 2.3 (CU)
- [ ] Done
**PROMPT TO PASTE:** Close-up on the servant girl's face as she registers what she's seeing, dawning horror, minimal camera movement, patterned morning light from lattice windows, photorealistic, cinematic, smooth natural motion, consistent character appearance, 24fps film-like motion, no morphing or flickering artifacts.
**EXACT FILENAME:** `Chapter_01_Shot_2.3_v1.mp4`

### Shot 2.4 (INSERT)
- [ ] Done
**PROMPT TO PASTE:** Insert shot: a tray hitting the floor, contents scattering, quick natural motion, patterned morning light, photorealistic interior, Sahel-inspired palace architecture, smooth natural motion, 24fps film-like motion, no morphing or flickering artifacts.
**EXACT FILENAME:** `Chapter_01_Shot_2.4_v1.mp4`

---

## SCENE 3 — INT. University of the Covenant, Scholars' Hall — Morning (10 shots)

**FEED THESE REFERENCE IMAGES (all shots in this scene):** `Fatima_bint_Adamu_REFERENCE_v1.png`, `Elder_Kamal_REFERENCE_v1.png`, `Yusuf_al-Kanem_REFERENCE_v1.png`, `GMU-503_Room1_ScholarsHall_REFERENCE_v1.png`
**Location context (append to every shot below):** Academic lecture hall with terraced white stone walls, high lattice windows casting bright natural light, a wooden lectern, semi-circular seating for robed scholars, Sahel-inspired university architecture, photorealistic, smooth natural motion, consistent character appearance frame-to-frame, consistent lighting direction, 24fps film-like motion, no morphing or flickering artifacts.

### Shot 3.1 (EST WS)
- [ ] Done
**PROMPT TO PASTE:** Establishing wide shot: Scholars' Hall, sunlight through lattice windows, Fatima bint Adamu at the lectern mid-argument, tall composed West African woman, deep indigo scholar's robe with gold trim, dark eyes, calm deliberate posture. [+ Location context above]
**EXACT FILENAME:** `Chapter_01_Shot_3.1_v1.mp4`

### Shot 3.2 (MS)
- [ ] Done
**PROMPT TO PASTE:** Medium shot: Fatima delivering the tariff-dispute argument, animated but controlled gesture, dark eyes holding focus, indigo and gold scholar's robe. [+ Location context above]
**EXACT FILENAME:** `Chapter_01_Shot_3.2_v1.mp4`

### Shot 3.3 (OTS, Fatima's POV)
- [ ] Done
**PROMPT TO PASTE:** Over-the-shoulder shot from Fatima's point of view: Elder Kamal and other robed scholars listening, visibly unconvinced, composed and exacting West African man in his sixties with a neatly groomed beard among semi-circular seated scholars. [+ Location context above]
**EXACT FILENAME:** `Chapter_01_Shot_3.3_v1.mp4`

### Shot 3.4 (CU)
- [ ] Done
**PROMPT TO PASTE:** Close-up on Elder Kamal delivering his dry retort ("you'd have us negotiate with merchants the way we negotiate with children"), composed and exacting expression, neatly groomed beard, stern default with a hint of dry humor. [+ Location context above]
**EXACT FILENAME:** `Chapter_01_Shot_3.4_v1.mp4`

### Shot 3.5 (CU)
- [ ] Done
**PROMPT TO PASTE:** Close-up on Fatima's reply, a ripple of reluctant amusement crossing the room, small brief dry smile. [+ Location context above]
**EXACT FILENAME:** `Chapter_01_Shot_3.5_v1.mp4`

### Shot 3.6 (CU)
- [ ] Done
**PROMPT TO PASTE:** Close-up on Elder Kamal's almost-smile, caught and immediately suppressed, subtle facial micro-expression. [+ Location context above]
**EXACT FILENAME:** `Chapter_01_Shot_3.6_v1.mp4`

### Shot 3.7 (WS)
- [ ] Done
**PROMPT TO PASTE:** Wide shot: doors banging open, Yusuf al-Kanem entering the Scholars' Hall at a near-run, middle-aged deliberately unremarkable West African man in plain muted grey-blue Zamar court dress, urgent but controlled movement. [+ Location context above]
**EXACT FILENAME:** `Chapter_01_Shot_3.7_v1.mp4`

### Shot 3.8 (CU)
- [ ] Done
**PROMPT TO PASTE:** Close-up on Yusuf, breathless but composed, delivering the line "Princess. Your father." — soft reassuring expression even under urgency. [+ Location context above]
**EXACT FILENAME:** `Chapter_01_Shot_3.8_v1.mp4`

### Shot 3.9 (CU)
- [ ] Done
**PROMPT TO PASTE:** Close-up on Fatima — one full second of complete stillness, dark eyes holding, faint appraising expression breaking into shock, minimal camera movement. [+ Location context above]
**EXACT FILENAME:** `Chapter_01_Shot_3.9_v1.mp4`

### Shot 3.10 (WS / TRACK)
- [ ] Done
**PROMPT TO PASTE:** Wide tracking shot: Fatima moving fast for the door, her robe forgotten on the bench behind her, urgent rather than elegant movement, natural fabric physics on the indigo robe. [+ Location context above]
**EXACT FILENAME:** `Chapter_01_Shot_3.10_v1.mp4`

---

## SCENE 4 — EXT. Zamar Cavalry Grounds — Morning (9 shots)

**FEED THESE REFERENCE IMAGES (all shots in this scene):** `Malik_ibn_Adamu_REFERENCE_v1.png`, `GMU-504_TrainingGrounds_REFERENCE_v1.png`
**Location context (append to every shot below):** Dusty open-air cavalry training ground on a city's outskirts, wooden fencing and practice weapon racks, morning sunlight, small indigo unit banners, Sahel-inspired military setting, photorealistic, smooth natural motion, consistent character appearance frame-to-frame, consistent lighting direction, 24fps film-like motion, no morphing or flickering artifacts.

### Shot 4.1 (EST WS)
- [ ] Done
**PROMPT TO PASTE:** Establishing wide shot: dusty training ground, soldiers in practical leather training gear sparring and watching, energetic informal morning atmosphere. [+ Location context above]
**EXACT FILENAME:** `Chapter_01_Shot_4.1_v1.mp4`

### Shot 4.2 (MS)
- [ ] Done
**PROMPT TO PASTE:** Medium shot: Malik ibn Adamu disarming his sparring partner, athletic cavalry-officer build, close-cropped hair, dust-colored leather training gear with forearm guards, confident fluid motion. [+ Location context above]
**EXACT FILENAME:** `Chapter_01_Shot_4.2_v1.mp4`

### Shot 4.3 (WS)
- [ ] Done
**PROMPT TO PASTE:** Wide shot: watching soldiers breaking into genuine laughter, informal energetic atmosphere. [+ Location context above]
**EXACT FILENAME:** `Chapter_01_Shot_4.3_v1.mp4`

### Shot 4.4 (CU / OTS)
- [ ] Done
**PROMPT TO PASTE:** Close-up/over-the-shoulder: Malik delivering a warm banter line to the sparring soldier, open expressive face, quick to smile. [+ Location context above]
**EXACT FILENAME:** `Chapter_01_Shot_4.4_v1.mp4`

### Shot 4.5 (CU)
- [ ] Done
**PROMPT TO PASTE:** Close-up: the young soldier's reply, comic-relief energy, plain slightly disheveled training gear. [+ Location context above]
**EXACT FILENAME:** `Chapter_01_Shot_4.5_v1.mp4`

### Shot 4.6 (WS)
- [ ] Done
**PROMPT TO PASTE:** Wide shot: a dust-covered Zamar messenger-cavalry Rider galloping through the gate at speed, nearly running down two grooms, urgent motion, plain functional riding gear. [+ Location context above]
**EXACT FILENAME:** `Chapter_01_Shot_4.6_v1.mp4`

### Shot 4.7 (CU)
- [ ] Done
**PROMPT TO PASTE:** Close-up: the Rider, breathless, delivering "My prince. The Palace. It's the Sultan." — dust-covered from hard riding, urgent expression. [+ Location context above]
**EXACT FILENAME:** `Chapter_01_Shot_4.7_v1.mp4`

### Shot 4.8 (CU)
- [ ] Done
**PROMPT TO PASTE:** Close-up: Malik's face going completely still, the shift from warmth to shock, open expressive face registering real emotion. [+ Location context above]
**EXACT FILENAME:** `Chapter_01_Shot_4.8_v1.mp4`

### Shot 4.9 (WS)
- [ ] Done
**PROMPT TO PASTE:** Wide shot: Malik already moving with purpose, calling "Get my horse.", decisive urgent motion. [+ Location context above]
**EXACT FILENAME:** `Chapter_01_Shot_4.9_v1.mp4`

---

## SCENE 5 — INT. Palace of Zamar, Sultan's Chamber — Day (11 shots) — HIGH PRIORITY (first major two-hander)

**FEED THESE REFERENCE IMAGES (all shots in this scene):** `Fatima_bint_Adamu_REFERENCE_v1.png`, `Malik_ibn_Adamu_REFERENCE_v1.png`, `GMU-502_Room1_SultansChamber_REFERENCE_v1.png`
**Location context (append to every shot below):** Intimate royal study chamber, earth-toned walls with indigo and gold geometric tile inlay, carved lattice windows, quiet and personal rather than grand, photorealistic interior, Sahel-inspired palace architecture, smooth natural motion, consistent character appearance frame-to-frame, consistent lighting direction, 24fps film-like motion, no morphing or flickering artifacts.

### Shot 5.1 (WS)
- [ ] Done
**PROMPT TO PASTE:** Wide shot: Fatima alone at the desk, ledger open, the room set right but a lingering wrongness in the air, still and composed posture. [+ Location context above]
**EXACT FILENAME:** `Chapter_01_Shot_5.1_v1.mp4`

### Shot 5.2 (CU)
- [ ] Done
**PROMPT TO PASTE:** Close-up: Fatima reading her father's unfinished sentence in the ledger, dark eyes, controlled grief. [+ Location context above]
**EXACT FILENAME:** `Chapter_01_Shot_5.2_v1.mp4`

### Shot 5.3 (WS)
- [ ] Done
**PROMPT TO PASTE:** Wide shot: Malik entering behind her, still visibly dusty from the ride, cavalry command tunic. [+ Location context above]
**EXACT FILENAME:** `Chapter_01_Shot_5.3_v1.mp4`

### Shot 5.4 (2-SHOT)
- [ ] Done
**PROMPT TO PASTE:** Two-shot, both siblings in frame together — a quiet beat of shared grief rather than rivalry, "not rivals, just people who lost their father." [+ Location context above]
**EXACT FILENAME:** `Chapter_01_Shot_5.4_v1.mp4`

### Shot 5.5 (OTS / CU alternating)
- [ ] Done
**PROMPT TO PASTE:** Alternating over-the-shoulder / close-up exchange: "Was it — did anyone say —" / "He went to sleep writing." — restrained emotional exchange between Fatima and Malik. [+ Location context above]
**EXACT FILENAME:** `Chapter_01_Shot_5.5_v1.mp4`

### Shot 5.6 (INSERT)
- [ ] Done
**PROMPT TO PASTE:** Insert shot: Malik's hands picking up and closing the ledger, deliberate gentle motion. [+ Location context above]
**EXACT FILENAME:** `Chapter_01_Shot_5.6_v1.mp4`

### Shot 5.7 (CU)
- [ ] Done
**PROMPT TO PASTE:** Close-up: Malik delivering "Forty days." with a small exhausted laugh, warm but tired expression. [+ Location context above]
**EXACT FILENAME:** `Chapter_01_Shot_5.7_v1.mp4`

### Shot 5.8 (CU / OTS alternating)
- [ ] Done
**PROMPT TO PASTE:** Alternating close-up / over-the-shoulder: the "countdown" exchange between Fatima and Malik, escalating quietly, tension rising beneath calm surfaces. [+ Location context above]
**EXACT FILENAME:** `Chapter_01_Shot_5.8_v1.mp4`

### Shot 5.9 (CU)
- [ ] Done
**PROMPT TO PASTE:** Close-up: Malik asking "Is that a warning?" — genuine hurt beginning to show through his usually open face. [+ Location context above]
**EXACT FILENAME:** `Chapter_01_Shot_5.9_v1.mp4`

### Shot 5.10 (CU)
- [ ] Done
**PROMPT TO PASTE:** Close-up: Fatima's answer, careful and direct, controlled stillness as her tell. [+ Location context above]
**EXACT FILENAME:** `Chapter_01_Shot_5.10_v1.mp4`

### Shot 5.11 (2-SHOT)
- [ ] Done
**PROMPT TO PASTE:** Two-shot, holding on both siblings — a visible unresolved shift in their dynamic, quiet and charged. [+ Location context above]
**EXACT FILENAME:** `Chapter_01_Shot_5.11_v1.mp4`

---

## SCENE 6 — INT. Diwan Hall — Later, Day (6 shots)

**FEED THESE REFERENCE IMAGES (all shots in this scene):** `Fatima_bint_Adamu_REFERENCE_v1.png`, `Malik_ibn_Adamu_REFERENCE_v1.png`, `Elder_Kamal_REFERENCE_v1.png`, `GMU-502_Room2_DiwanHall_REFERENCE_v1.png`
**Location context (append to every shot below):** Formal council chamber with tiered stone seating for a dozen robed scholars and clergy, earth-toned walls with indigo and gold geometric ornamentation, tall lattice windows, solemn formal lighting, Sahel-inspired judicial-religious architecture, photorealistic, smooth natural motion, consistent character appearance frame-to-frame, consistent lighting direction, 24fps film-like motion, no morphing or flickering artifacts.

### Shot 6.1 (EST WS)
- [ ] Done
**PROMPT TO PASTE:** Establishing wide shot: full council chamber, tiered seating, Fatima and Malik standing at opposite ends of the open floor. [+ Location context above]
**EXACT FILENAME:** `Chapter_01_Shot_6.1_v1.mp4`

### Shot 6.2 (MS)
- [ ] Done
**PROMPT TO PASTE:** Medium shot: Elder Kamal presiding, beginning the formal proclamation, presiding sash, exacting composed bearing. [+ Location context above]
**EXACT FILENAME:** `Chapter_01_Shot_6.2_v1.mp4`

### Shot 6.3 (CU)
- [ ] Done
**PROMPT TO PASTE:** Close-up: Kamal delivering "the throne of Zamar is vacant..." with formal weighted cadence. [+ Location context above]
**EXACT FILENAME:** `Chapter_01_Shot_6.3_v1.mp4`

### Shot 6.4 (WS)
- [ ] Done
**PROMPT TO PASTE:** Wide shot: the full council listening in formal solemn silence. [+ Location context above]
**EXACT FILENAME:** `Chapter_01_Shot_6.4_v1.mp4`

### Shot 6.5 (CU)
- [ ] Done
**PROMPT TO PASTE:** Close-up: Kamal delivering "The clock begins today." — his most formally performed line, measured and deliberate. [+ Location context above]
**EXACT FILENAME:** `Chapter_01_Shot_6.5_v1.mp4`

### Shot 6.6 (CROSSCUT CU/CU)
- [ ] Done
**PROMPT TO PASTE:** Crosscut close-ups: Fatima and Malik's single shared look across the hall, unspoken weight passing between them. [+ Location context above]
**EXACT FILENAME:** `Chapter_01_Shot_6.6_v1.mp4`

---

## SCENE 7 — EXT. Tsauri Keep, Kasar Dutse — Day (7 shots)

**FEED THESE REFERENCE IMAGES (all shots in this scene):** `Garba_Ironhand_REFERENCE_v1.png`, `GMU-505_FortressWall_REFERENCE_v1.png`
**Location context (append to every shot below):** High grey stone fortress wall overlooking a dramatic mountain pass, deep red banners snapping in strong wind, overcast dramatic sky, harsh mountain light, Sahel-inspired highland fortress architecture, photorealistic, smooth natural motion, consistent character appearance frame-to-frame, consistent lighting direction, 24fps film-like motion, no morphing or flickering artifacts.

### Shot 7.1 (EST WS)
- [ ] Done
**PROMPT TO PASTE:** Establishing wide shot: high fortress wall over the mountain pass, strong wind, red banners snapping. [+ Location context above]
**EXACT FILENAME:** `Chapter_01_Shot_7.1_v1.mp4`

### Shot 7.2 (MS)
- [ ] Done
**PROMPT TO PASTE:** Medium shot: King Garba Ironhand standing at the wall's edge, weathered mid-fifties man with grey-streaked beard and old eyebrow scar, deep red and iron-grey layered garments, a Messenger kneeling behind him. [+ Location context above]
**EXACT FILENAME:** `Chapter_01_Shot_7.2_v1.mp4`

### Shot 7.3 (CU)
- [ ] Done
**PROMPT TO PASTE:** Close-up: Garba delivering "Forty days." with total stillness and quiet unhurried authority, low register. [+ Location context above]
**EXACT FILENAME:** `Chapter_01_Shot_7.3_v1.mp4`

### Shot 7.4 (CU)
- [ ] Done
**PROMPT TO PASTE:** Close-up: the Messenger's reply, kneeling posture, plain Kasar Dutse red and iron-grey uniform. [+ Location context above]
**EXACT FILENAME:** `Chapter_01_Shot_7.4_v1.mp4`

### Shot 7.5 (WS)
- [ ] Done
**PROMPT TO PASTE:** Wide shot: Garba turning, calling orders to mobilize the war-captains, unhurried decisive motion, calm rather than urgent. [+ Location context above]
**EXACT FILENAME:** `Chapter_01_Shot_7.5_v1.mp4`

### Shot 7.6 (CU) — HIGH PRIORITY (episode's closing line)
- [ ] Done
**PROMPT TO PASTE:** Close-up: Garba's closing line delivered almost gently, "let's see what a kingdom of scholars does with a countdown," calm unsettling quietness. [+ Location context above]
**EXACT FILENAME:** `Chapter_01_Shot_7.6_v1.mp4`
**Recommend Veo 3.1 for this shot** (episode-closing line, per GMU-006 priority guidance).

### Shot 7.7 (WS, pull back)
- [ ] Done
**PROMPT TO PASTE:** Wide pull-back shot: Garba alone at the wall, the mountain pass stretching below him, scale emphasized against his solitary stillness. [+ Location context above]
**EXACT FILENAME:** `Chapter_01_Shot_7.7_v1.mp4`

---

# SECTION 3 — Replicating This for Chapters 02–20 (mechanical formula, no creative judgment needed)

For every remaining chapter:

1. Open that chapter's shot list in `20_STORYBOARDS/CHAPTER_XX/Chapter_XX_Shot_List.md`.
2. For each scene in the list, note its **Location** ID (e.g., GMU-505) and **Characters** listed at the top of that scene.
3. Build that scene's **Location context** block by copying the exact "AI image prompt" text for that room/variant from the matching `19_CONCEPT_ART/GMU-50X` file (drop the "photorealistic... wide shot" tail and instead append the fixed video-motion tail: `photorealistic, smooth natural motion, consistent character appearance frame-to-frame, consistent lighting direction, 24fps film-like motion, no morphing or flickering artifacts.`)
4. For each shot row in that scene's table, write: `[Shot type] shot: [the Description text from that row, lightly reworded into a camera-direction sentence if needed] + [that character's short physical descriptor, reused from their GMU-013 prompt] + [the Scene's Location context block from step 3]`
5. Reference images to feed = every character appearing in that shot's `AI_MODEL_LIBRARY/*_REFERENCE_v1.png` + that scene's location `19_CONCEPT_ART/*_REFERENCE_v1.png`.
6. Filename = `Chapter_XX_Shot_<row number>_v1.mp4`, saved to `06_SEASON_ONE/CHAPTER_XX/RENDERS/`.
7. Any shot flagged as highest-priority in that chapter's Production Notes section → use Veo 3.1 instead of Kling.

This is exactly the same process just applied to Chapter 01 above — nothing here requires new creative decisions, only mechanical application of the existing shot list + existing character/location prompts.

**Recommended chapter order (per GMU-006 §4):** Chapters 01–02 first (done above for 01), then Chapters 19–20 (the finale), then the rest in story order (03 through 18).

## Status

Draft — ready to execute. Chapter 01's 24 shots are fully assembled from `GMU-771_Chapter_01_Shot_List.md` combined with the locked character/location prompts from GMU-013/GMU-014 and GMU-007's master style language. Section 3's formula is mechanical, not creative — apply it identically to Chapters 02–20 as those chapters' Phase 1 assets are locked.
