Document ID: GMU-320
Document Name: Master Encyclopedia — Schema
Classification: Reference
Version: 0.6 Draft
Status: In Progress
Owner: Huzaifa Yakub
Last Edited: 2026-07-12 (population expanded to 55 entries — see Status)
Canon Status: N/A
Approval Status: Pending
Dependencies: GMU-004

---

# GMU Master Encyclopedia — Schema

A Wikipedia-style reference for every person, village, horse, sword, building, battle, proverb, king, law, road, festival, food, and tree in the universe. Target: 10,000+ entries. One file per entry in this folder, named `ENTRY-#####_Name.md`.

## Entry ID Range

`ENTRY-00001` upward. Reserve blocks by category so IDs stay sortable:

| Range | Category |
|---|---|
| ENTRY-00001–00999 | Places (cities, villages, regions) |
| ENTRY-01000–01999 | People |
| ENTRY-02000–02999 | Objects (weapons, artifacts, buildings) |
| ENTRY-03000–03999 | Events (battles, treaties, ceremonies) |
| ENTRY-04000–04999 | Culture (proverbs, festivals, customs, food) |
| ENTRY-05000–05999 | Flora/Fauna (trees, horses, animals) |
| ENTRY-06000–06999 | Institutions (laws, offices, orders) |

## Standard Entry Template

```
Document ID: ENTRY-#####
Document Name: [Entry Title]
Classification: Encyclopedia Entry
Category: Place | Person | Object | Event | Culture | Flora/Fauna | Institution
Version: 0.1 Draft
Status: Not Started
Owner:
Last Edited: YYYY-MM-DD
Canon Status: Provisional | Canon
Approval Status: Pending
Dependencies: [related entries / bibles]

---

# [Entry Title]

## Summary
[1-2 sentence definition]

## Key Facts
[Category-specific fact table — see worked example]

## Description
[Full prose description]

## History
[If applicable]

## Cross References
[Links to related ENTRY-##### IDs, and to owning bibles e.g. GMU-306 Architecture Bible]

## Maps
[Link to relevant Atlas entry, if a place]
```

See `ENTRY_00001_Birnin_Zamar.md` in this folder for a fully worked example (a city entry, adapted from the founding discussion).

## Status

Schema defined. **Population expanded 2026-07-12: 55 entries total**, across all seven categories:

- **Places (11):** Birnin Zamar (ENTRY-00001, revised), Royal Palace of Zamar (00002), University of the Covenant (00003), The Great Market (00004), Tsauri Keep (00005), Port of Kwarafi (00006), Zamar Cavalry Grounds (00007), Kwarafi Merchant House (00008), Great Sanctuary of the Covenant (00009), Kantin Rafi (00010), Old Customs House (00011)
- **People (15):** all named Season One characters — Fatima, Malik, Garba, Amina, Yusuf, Danladi, Bashir, Tahir, Kamal, Halima, Rafiu, Nafisa, Abubakar (ENTRY-01001–01013), plus Sultan Adamu I (01014) and Sultan Adamu III (01015) as historical/referenced figures — each a concise cross-reference pointer to the full biography in GMU-005 (or, for the two Sultans, to the founding-era and pre-Season-One references that establish them), not a duplicate
- **Objects (7):** Yusuf's Signet (02001), the Seal of Zamar (02002), the Planted Evidence Trail (02003), the Compass Rose Standard of Zamar (02004), King Garba's War-Blade (02005), the Founding Charter of Kwara (02006), the Diwan's Ledger of Ratification (02007)
- **Events (10):** the Death of Sultan Adamu III (03001), the Murder of Elder Bashir (03002), the Border Skirmish (03003), the Tsauri Pass Seizure (03004), the Diwan Ratification Vote and Yusuf's Exposure (03005), the Coronation of Fatima (03006), the Founding of Birnin Zamar (03007), the Unification of Kasar Dutse (03008), the Founding of the Confederacy of Kwara (03009), the Ratification of Sultan Adamu III (03010)
- **Culture (4):** Founding Day (04001), the Pass Opening (04002), Flood Reckoning (04003), Harvest Court (04004)
- **Flora/Fauna (4):** Kasar Dutse Mountain Horse (05001), Silver River Fish (05002), Zamar Grain (05003), Northern Desert Caravan Camel (05004, new — see GMU-317 §6)
- **Institutions (4):** The Diwan al-Ilm (06001), Merchant Council of Kwara (06002), War-Captains of Kasar Dutse (06003), Ulama of Zamar (06004)

*(Note: this Status section was found truncated mid-sentence at the "Culture (4)" line during the 2026-07-12 update — completed and the two missing category bullets restored above; no entry content was lost, only this summary list.)* 