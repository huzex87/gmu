Document ID: GMU-007
Document Name: Prompt Library
Classification: Reference
Version: 0.3 Draft
Status: In Progress
Owner: Huzaifa Yakub
Last Edited: 2026-07-11 (corrected: removed Udio per GMU-006 tool research)
Canon Status: N/A
Approval Status: Pending
Dependencies: GMU-002 (Creative & Brand Bible), GMU-004 (World Bible), GMU-005 (Character Bible), GMU-006 (AI Production Bible)

---

# GMU-007 — Prompt Library

Estimated length: ~500 pages at full maturity. This v0.2 draft establishes the reusable prompt system every character sheet and location brief in this repository already draws on informally — this document makes those conventions explicit, catalogued, and copy-pasteable, so consistency doesn't depend on any one person remembering the right phrasing. Grows continuously as production proceeds; treat every section below as a living template, not a finished spec.

## How To Use This Document

Every AI image/video/voice/music prompt in this repository (character sheets in `05_CHARACTER_BIBLE/AI_MODEL_LIBRARY/`, location briefs in `19_CONCEPT_ART/`) already follows the conventions below. When writing a *new* prompt — for a shot not explicitly covered by an existing sheet, a new background character, or a new location — build it from these templates rather than freehand, so it matches everything already generated. Bracketed `[terms]` are the variables to fill in per-asset.

---

## 1. Master Visual Style Prompt (append to every image/video generation)

This is the base "look" of Gidan Mulki Universe — append it to the end of every character, location, and prop prompt in this repository, adjusting only the medium-specific tail (photorealistic still vs. cinematic video motion).

**Base style block (still images):**
> ...photorealistic, cinematic quality, natural volumetric lighting, rich but grounded color grading, Sahel-inspired West African aesthetic, culturally specific and respectful detail (not generic "fantasy Africa"), sharp fine detail on fabric texture and architectural carving, consistent character reference sheet where applicable, no anachronistic elements, no modern text or logos.

**Base style block (video generation, append after the still-image prompt):**
> ...smooth natural motion, consistent character appearance frame-to-frame, cinematic camera movement matching the shot type specified, natural fabric and hair physics, consistent lighting direction throughout the shot, 24fps film-like motion, no morphing or flickering artifacts.

**Negative prompt (apply to all generations, per Section 9):** see Section 9 below — do not generate without it.

---

## 2. Per-Kingdom / Per-Faith Environment Templates

Use these as the opening clause of any environment prompt not already covered by an existing location brief (`19_CONCEPT_ART/`). Each pulls its palette directly from GMU-002's locked color codes.

### 2.1 Zamar (Sultanate)

