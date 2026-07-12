Document ID: GMU-017
Document Name: Music, Editing & Quality Gate Master Checklist
Classification: Reference (Production Asset / Staff Handoff Packet)
Version: 1.0
Status: In Progress
Owner: Huzaifa Yakub
Last Edited: 2026-07-12
Canon Status: N/A
Approval Status: Pending
Dependencies: GMU-007 §8 (Music direction), GMU-006 §5–7 (Phases 4–6), GMU-016 (video must exist before scoring/editing a chapter)

---

# GMU-017 — Music, Editing & Quality Gate Master Checklist

**Hand this document to your music/score person and your editor.** It covers Phase 4 (Suno music generation, exact prompts embedded), Phase 5 (DaVinci Resolve assembly, exact steps), and Phase 6 (the quality gate checklist to run before calling any chapter finished).

---

## PART A — Music (Suno). Hand to: Music/Score person.

### Before You Start
1. Create a Suno account (suno.com), subscribe to **Pro or Premier** — the free tier's output cannot be used commercially, and this does not apply retroactively if you upgrade later. Generate everything under a paid plan from day one.
2. **Do not use Udio for this project** — as of 2026 it's a closed platform that doesn't allow downloading/exporting generated tracks, making it unusable for a video production pipeline.

### The 6 Ready-to-Paste Music Prompts (one per mood/kingdom, embedded verbatim from GMU-007 §8)

Generate per-scene or per-chapter cues, not one long score — this lets you swap a single cue later without regenerating everything.

**1. Zamar theme** — use for any scene set in the Palace, Diwan Hall, University, or involving Zamar characters in a law/scholarship context:
> Contemplative orchestral cue, string and wind instrumentation, modal/scalar patterns evocative of West African and Islamic scholarly musical traditions, restrained percussion, dignified rather than triumphant mood, "law and learning" atmosphere, no vocals.

**2. Kasar Dutse theme** — use for Tsauri Keep, Garba's scenes, any Kasar Dutse military mobilization:
> Driving percussion-forward orchestral cue, low brass or horn, martial but not bombastic, mountain-wind ambient texture underneath, no vocals.

**3. Kwara theme** — use for the Kwarafi Merchant House, Amina's scenes, canal/trade settings:
> Light rhythmically fluid orchestral cue, water-adjacent ambient texture (subtle flowing/liquid sound design), charming rather than grand mood, no vocals.

**4. The Covenant / faith theme** — use for the Great Sanctuary, Nafisa's scenes, religious ceremony:
> Vocal-forward devotional cue in the tradition of real Islamic chant/call structure (research actual maqam/nasheed conventions — do not invent generic "spiritual" music), sparse instrumentation, reverent mood.

**5. The fourth power / Yusuf's theme** — use sparingly, only where his true nature needs subtle musical presence:
> Deliberately minimal or near-silent ambient cue, mostly room-tone and negative space, until a single sustained unresolved tone may be introduced only in Episode/Chapter 9's reveal scene — do not score Yusuf's earlier appearances with any identifiable musical theme.

**6. Tension/investigation theme** — use for the mourning-period investigation scenes, Bashir's death aftermath, quiet-conversation scenes needing an undercurrent:
> Sparse, percussive orchestral cue that uses negative space and silence deliberately, understated tension, no vocals, avoid over-scoring.

### Procedure per cue
1. Paste the matching mood prompt above into Suno's generation box.
2. Add scene-specific detail: cue length and purpose (e.g., "40-second cue for a quiet council scene, fading out at the end").
3. Generate (Suno gives 2 variations) — pick the stronger one.
4. Download (MP3 or WAV).
5. Save into `21_SOUNDTRACK/`, named: `Chapter_<NN>_<Kingdom/Mood>_Cue_v1.mp3` (e.g., `Chapter_01_Zamar_Council_Cue_v1.mp3`).
6. Optional: also try the same prompt in ElevenLabs Music as a comparison — useful later for its Inpainting feature if you need to fix one section of an accepted cue without regenerating the whole thing.

### Sound design (not covered by a ready prompt yet)
Ambient/foley (crowd noise, cavalry, market ambience, mountain wind) isn't in GMU-007 yet — source stock/library sound effects matching each scene's location and mood, or use whichever tool's SFX feature is available. Log any effective prompts you find back into GMU-007 §8 for reuse.

---

## PART B — Editing & Assembly (DaVinci Resolve). Hand to: Editor.

### Before You Start
1. Download DaVinci Resolve free tier: blackmagicdesign.com/products/davinciresolve.
2. Do not start a chapter's edit until: (a) all its video shots exist in `06_SEASON_ONE/CHAPTER_XX/RENDERS/` per GMU-016, (b) all its dialogue clips exist per GMU-015, (c) its music cues exist per Part A above.

### Per-Chapter Assembly Steps
1. Open DaVinci Resolve → **New Project** → name it `GMU Chapter <NN>`.
2. **Media** tab → import every clip from that chapter's `RENDERS/` folder, plus dialogue audio and music cues (drag-and-drop from File Explorer into the Media Pool).
3. **Edit** tab → drag video clips onto the timeline **in screenplay order** (check `Chapter_XX_Screenplay.md` for correct scene order — this is not necessarily the order shots were generated in).
4. Add audio layers in this priority, top to bottom: dialogue first (never sacrifice dialogue clarity), music underneath, sound design/ambience as the lightest top layer.
5. **Color** tab → grade each scene to its location's established palette:
   - Zamar interiors/exteriors: warm amber lattice-light tones
   - Kasar Dutse: harsher, cooler, overcast tones
   - Kwara: reflected water-light, cooler/greener
   - Covenant/Sanctuary: clear, unshadowed, neutral light
   - This step is what actually locks the look consistent — AI-generated shots vary in color temperature even from identical prompts.
6. Titles: apply GMU-002 §14's compass-rose-reveal/palette-cycling title card design, but only once you have real cut footage to design it against.
7. **Deliver** tab → export the finished chapter.

---

## PART C — Quality Gate (run before calling ANY chapter finished). Hand to: Whoever signs off on chapters (recommend: project owner).

Watch the finished cut once, specifically checking each of these — this is GMU-001 §12's Charter bar, applied per chapter:

- [ ] Character faces/costumes stay consistent shot to shot (the single most common failure point — check especially at scene cuts)
- [ ] Architecture and color language stay consistent within each location across the chapter
- [ ] The narrative is clear to someone who hasn't read the screenplay
- [ ] Each character's voice is distinct enough to identify who's speaking without seeing them
- [ ] No drifted/inconsistent faces versus that character's locked GMU-013 reference
- [ ] No visual/tonal violations of any character-specific guardrail (Yusuf/Abubakar not sinister-looking, Garba not caricatured, Nafisa's costume not defaulting to Zamar colors)
- [ ] Combat/violence content matches the restrained, non-graphic treatment specified in GMU-007 §5 (only relevant for Chapters with skirmish/action content — Episode 5 and 7 material)

If any box fails: identify which phase produced the problem (wrong reference locked in GMU-013/014, wrong voice cast in GMU-015, a drifted shot in GMU-016, or a color-grade miss in Part B here) and fix at that phase rather than patching around it in the final export.

**Do this per chapter, every time** — chapters produced early in the pipeline (when reference images and prompt technique were newest/least refined) are exactly where drift is most likely to have crept in unnoticed.

## Status

Draft — ready to execute. Music prompts extracted verbatim from GMU-007 §8; editing/QA steps extracted and expanded from GMU-006 §§5–7 into literal click-level instructions. No new creative decisions were made — only actual music-cue selection (Suno's 2-variation pick) and grading judgment calls require real staff input.
