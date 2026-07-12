# Working Document Templates

Templates for everything in `working/`. Fill every field; write "none" rather than omitting. These docs must let a fresh session with zero conversation history continue perfectly — write for that reader.

---

## STATE.md

```markdown
# Session State — [Project Name]
Started: [date] · Giver: [name/role if known] · Maker: [name/role if known]

| Phase | Status | Completed | Note |
|---|---|---|---|
| 0 — Subject ingest | not started / in progress / done | [timestamp] | [one line, e.g. "14 assets inventoried, giver confirmed"] |
| 1 — Raw dump | ... | | |
| 2 — Interrogation | ... | | [e.g. "items 1–3 confirmed, 4 open, 5–6 untouched"] |
| 3 — Evidence | ... | | |
| 4 — Gate | ... | | |
| 5 — Package | ... | | |

**Next action:** [always current, always specific — "Resume item 4 (wordmark weight): giver said 'too corporate', probing what corporate means, last candidate set sent"]
```

Update on every meaningful step, not just phase boundaries. A closed laptop at any moment must leave this file truthful.

---

## 00-SUBJECT.md

```markdown
# Subject Report — [Project Name]

## Context
- The work: [what the maker produced, one paragraph]
- The maker was asked to: [scope/brief as the giver states it]
- Goal of this feedback round: [what the giver wants to happen next]
- Round: [1 / 2 / n — context only, v1 sessions are standalone]

## Asset inventory (renamed at intake — names now frozen)
| Original name | New name | Type | Description (1 line) |
|---|---|---|---|

## Structure map
[For large documents: section names + page/heading refs, so interrogation can cite "p.34, color system". For small subjects: brief outline.]

## Understanding playback
[The summary given to the giver, verbatim.]

**Giver confirmed this understanding:** [yes — date/words used]
```

---

## 01-RAW-DUMP.md

```markdown
# Raw Dump — [Project Name]

## Verbatim
[Everything the giver said, exactly as said. No cleanup, no summary, no fidelity loss. Multiple dumps get dated subsections.]

## Candidate items (Phase 2 worklist)
| # | Candidate item (one line) | Source (quote fragment) |
|---|---|---|

**Giver confirmed list complete:** [yes/date]
```

---

## 02-ITEMS.md

```markdown
# Interrogation Ledger — [Project Name]

## Item [N]: [short title]
- **Status:** raw / probing / confirmed / hunch (override) / dropped
- **Raw words:** "[verbatim from dump]"
- **Target:** [specific element, file, page]
- **Reaction:** [what they feel about what's there]
- **Why:** [the reasoning excavated by probing]
- **Direction:** [what they want instead]
- **Evidence:** [asset new-names / links from 03-EVIDENCE.md]
- **Priority:** must / should / consider
- **Echo-check (canonical wording):** "[the confirmed echo, verbatim]"
- **Probe log:** [1–3 lines: how we got here — useful on resume]
- **If hunch:** giver's override words: "[verbatim]"
```

One block per item. Status field is what makes resume work — keep it current.

---

## 03-EVIDENCE.md

```markdown
# Evidence Manifest — [Project Name]

## Assets
| New name | Original name | What it shows | Why included (what specifically applies) | Supports item(s) |
|---|---|---|---|---|

## Links
| URL | What it is | Why included | Supports item(s) |
|---|---|---|---|

## Research findings (confirmed by giver)
- [finding + source link + which item it clarified]

## Contradiction notes & common threads
- [e.g. "ref-01..04 span 3 visual directions; giver confirmed the common thread is low-density layouts with one loud accent — logged as item 7"]
```

---

## 04-GATE.md

```markdown
# Readiness Gate — [Project Name] — run [date]

## Session-level checks
- [ ] Subject understanding confirmed by giver (00-SUBJECT.md)
- [ ] All candidate items resolved: confirmed / hunch / dropped (02-ITEMS.md)
- [ ] Every asset & link has description + purpose + item linkage (03-EVIDENCE.md)
- [ ] Contradictions resolved into threads or explicitly noted
- [ ] Keep-list captured (what the maker must NOT touch)
- [ ] Asks captured (concrete next deliverables)

## Per-item checks
| Item | Specific target | Why present | Direction present | Evidence ≥1 | Verdict |
|---|---|---|---|---|---|
| 1 | ✓/✗ | ✓/✗ | ✓/✗ | ✓/✗/hunch | pass / reopen / hunch-pass |

## Overrides
- [item # — giver's exact words authorizing the override]

**Gate result:** PASSED / not yet — [what's blocking]
```

Fail → reopen the item in Phase 2, tell the giver exactly what's missing. Nothing is written to `package/` until this reads PASSED.
