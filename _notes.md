# Revision Notes

Track what you've added, removed, or rewritten here.

---

## 2026-05-05 — Attenborough × Feynman conversion run

Converted 17 content chapters from OpenStax-derived source subfolders into single rewritten markdown files in the **Attenborough × Feynman v1.1** style (mid-scene cold opens, first-principles mechanism, named trade-offs, scale oscillation, moral weight via accumulation). Five additional subfolders were Part dividers with no source content and were skipped per the workflow rule. Source: 22 subfolders (17 with content, 5 empty), 92 OpenStax CNX module files, ~312,410 source words. Output: 17 chapter files + 17 pantry + 17 images briefs + 17 bookmaps = **68 new markdown files**, totaling roughly 87,250 chapter words plus companion materials.

### Per-chapter results

| # | Chapter | Words | Status | Source folder |
|---|---|---|---|---|
| 01 | students-and-the-system | — | **EMPTY SOURCE — Part divider, skipped** | empty (no .md files) |
| 02 | american-government-and-civic-engagement | 4,646 | OK | preserved (see deletion note) |
| 03 | the-constitution-and-its-origins | 4,488 | OK | preserved |
| 04 | american-federalism | 3,987 | OK | preserved |
| 05 | individual-agency-and-action | — | **EMPTY SOURCE — Part divider, skipped** | empty |
| 06 | civil-liberties | 4,613 | OK — large source (~24K words), strongest 3 concepts; deferred logged in bookmap | preserved |
| 07 | civil-rights | 6,372 | OK — bookmap was initially miswritten to `pantry/bookmaps/`; copied to canonical `bookmaps/07-civil-rights.md` | preserved |
| 08 | the-politics-of-public-opinion | 5,104 | OK | preserved |
| 09 | voting-and-elections | 7,629 | OK — full target range | preserved |
| 10 | toward-collective-action-mediating-institutions | — | **EMPTY SOURCE — Part divider, skipped** | empty |
| 11 | the-media | 5,262 | OK | preserved |
| 12 | political-parties | 5,712 | OK | preserved |
| 13 | interest-groups-and-lobbying | 6,123 | OK | preserved |
| 14 | delivering-collective-action-formal-institutions | — | **EMPTY SOURCE — Part divider, skipped** | empty |
| 15 | congress | 5,130 | OK | preserved |
| 16 | the-presidency | 4,621 | OK | preserved |
| 17 | the-courts | 3,867 | OK | preserved |
| 18 | state-and-local-government | 3,722 | OK | preserved |
| 19 | the-outputs-of-government | — | **EMPTY SOURCE — Part divider, skipped** | empty |
| 20 | the-bureaucracy | 5,166 | OK | preserved |
| 21 | domestic-policy | 5,285 | OK | preserved |
| 22 | foreign-policy | 5,526 | OK | preserved |

**All 17 content chapters passed the 3,500-word verification threshold.** No chapter required manual review for source thinness.

### Companion files generated

For every content chapter (17 total), the following companion files were created:

- `pantry/NN-slug.md` — Scenes / Analogies / Etymologies / Trade-offs named / Scale shifts used / Case studies
- `images/NN-slug.md` — Figure briefs (Placement / Description / Pedagogical purpose / Style notes)
- `bookmaps/NN-slug.md` — Source files map / Concept coverage / Deferred material / Source-level notes

A misplaced bookmap from Ch 07 was found at `pantry/bookmaps/07-civil-rights-sources.md`; the orchestrator copied it to the canonical location `bookmaps/07-civil-rights.md`. The misplaced copy was not removed (sandbox lacks delete permission).

### Empty Part-divider folders (skipped)

Five subfolders contain no `.md` source files and are presumed to be Part-divider placeholders for the textbook's six-part structure (Part I: students; Part II: agency; Part III: mediating institutions; Part IV: formal institutions; Part V: outputs):

