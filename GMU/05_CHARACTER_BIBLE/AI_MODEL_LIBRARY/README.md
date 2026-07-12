Document ID: GMU-005a
Document Name: AI Model Library — Schema
Classification: Reference
Version: 0.3 Draft
Status: In Progress
Owner: Huzaifa Yakub
Last Edited: 2026-07-11 (added Episodes 3-9 character sheets: Halima, Rafiu, Nafisa, Abubakar)
Canon Status: N/A
Approval Status: Pending
Dependencies: GMU-005

---

# AI Model Library

Per-character reusable production assets. One file per character, named `<CHARACTER_NAME>_assets.md`. Each sheet covers physical reference, costume, expression/performance notes, a ready-to-use AI image generation prompt, and voice direction — everything needed to generate consistent concept art and, later, consistent video across scenes.

## Episode 01 Character Design Sheets (complete)

| ID | Character | File | Priority |
|---|---|---|---|
| GMU-401 | Fatima bint Adamu | `Fatima_bint_Adamu_assets.md` | Highest — protagonist |
| GMU-402 | Malik ibn Adamu | `Malik_ibn_Adamu_assets.md` | Highest — co-protagonist |
| GMU-403 | King Garba Ironhand | `Garba_Ironhand_assets.md` | High |
| GMU-404 | Speaker Amina Bello Kwarafi | `Amina_Bello_Kwarafi_assets.md` | High |
| GMU-405 | Yusuf al-Kanem | `Yusuf_al-Kanem_assets.md` | High |
| GMU-406 | Danladi | `Danladi_assets.md` | Medium — priority rises at Episode 8 |
| GMU-407 | Elder Bashir | `Elder_Bashir_assets.md` | Highest — episode's emotional pivot |
| GMU-408 | General Tahir | `General_Tahir_assets.md` | Medium |
| GMU-409 | Elder Kamal | `Elder_Kamal_assets.md` | Medium — rises at Episode 9 |
| GMU-410 | Background/incidental roles (8 characters) | `Background_and_Incidental_Characters.md` | Low — lighter notes only |

## Episodes 03–09 Character Design Sheets (new)

| ID | Character | File | First Appears |
|---|---|---|---|
| GMU-411 | Queen Mother Halima | `Halima_assets.md` | Episode 03 |
| GMU-412 | Commander Rafiu | `Commander_Rafiu_assets.md` | Episode 04 |
| GMU-413 | High Cleric Nafisa | `High_Cleric_Nafisa_assets.md` | Episode 06 |
| GMU-414 | Abubakar | `Abubakar_assets.md` | Background Ep 1–6; named Ep 07 |

Note: GMU-405 (Yusuf al-Kanem) has an added post-reveal note at the bottom of his sheet reflecting his Episode 9 exposure — his physical/costume design does not change, only the production guidance around his true signet.

## Per-Character Asset Schema (original template, still applies)

```
Character: [Name]
Linked Character Bible Entry: GMU-005 §[section]

Face Model:        [reference / seed / LoRA identifier]
Voice Model:        [ElevenLabs voice ID or description]
Walking Style:      [description]
Expression Set:     [list of reference expressions]
Horse:               [if applicable — linked to Bestiary/Encyclopedia]
Weapon:              [linked to Military Bible]
Costume:             [linked to Costume Bible, by scene/rank variant]
Prompt Library Ref:  GMU-007 §[section]
```

Note: the completed sheets above use a slightly expanded format (Physical Reference / Costume / Expression Notes / AI Prompt / Voice Direction) that proved more useful in practice than the original schema's flat field list — the schema stays here as the original spec, but new sheets should follow the pattern in the Episode 01 files.

## Status

In Progress. All 9 named Episode 1 characters, the consolidated background-roles file, and 4 new Episodes 3–9 characters (Halima, Rafiu, Nafisa, Abubakar) are drafted and ready to generate reference images against — 13 named character sheets total. Still needed: actual image generation (requires FLUX/Midjourney access — see README's Recommended External Infrastructure), then locking approved images here as the canonical reference before video generation begins. Voice model selection (actual ElevenLabs voice IDs) is deferred until voice casting begins — these sheets currently specify direction/character, not a bound voice ID.
