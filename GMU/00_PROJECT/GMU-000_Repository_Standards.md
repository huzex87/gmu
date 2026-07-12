# GMU Repository Standards

Document ID: GMU-000
Document Name: Repository Standards
Classification: Governance
Version: 1.0
Status: Active
Owner: Huzaifa Yakub
Last Edited: 2026-07-10
Canon Status: N/A (process document)
Approval Status: Approved
Dependencies: None

---

## 1. Purpose

This document defines the rules every GMU document must follow so that a 3,500+ page, multi-year, multi-collaborator franchise stays internally consistent. Read this before creating or editing any document in the repository.

## 2. Required Metadata Header

Every document (bible, entry, screenplay, asset spec) must open with this block:

```
Document ID: GMU-XXX
Document Name:
Classification: Canon (Foundational) | Canon | Non-Canon | Reference | Governance
Version: 0.1 Draft
Status: Not Started | In Progress | Draft | In Review | Approved | Locked
Owner:
Last Edited: YYYY-MM-DD
Canon Status: Provisional | Canon | Deprecated
Approval Status: Pending | Approved | Rejected
Dependencies: [Document IDs this one relies on]
```

| Field | Meaning |
|---|---|
| Document ID | Unique, sequential (GMU-001, GMU-002…). Encyclopedia entries use `ENTRY-###`. |
| Classification | "Canon (Foundational)" = load-bearing for the whole universe; changing it requires review. |
| Version | Semantic-ish: `0.x Draft` pre-approval, `1.0` on approval, increment minor for edits, major for canon-breaking revisions. |
| Status | Lifecycle stage — keep current. |
| Owner | Person (or role) accountable for the document. |
| Canon Status | Whether content is binding on all future material. |
| Approval Status | Has this cleared governance review (Section 4)? |
| Dependencies | What has to stay stable for this doc to remain valid — flags ripple effects when something upstream changes. |

## 3. Document ID Registry

| Range | Reserved For |
|---|---|
| GMU-000 – GMU-099 | Governance / project-level (charter, standards, franchise plan) |
| GMU-100 – GMU-199 | Creative & Brand |
| GMU-200 – GMU-299 | Series Bible |
| GMU-300 – GMU-399 | World Bible + sub-bibles |
| GMU-400 – GMU-499 | Character Bible |
| GMU-500 – GMU-599 | AI Production Bible |
| GMU-600 – GMU-699 | Prompt Library |
| GMU-700 – GMU-799 | Screenplays |
| GMU-800 – GMU-899 | Marketing |
| GMU-900 – GMU-999 | Franchise Plan / Investor materials |
| ENTRY-00001+ | Master Encyclopedia entries |

*(Note: the original Phase 0 list used GMU-001 through GMU-010 as flat top-level document numbers — that numbering is preserved for the 10 primary bibles below. This registry extends it for everything that comes after, e.g. individual encyclopedia entries or sub-bible chapters, so IDs never collide as the corpus grows.)*

## 4. Canon Change Control

Elements that are **fixed once approved** unless formally revised through this process:

- Geography
- Calendar
- Kingdoms
- Major historical events
- Royal houses
- Constitutional structure
- Core character biographies

To change any of the above: open a change note in the owning document, bump its version, list every dependent document (via the Dependencies field of anything downstream), and get Owner sign-off before merging.

## 5. Quality Gates Before "Approved"

**Writing:** clear narrative, consistent canon, strong dialogue, distinct character voices.
**Visuals:** consistent architecture, consistent costumes, recognizable symbols, cohesive color language.
**Production:** repeatable workflows, organized assets, version-controlled documentation.

## 6. Folder Placement Rule

If you're unsure where a new document belongs, it goes in the folder matching its Document ID range above. Encyclopedia entries always go in `04_WORLD_BIBLE/MASTER_ENCYCLOPEDIA/`, tagged with category (person, place, object, event, custom) in the entry itself.