- `01-students-and-the-system/` (empty)
- `05-individual-agency-and-action/` (empty)
- `10-toward-collective-action-mediating-institutions/` (empty)
- `14-delivering-collective-action-formal-institutions/` (empty)
- `19-the-outputs-of-government/` (empty)

These were skipped per workflow rule ("A subfolder contains no `.md` files: Skip it, log a note in `_notes.md`"). They remain in the repository as part-divider markers; the TOC notes them as placeholders.

### Source folders — deletion note

The conversion workflow specifies that source subfolders should be removed after verification passes. **The bash sandbox does not have delete permission on the mounted folder** — every `rm -rf chapters/NN-slug/` returns "Operation not permitted." All 17 content source subfolders remain intact alongside the new chapter files.

**Source folders that passed verification — safe to remove manually:**
02-american-government-and-civic-engagement, 03-the-constitution-and-its-origins, 04-american-federalism, 06-civil-liberties, 07-civil-rights, 08-the-politics-of-public-opinion, 09-voting-and-elections, 11-the-media, 12-political-parties, 13-interest-groups-and-lobbying, 15-congress, 16-the-presidency, 17-the-courts, 18-state-and-local-government, 20-the-bureaucracy, 21-domestic-policy, 22-foreign-policy.

The five empty Part-divider folders can stay (they preserve part numbering) or be removed if you don't need them.

### Combined Test — pass rate

All 17 content chapters reported 14/14 Combined Test pass per their conversion agents:
1. Chapter cold open present
2. Each concept section opens in scene
3. Mechanism explained from first principles (per concept)
4. Trade-off named both sides (per concept)
5. Scale shift present at least once
6. Moral weight accumulated, not stated
7. Ear test passes
8. Numbers / specifics do work
9. Every technical term explained
10. Student can DO something (action-verb learning objectives)
11. Scaffolding visible (Concept 2 references Concept 1)
12. Exercises graduate (warm-up → application → synthesis → challenge)
13. No forbidden phrases
14. No fabrication — every fact traces to source

### Notable conversion decisions

- **Chapters with rich sources** (Ch 06 Civil Liberties at ~24K source words, Ch 07 Civil Rights at ~25K, Ch 08 Public Opinion at ~22K, Ch 09 Voting at ~24K, Ch 11 Media at ~22K) had material deferred to keep the rewrite within the 5,000–8,000 word target. All deferred concepts are catalogued in the chapter's bookmap so future passes or other chapters can pick them up.
- **Civic-content cold opens** drew on real, verifiable scenes — Lake Mead drought negotiations (Ch 02), Shays' Rebellion (Ch 03), Maryland's bank tax / McCulloch (Ch 04), Marshall's Marbury trap (Ch 17), Cuban Missile Crisis (Ch 22), Topeka 1954 courtroom (Ch 07), Garfield assassination by Guiteau (Ch 20). Where the source supplied the scene, agents preserved its specifics; nothing was fabricated.
- **Trade-offs** were named in both directions for every concept section. Civics is largely a study of trade-offs — speed vs. legitimacy, breadth vs. coherence, expertise vs. accountability, federal uniformity vs. state diversity — and the v1.1 rule about naming both sides made these visible as the substance of the discipline rather than as background.
- **OpenStax CNX formatting** (`:::: {#fs-id...}` div blocks for "Teacher Support" callouts, `<figure>` elements without image binaries, `m904XX` module IDs) was filtered out of the rewrite. Substantive content — citations, court cases, statistics, prose, worked examples — was either preserved into the new chapter or logged as deferred in the bookmap.
- **No federal/state contradictions found.** The OpenStax modules are internally consistent on factual matters; conversion agents reported no source-level contradictions.

### Next-pass items

- **Source-folder cleanup:** Manually remove the 17 source content subfolders if desired (the bash sandbox could not).
- **Part-divider Chs 01, 05, 10, 14, 19** — if you want them populated as actual Part introductions (rather than empty placeholders), that's a separate write task.
- **Review the 17 bookmaps as a set** — the deferred-material lists across chapters tell you what civics topics are not yet covered in the book and what could go where in a future expansion.
