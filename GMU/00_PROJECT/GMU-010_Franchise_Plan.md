Document ID: GMU-010
Document Name: Franchise Plan
Classification: Governance
Version: 1.0 Draft
Status: In Progress
Owner: Huzaifa Yakub
Last Edited: 2026-07-11
Canon Status: N/A
Approval Status: Pending
Dependencies: GMU-001 (Charter §3, §4), GMU-000 (Repository Standards), GMU-009 (Marketing Plan)

---

# GMU-010 — Franchise Plan

How Gidan Mulki Universe expands beyond the television series into the full franchise scope named in GMU-001 §3: publishing, digital/interactive, gaming, educational content, and commercial licensing. This is the business and IP-expansion counterpart to the Series Bible — it plans *what gets built and when*, not story content itself.

## 1. Multi-Media Expansion Roadmap (per GMU-001 §3)

### 1.1 Publishing

- **Novels** — direct prose adaptations of each season, expandable beyond screenplay constraints (interiority, backstory) in ways the screen format can't carry. Season One's 20-chapter structure (GMU-008) maps naturally onto a novel's chapter structure, making this the lowest-adaptation-cost publishing product.
- **Graphic novels** — visual adaptation drawing directly on GMU-002's locked visual system and, once produced, the character/location reference images from GMU-006's pipeline — the same visual assets serve both the show and this product.
- **Encyclopedias** — a physical/ebook product built directly from the Master Encyclopedia (GMU-320 schema, population in progress) once it reaches sufficient depth — this is the one publishing product that's already partially built as a byproduct of production-bible work rather than requiring separate authoring.
- **Children's editions** — simplified, age-appropriate adaptations; requires a separate editorial pass to soften Season One's political-thriller content (a death, a murder investigation, war) rather than a direct adaptation.

### 1.2 Digital/Interactive

- **Interactive website** — the long-term home for the world (per GMU-009 §5); should launch with, at minimum, the character roster and world map once the Atlas (GMU-311) has an illustrated version.
- **Character database** — a browsable version of GMU-005's Character Bible and the Master Encyclopedia's Person-category entries.
- **Interactive timeline** — built directly from GMU-004 §3's CU timeline and GMU-313's Calendar, expandable as the Master Encyclopedia's Event-category entries grow.
- **Interactive map** — built once GMU-311's written Atlas gets an illustrated version (flagged as an open task in GMU-311 §7).
- **Wiki** — effectively a public-facing mirror of the Master Encyclopedia, gated to what's appropriate for public release versus internal production reference.

### 1.3 Gaming

- **Mobile strategy game** — natural fit given the three-power political structure (GMU-004 §2) already resembles a strategy game's faction design; the Political, Military, and Economic Bibles (GMU-309, GMU-308, GMU-310) are effectively a ready-made game-design reference for faction mechanics.
- **PC strategy game** — deeper version of the same, potentially spanning the full CU timeline (GMU-004 §3) rather than just Season One's 427 CU snapshot.
- **RPG** — character-driven, likely set in the same era as the show but following original characters rather than the principal cast, to avoid contradicting screen canon.
- **Card game** — lowest-cost gaming product, built directly from the Character Bible and Master Encyclopedia's existing entries as card content.

### 1.4 Educational