> [Interior/Exterior] in Sahel-inspired Islamic-scholarly architecture, earth-toned walls (warm sand, ochre) with indigo (#2E3A6E) and gold (#C9A24B) geometric tile inlay and carved lattice ornamentation, deep-set lattice windows casting patterned light, off-white (#F4EFE4) stone base, understated furnishings relative to the architecture, law-and-learning aesthetic rather than martial or mercantile display...

### 2.2 Kasar Dutse (Kingdom)

> [Interior/Exterior] in fortified mountain-stone architecture, deep red (#7A2323) and iron-grey (#5C5F62) banners and accents against raw black (#1C1B19) and grey stone, minimal ornamentation, crossed-spear motifs, defensive and martial in character, honor-code austerity rather than ceremonial richness...

### 2.3 Kwara (River Confederacy)

> [Interior/Exterior] in open mercantile architecture, light timber and pale stone construction, emerald (#1F5C4A) and white (#F7F5F0) banners with silver (#B8BFC4) accent trim, canal-facing open walls, transparency and liquidity of movement rather than monumentality, functioning trade-economy aesthetic...

### 2.4 The Faith of the Covenant (Islam — faith-specific, cross-kingdom)

> [Interior/Exterior] in austere Islamic sanctuary architecture, neutral stone tones (sand, pale grey, warm white) with restrained geometric carving distinct from any single kingdom's color system, soaring pillars or high windows admitting clear unshadowed light, dignified and independent of political display...
Per GMU-004 §1's religious-basis decision: keep this space visually and symbolically outside the Zamar/Kasar Dutse/Kwara color system entirely — do not default to Zamar's indigo/gold even though the Sanctuary is physically located in Birnin Zamar.

### 2.5 Neutral / Unaligned Spaces (villages, disused/derelict locations)

> [Interior/Exterior] in humble, sun-worn Sahel vernacular architecture, ochre and tan earth tones, weathered wood, no kingdom banners or official color-coding present, lived-in and human-scale rather than ceremonial...

---

## 3. Character Consistency Formula

Every character prompt in `05_CHARACTER_BIBLE/AI_MODEL_LIBRARY/` follows this five-part structure. Use it verbatim when drafting a prompt for a background/incidental character not already covered by `Background_and_Incidental_Characters.md`:

1. **Demographic anchor:** age, build, ethnicity/region-appropriate features (West African, Sahel-region-consistent)
2. **Defining physical trait:** the one or two details that make the character recognizable at a glance (a scar, a particular bearing, a signature stillness or restlessness)
3. **Costume, by kingdom/rank:** pull directly from the character's kingdom template (Section 2) plus their specific rank/role markers per their Character Bible entry
4. **Setting/lighting context:** match the scene's location brief
5. **Reference-sheet framing:** `...consistent character reference sheet, neutral studio background, front view / three-quarter view / side profile` for turnaround sheets; drop this clause for in-scene/action generations

**Formula example (generic template):**
> Portrait and full-body reference turnaround of a [age] [build] West African [gender], [defining physical trait], wearing [kingdom costume template + rank markers]. [Setting from location brief], [lighting condition], photorealistic, consistent character reference sheet, neutral studio background, front view / three-quarter view / side profile.

## 4. Costume Rendering Notes (by rank tier)

- **Royalty/heads of state (Fatima, Malik, Garba, Amina):** full kingdom color saturation, rank-appropriate ornament per Character Bible costume markers, richest fabric detail in any given scene.
- **Senior officials/clergy (Kamal, Bashir, Nafisa, Tahir):** kingdom or faith colors present but more restrained, formal robes/uniform over ceremonial richness.
- **Field/working rank (Danladi, Rafiu, common soldiers, village elders):** muted, practical, weathered versions of kingdom colors — visibly lived-in rather than pristine, per GMU-412's "practical repairs, sun-faded fabric" note.
- **Household/background staff (Abubakar, stewards, clerks):** minimal-to-no rank markers, deliberately unremarkable per GMU-414's design philosophy — do not over-ornament background characters even when generating them at higher visual prominence for a specific shot.
- **The unnamed fourth power (Yusuf's true signet, post-Episode 9):** small, geometric, deliberately ancient/plain mark — never elaborate. See GMU-405's post-reveal note.

## 5. Battle / Action Scene Prompts

Season One has exactly two armed-conflict sequences (Episode 5's border skirmish, Episode 7's pass seizure) plus several tense-but-unarmed standoffs (Episode 2, Episode 3's border pass scenes). Keep combat generation restrained and non-graphic per GMU-001's quality bar — this is a political drama, not a war epic.

**Skirmish/close combat template (Episode 5):**
> Chaotic close-quarters skirmish between [Zamar cavalry template] and [Kasar Dutse cavalry template], dust and motion blur, urgent and confused rather than choreographed, non-graphic impact framing (cut away from direct violence, favor reaction shots and aftermath), muted desaturated color grading during combat, restrained camera shake, film-realistic rather than stylized...

**Standoff/tension template (border pass scenes, Episodes 2, 3, 5, 7):**
> Two opposing military formations facing each other across [marker stones / a contested line], static tense composition, wide shot emphasizing distance and scale, muted early-morning or dusk lighting, flags/banners as the only movement in an otherwise still frame, high tension through stillness rather than action...

**Aftermath template (post-skirmish, Episode 5 Act Three/Four):**
> Quiet battlefield aftermath, fallen figures framed respectfully and non-graphically (silhouette, distance, or partial framing rather than explicit detail), soldiers in shock or grief, muted grey-blue color grading, overcast or dusk lighting, somber restrained tone...

## 6. Establishing Shot / Cinematography Prompts

Tied directly to GMU-002's cinematography and lighting philosophy (camera language: formal symmetry for ceremonial power, handheld intimacy for private/emotional scenes; lighting: warm interior lattice-light for Zamar, cold stone-light for Kasar Dutse, reflected water-light for Kwara, clear unshadowed light for the Covenant).

**Wide establishing template:**
> Wide establishing shot of [location], [time of day] light consistent with [kingdom/faith lighting philosophy], camera [static/slow push/aerial], scale emphasized to orient the audience, cinematic color grading matching [kingdom palette]...

**Intimate/dialogue scene template:**
> Medium/close framing for an intimate dialogue scene between [characters], handheld or subtly unstable camera for emotional scenes vs. locked-off formal framing for political/ceremonial scenes, [kingdom lighting philosophy], shallow depth of field on the primary subject...

## 7. Voice Generation Prompts / Direction Templates (ElevenLabs)

Character sheets currently specify vocal *direction* (tone, pacing, register) rather than a bound ElevenLabs voice ID — actual voice casting is deferred until production begins (see each character sheet's Voice Direction section). When casting, use this template to log the final binding:

```
Character:          [Name]
Character Bible Ref: GMU-005 §[section]
ElevenLabs Voice ID: [to be filled at casting]
Base Settings:       Stability [0-1], Similarity [0-1], Style Exaggeration [0-1]
Direction Summary:   [pull from character sheet's Voice Direction section]
Special Notes:       [e.g., Yusuf: no tonal shift during "tell" scenes until Ep 9; Abubakar: one vocal break allowed, Ep 9 only]
```

**General guidance:** Zamar characters (Fatima, Malik, Kamal, Bashir, Nafisa) — precise, measured diction reflecting the kingdom's law-and-learning identity. Kasar Dutse (Garba) — short, weighted sentences, minimal vocal ornamentation. Kwara (Amina) — charming, quick, never quite letting warmth read as sincerity. Yusuf/Abubakar — deliberately unremarkable, reassuring register that should never telegraph menace until their respective reveal scenes.

## 8. Music Generation Prompts (Suno / ElevenLabs Music) — Per Kingdom/Mood

Cross-reference `04_WORLD_BIBLE/MUSIC/` once that sub-bible is written; until then, use these as placeholder direction. **Tool note (2026-07-11, see GMU-006 §1):** generate on Suno's Pro/Premier plan for commercial release rights, or ElevenLabs Music as a licensed-training-data alternative. Do not use Udio — as of 2026 it has become a closed platform whose generations cannot be downloaded or used outside it, making it incompatible with this project regardless of plan tier.

- **Zamar theme:** contemplative, string and wind instrumentation, modal/scalar patterns evocative of West African and Islamic scholarly musical traditions, restrained percussion, "law and learning" mood — dignified rather than triumphant.
- **Kasar Dutse theme:** driving percussion-forward, low brass or horn, martial but not bombastic, mountain-wind ambient texture underneath.
- **Kwara theme:** lighter, rhythmically fluid, water-adjacent ambient texture (subtle flowing/liquid sound design), charming rather than grand.
- **The Covenant / faith theme:** vocal-forward (chant/call structure appropriate to real Islamic devotional music traditions — research actual maqam/nasheed conventions rather than inventing generic "spiritual" music), sparse instrumentation, reverent.
- **The fourth power / Yusuf's theme:** deliberately minimal or absent — silence and ambient room-tone as the musical choice, reinforcing "unremarkable by design" per his character sheet, until Episode 9's reveal, where a single sustained unresolved tone may be introduced.
- **Tension/investigation theme:** sparse, percussive, uses negative space — avoid over-scoring the season's many quiet-conversation scenes.

## 9. Negative Prompts / Consistency Guardrails

Apply to every generation in this repository without exception:

> Negative prompt: no anachronistic clothing or technology, no modern text or logos, no generic "fantasy Africa" tropes, no orientalist exoticization, no exaggerated or caricatured facial features, no inconsistent character faces between shots, no morphing/warping artifacts, no oversaturated or cartoonish color grading, no gratuitous graphic violence, no romanticized or sanitized war imagery that contradicts the screenplay's restrained treatment of combat, no invented religious iconography that isn't grounded in real Islamic visual tradition (per GMU-004 §1's editorial guidance).

**Character-specific guardrails:**
- Yusuf (GMU-405) / Abubakar (GMU-414): resist any tool's tendency to add "sinister" visual flourishes (shadowed lighting, narrowed eyes) — their menace is entirely behavioral/contextual, never visual.
- High Cleric Nafisa (GMU-413): do not default her costume/architecture to Zamar's indigo/gold — the Faith of the Covenant is visually independent of all three kingdoms.
- Garba (GMU-403): resist "warlord" caricature — per Theme 4 (no one is entirely good or evil), his design should read as dignified and restrained, not menacing.

## Status

In Progress. Core templates (Sections 1–9) now drafted, extracted from and made consistent with every prompt already used across `05_CHARACTER_BIBLE/AI_MODEL_LIBRARY/` (13 character sheets) and `19_CONCEPT_ART/` (10 location briefs). This is a living document — as actual image/video generation begins and specific prompts prove out (or fail) in practice, log successful phrasing back into this file so the library improves with use rather than staying purely theoretical. Still needed: real ElevenLabs voice ID bindings (post-casting), real Suno/ElevenLabs Music track references (post-composition), and a battle-tested set of "known good" seed/reference parameters once image generation actually begins.
