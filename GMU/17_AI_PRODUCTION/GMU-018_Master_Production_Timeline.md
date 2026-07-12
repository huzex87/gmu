Document ID: GMU-018
Document Name: Master End-to-End Production Timeline
Classification: Reference (Master Index)
Version: 1.0
Status: In Progress
Owner: Huzaifa Yakub
Last Edited: 2026-07-12
Canon Status: N/A
Approval Status: Pending
Dependencies: GMU-006, GMU-007, GMU-012, GMU-013, GMU-014, GMU-015, GMU-016, GMU-017

---

# GMU-018 — Master End-to-End Production Timeline

This is the single index document. Start here. It puts every other execution document in this repository into one strict order, names who should own each phase, and shows exactly what gets handed to whom and when. Everything referenced below already exists and is ready to execute — nothing in this document requires further writing before work can begin.

## The Full Pipeline, Start to Finish

```
STEP 0 — Read this document + GMU-012 (zero-experience orientation)
        ↓
STEP 1 — Character Images  (owner: Art Lead)         → GMU-013
STEP 2 — Location Images   (owner: Art Lead)          → GMU-014
        [STEP 1 + STEP 2 can run in parallel, same person or two people]
        ↓ (both must be 100% checked off before Step 3)
STEP 3 — Voice Casting     (owner: Voice Lead)        → GMU-015
        ↓ (can start as soon as Step 1 is done — doesn't need Step 2)
STEP 4 — Video Generation, per chapter (owner: Video Lead)  → GMU-016
        ↓ (needs Step 1 + Step 2 done; needs Step 3 done before dialogue is added to a shot)
STEP 5 — Music & Sound Design, per chapter (owner: Music Lead)  → GMU-017 Part A
        ↓ (can run in parallel with Step 4, once you know which chapter you're scoring)
STEP 6 — Editing & Assembly, per chapter (owner: Editor)  → GMU-017 Part B
        ↓ (needs Steps 3, 4, 5 all done for that specific chapter)
STEP 7 — Quality Gate, per chapter (owner: Project Owner)  → GMU-017 Part C
        ↓
Finished Chapter → repeat Steps 4–7 for the next chapter
```

## Staff Handoff Points (exactly what to hand each person)

| Role | Hand them | They do | They hand back |
|---|---|---|---|
| **Art Lead** | GMU-013 + GMU-014 (this packet) | Generates and locks all 13 character images + all 28 location images in Midjourney/FLUX | Two fully checked-off documents + all image files saved in `05_CHARACTER_BIBLE/AI_MODEL_LIBRARY/` and `19_CONCEPT_ART/` |
| **Voice Lead** | GMU-015 | Casts all 13 character voices in ElevenLabs, logs voice IDs | Fully checked-off document + voice IDs logged into GMU-007 §7 |
| **Video Lead** | GMU-016 (Chapter 01 done as template) + the relevant chapter's shot list from `20_STORYBOARDS/` | Generates every shot for a chapter in Kling/Veo, following GMU-016 Section 3's formula for chapters beyond 01 | Checked-off shot list + `.mp4` files in that chapter's `RENDERS/` folder |
| **Music Lead** | GMU-017 Part A | Generates that chapter's music cues in Suno | `.mp3`/`.wav` files in `21_SOUNDTRACK/` |
| **Editor** | GMU-017 Part B + all outputs from Video Lead, Voice Lead, Music Lead for that chapter | Assembles, grades, and exports the finished chapter in DaVinci Resolve | One exported finished chapter file |
| **Project Owner (you)** | GMU-017 Part C | Runs the Quality Gate checklist against the finished export | Sign-off, or a specific note on which phase to redo |

**Key rule that doesn't change no matter how many people you have:** Steps 1 and 2 (all characters, all locations) must be 100% finished before Step 4 starts on *any* chapter. This is the one sequencing rule GMU-006 is most insistent about — skipping it is the single most common way a project like this ends up with visibly inconsistent characters between early and late chapters.

## Recommended Chapter Production Order (once Steps 1–3 are fully done)

1. Chapter 01, then Chapter 02 (most heavily detailed, prompt-tested material — do these first to validate your whole pipeline works before scaling to the rest)
2. Chapter 19, then Chapter 20 (season finale — the visual culmination, most likely footage for a trailer/pitch reel)
3. Chapters 03–18, in story order

## If You're Running This With Multiple Staff Simultaneously

Once GMU-013 and GMU-014 are both fully checked off, you can parallelize aggressively:
- One Video Lead can work Chapter 01 while a second works Chapter 02, since both only depend on the now-complete Phase 1 assets and Phase 2 (voices, if dialogue is being added).
- Music Lead and Video Lead can work the same chapter simultaneously (music doesn't depend on video existing first) — they only need to converge at the Editor's desk.
- The Editor is the one true bottleneck per chapter — nothing in Step 6 can start until Steps 3–5 are all done for that specific chapter.

## Budget Snapshot (full detail in GMU-006 §10)

- Images (Steps 1–2): likely under $50–100 total across all 41 images (13 characters + variants + 28 locations + variants).
- Voice (Step 3): ElevenLabs Creator, $22/mo, likely sufficient for the full season.
- Video (Step 4): the dominant cost — roughly $350 baseline at Kling pricing for the whole season's shots, budget 2–3x that for retries.
- Music (Step 5): Suno Pro/Premier, roughly $10–30/mo.
- Editing (Step 6): free (DaVinci Resolve free tier).

## Document Map — Everything You Need, In One Place

| Document | What it's for |
|---|---|
| GMU-018 (this document) | Start here — the master order and handoff map |
| GMU-012 | Zero-experience orientation to every tool, before touching any of them |
| GMU-013 | Character image generation — full checklist, ready to execute |
| GMU-014 | Location image generation — full checklist, ready to execute |
| GMU-015 | Voice casting — full checklist, ready to execute |
| GMU-016 | Video generation — Chapter 01 fully worked, formula for the rest |
| GMU-017 | Music, editing, and quality gate — full checklist, ready to execute |
| GMU-006 | The underlying strategy document all of the above were built from — read if you want the "why," not just the "how" |
| GMU-007 | The master prompt/style library every checklist above pulled its exact prompts from |

## Status

Draft — this is the operational entry point for turning the finished GMU production bible into actual footage. Every document it references is complete and ready to execute as of 2026-07-12. Update the chapter-by-chapter progress by checking off GMU-013 through GMU-017 as work proceeds; this document itself shouldn't need to change unless the overall pipeline strategy changes.