- **African history companion** — contextualizes the show's real Sahelian and Islamic-governance grounding (GMU-305, GMU-004 §1) against actual history, distinct from the in-world fiction itself.
- **Architecture companion** — built from GMU-306's Architecture Bible, explaining both the fictional per-kingdom systems and their real Sudano-Sahelian architectural grounding (per GMU-305/GMU-506's research).
- **Leadership companion** — drawing on the show's political-drama content (succession law, governance systems, GMU-309) as a leadership/ethics discussion framework.
- **Storytelling curriculum** — using the production process itself (Charter → World Bible → Character Bible → Screenplay → Storyboard, per GMU-001's Addendum pipeline) as a teachable worldbuilding methodology.

### 1.5 Commercial

- **Merchandise** — built directly from GMU-002's locked visual system (kingdom colors, seals, symbols) once that system is fully finalized.
- **Licensing** — third-party use of the world/characters, gated behind the IP protection strategy (Section 5).
- **Collectibles** — figures/art tied to character and location reference art once Phase 1 image generation (GMU-006 §2) produces a locked visual library.
- **Art books** — a natural byproduct of concept art production (GMU-006 §2, GMU-007's Prompt Library, 19_CONCEPT_ART/'s location briefs) rather than a separately authored product.

## 2. Sequencing (per GMU-001 §4)

| Year | Milestone | Franchise-plan relevance |
|---|---|---|
| **Year One** | Charter, Series Bible, World Bible, Character Bible, Season One, Episode One screenplay, Pitch Deck, Visual Identity, Website Prototype | **Status as of 2026-07-11: design phase essentially complete** — Charter, Series Bible, World Bible (all 14 sub-bibles), Character Bible, full Season One (20 chapters), Prompt Library, and AI Production Bible are all drafted. Pitch Deck (GMU-009 §3) and Website Prototype remain the two genuinely open Year One items. |
| **Year Two** | AI Concept Art, Storyboards, Trailer, Pilot Episode, Investor Package | Storyboards are already complete (GMU-771–790); AI Concept Art, Trailer, and Pilot Episode require Phase 1–5 production (GMU-006) to actually begin. Investor Package draws on GMU-009 §4. |
| **Year Three** | Begin production of the first season; expand audience engagement through digital platforms and publishing | First publishing (Section 1.1) and digital (Section 1.2) products should target this window, once Season One footage exists to adapt from and market against. |

## 3. GMU Studio Company Formation Plan

**Proposed divisions** (per the original founding discussion's scope): Writing, Animation, Film, Publishing, Games, AI Research, Music, Education, Licensing, Merchandise, Training. Each division corresponds directly to a Section 1 product category above — Writing/Film to the core series, Publishing to Section 1.1, Games to Section 1.3, Education to Section 1.4, Licensing/Merchandise to Section 1.5, AI Research to the production pipeline itself (GMU-006), and Music/Training as supporting functions (the former feeding GMU-314's Music Bible into real scoring, the latter feeding Section 1.4's storytelling curriculum back into the studio's own onboarding, alongside START_HERE.md).

**Sequencing note:** Per GMU-001 §10's production philosophy, formal division structure should follow actual production need rather than being staffed up speculatively — a single AI Research/Production function can cover Phase 1 production (GMU-006) long before a dedicated Games or Merchandise division has anything to build against.

## 4. GitHub Organization / Repository Split Plan

Per the root README's existing note, when ready to move off the local repository: a private GitHub org (`GMU Studio`) split into `gmu-charter`, `gmu-world-bible`, `gmu-characters`, `gmu-screenplays`, `gmu-prompts`, `gmu-production`, `gmu-assets`, `gmu-website`, `gmu-brand`. This split should happen once the repository is stable enough that cross-repo Dependencies references (per GMU-000 §2) won't be constantly broken by ongoing edits — likely once Year One's remaining items (Pitch Deck, Website Prototype) are complete, rather than mid-draft as sub-bibles were still being written.

## 5. IP Protection and Licensing Strategy

**Originality as protection:** Per GMU-001 §9's Franchise Position, the project's core IP-protection asset is its originality — a wholly original setting, cast, and mythology rather than an adaptation, meaning there's no underlying-rights complexity to manage before the studio can license its own material freely.

**Licensing gating (per Section 1.5):** No third-party licensing should be granted before GMU-002's visual identity is fully locked and before a Canon-classified core (per GMU-000 §4's Canon Change Control — geography, calendar, kingdoms, major historical events, royal houses, constitutional structure, core character biographies) is stable, so licensed products can't accidentally contradict material the core team later needs to lock differently.

**Trademark scope:** "GIDAN MULKI" as the flagship title (per GMU-001 Addendum, already locked) is the primary trademark asset; kingdom names (Zamar, Kasar Dutse, Kwara) and the franchise's visual seals (GMU-002) are secondary marks worth registering once commercial licensing (Section 1.5) becomes real rather than speculative.

## 6. Long-Term Vision

The founding discussion's original scope named a long-term ambition of GMU Studio eventually supporting 20–40 original African universes under one studio umbrella, with Gidan Mulki Universe as the first and proof-of-concept franchise. This document does not plan those future universes in any detail — doing so now would violate the same "just enough, just in time" discipline that governs the World Bible's sub-bibles (GMU-004 §6) — but the studio-formation structure in Section 3 and the repository/documentation standards in GMU-000 are deliberately built to be reusable for a second universe once Gidan Mulki itself reaches Year Three's production milestone.

## Status

In Progress. Full multi-media expansion roadmap, Year 1/2/3 sequencing (cross-checked against the project's actual current state), company formation plan, GitHub org plan, and IP protection strategy drafted against GMU-001's real Scope and Strategic Objectives sections. The long-term multi-universe vision (Section 6) is intentionally left unplanned in detail, consistent with the project's broader "just enough, just in time" discipline.
