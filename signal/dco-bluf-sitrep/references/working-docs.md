# Working Document Templates

Everything in `working/`. Fill every field; "none" or "skipped" rather than omitting. A fresh session with zero conversation history must continue perfectly from these docs. (LOG.md's template lives in ledger.md; SITREP-NN.md's in sitrep-template.md.)

---

## STATE.md

```markdown
# Session State — [Subject]
Subject: [what this sitrep covers] · Reader: [name/role if known]
**Current run: [N]** · Runs completed: [list with dates, e.g. "1 (07/11)"]

## Run [N] phases
| Phase | Status | Completed | Note |
|---|---|---|---|
| 0 — Scope + brain dump | not started / in progress / done | [timestamp] | [one line] |
| 1 — Acquisition | ... | | [e.g. "5 acquired, zoom transcript unavailable"] |
| 2 — Reconstruction | ... | | [e.g. "ledger at L-23, email thread 2 of 3 processed"] |
| 3 — Analysis | ... | | |
| 4 — SITREP + plan | ... | | |

**Next action:** [always current, always specific — "Process slack export (source 4), append to ledger from 07/02 forward"]
```

On a chained run: increment the run counter, add a fresh phase table for the new run (keep old tables below it as history).

---

## 00-SCOPE.md

```markdown
# Scope — [Subject]

## Boundary
[What this sitrep is on — and, if useful, what's explicitly OUT.]

## Players
| Name | Role / relationship | 
|---|---|

## Brain dump — Run [N], [date]  (verbatim)
[Everything the reader got off their chest, exactly as said. "Skipped" if skipped.]

## What the reader most needs to know
[Their words if stated; otherwise "DEFAULT: where do things stand and what do I do."]
```

Chained runs append a new dated brain-dump section; boundary and players are updated in place if they changed.

---

## 01-SOURCES.md

```markdown
# Source Log — [Subject]  (cumulative)

| # | Source | Type | Origin | Span | What it is (1 line) | Status | Run |
|---|---|---|---|---|---|---|---|
| 1 | email thread w/ Scotty | thread | Gmail MCP | 06/12–07/09 | Project main thread | acquired | 1 |
| 2 | reader dump 07/11 | recollection | Phase 0 | — | Brain dump | acquired | 1 |

**Gaps / unavailable:** [source — why — what was suggested to obtain it. These become known unknowns.]
**Nothing extractable:** [sources processed in Phase 2 that yielded no ledger entries]
```

---

## 03-ANALYSIS.md

```markdown
# Analysis — [Subject] — Run [N], [date]

## State of play
| Workstream / deliverable | Status | Basis |
|---|---|---|
| Contact form fix | claimed done (unverified) | L-04 vs L-05 |

## Open loops (oldest first)
| Who owes | Owes whom | What | Opened | Age |
|---|---|---|---|---|
| Scotty | Demetrious | CRM credentials | L-02, 06/14 | 27d |

## Contradictions
| # | Claim A | Claim B | What hangs on it |
|---|---|---|---|
| C-1 | form fixed [L-04] | still failing [L-05] | launch readiness |

## Dropped balls
- [ASKED/PROMISED with no follow-through found] [L-ID]

## Unknowns
- [question no source answers / gap from unavailable source]

## Delta since SITREP-[N-1]  (chained runs only)
- Closed: … · Opened: … · Status changes: … · Contradictions resolved: …
```

Rewritten fresh each run (prior analyses are preserved in the numbered SITREPs).
