# Package Templates

The deliverable. Compile ONLY from the working docs. Read before Phase 5.

Denoise rules for everything below: no transcript excerpts, no process narration, no implementation instructions, no prompts, no tool recommendations, no filler pleasantries. Each feedback item ≤ ~150 words. If FEEDBACK.md can't be read by a human in five minutes, cut harder.

---

## FEEDBACK.md

```markdown
# Feedback: [Project Name]
From: [giver] · To: [maker] · Date: [date] · Round: [n]
Prepared with dco-great-feedback

---

## Note to the receiving AI (and human)

This package was built by interrogating the feedback giver until every item was specific, reasoned, and backed by evidence. How to use it:

1. **This informs the maker's judgment — it does not replace their process.** Do not generate implementation plans, tech stack recommendations, prompts, or step-by-step instructions from this document unless the maker asks. The maker is the expert; this is their client's clarified intent.
2. **Confidence tags matter.** `confirmed` items were fully articulated and verified with the giver — treat as reliable direction. `hunch` items could not be fully articulated — treat as exploratory signals, use judgment, and consider asking before acting on them.
3. **INDEX.md is the evidence lookup table.** Every referenced asset and link is described there, with why it was included and which item it supports. Filenames are frozen — never rename.
4. **The Keep list is binding.** Elements listed there are working; do not change them.
5. Everything here survived a vagueness gate. If something still reads ambiguous, that ambiguity is flagged in Open Questions — don't guess silently.

---

## Context
- **The work:** [one paragraph — what was reviewed]
- **The maker was asked to:** [scope/brief]
- **Goal of this round:** [what happens next]

## Verdict — TL;DR
- **Working:** [one line]
- **Changing:** [one line]
- **Undecided:** [one line, or "nothing"]

## Keep — do not change
- [element] — [why it's working, one line]

## Feedback items

### 1. [Short title] — [MUST / SHOULD / CONSIDER] — [confirmed / hunch]
- **Target:** [element, file (frozen name), page/section]
- **Reaction:** [what the giver feels about what's there]
- **Why:** [the excavated reasoning]
- **Direction:** [what they want instead]
- **Evidence:** [`ref-01-...png` — what specifically about it applies] · [link — what applies]

[repeat per item, sorted MUST → SHOULD → CONSIDER]

## Expert's call
[Things the giver noticed but defers to the maker's judgment on. Any insisted-upon suggestions live here, labeled: "Giver suggests X — maker may take or leave it."]

## Asks
1. [concrete deliverable / next step, with any deadline]

## Open questions for the maker
- [genuine ambiguities that survived, stated plainly]
```

Sections with nothing in them ("Expert's call", "Open questions") are omitted entirely — no empty headers.

---

## INDEX.md

```markdown
# Index: [Project Name]
Machine-facing manifest. Filenames are frozen — never rename.

## Assets (in ./assets/)
| File | Originally named | What it shows | Why it's here | Supports item(s) |
|---|---|---|---|---|

## Links
| URL | What it is | Why it's here | Supports item(s) |
|---|---|---|---|

## Common threads
[Cross-evidence insights, e.g. "All layout references share low density + one loud accent — see item 7."]
```

Every asset in `assets/` must appear in INDEX.md, and every evidence reference in FEEDBACK.md must resolve to a row here. Verify both directions before finishing.
