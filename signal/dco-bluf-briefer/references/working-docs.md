# Working Document Templates

Everything in `working/`. Fill every field; write "none" or "default" rather than omitting. A fresh session with zero conversation history must continue perfectly from these docs — write for that reader.

---

## STATE.md

```markdown
# Session State — [Brief Slug]
Started: [date] · Reader: [name/role if known] · Material from: [sender if known]

| Phase | Status | Completed | Note |
|---|---|---|---|
| 0 — Reader profile | not started / in progress / done | [timestamp] | [one line] |
| 1 — Acquisition | ... | | [e.g. "6 sources acquired, loom transcript unavailable"] |
| 2 — Digest | ... | | [e.g. "4 of 6 sources processed"] |
| 3 — Triage | ... | | |
| 4 — Brief | ... | | |

**Next action:** [always current, always specific — "Process proposal.pdf (source 5 of 6), then screenshots"]
```

---

## 00-READER.md

```markdown
# Reader Profile — [Brief Slug]

- **The material (reader's one-liner):** [what they said it is / "skipped"]
- **From:** [sender + relationship / "unknown"]
- **Reader's situation:** [deadline, pressure, state / "skipped"]
- **Standing question:** "[their exact words]"  — OR — "DEFAULT: What requires my action or decision, and is anything wrong?"
- **Anything else they said up front:** [verbatim fragments worth keeping / none]
```

---

## 01-SOURCES.md

```markdown
# Source Log — [Brief Slug]

| # | Source | Type | Origin | Size/length | What it is (1 line) | Status |
|---|---|---|---|---|---|---|
| 1 | loom-transcript.txt | transcript | pasted in chat, saved to file | ~15 min | Sender walkthrough of the new site | acquired |
| 2 | proposal.pdf | pdf | folder | 15 pp | Project plan | acquired |

**Gaps / unavailable:** [source + why + what was done about it — these become "known unknowns" in the brief]
**dco-great-feedback package detected:** [yes/no — if yes, path]
```

---

## 02-DIGEST.md

```markdown
# Digest — [Brief Slug]

## DECISIONS
- [item, 1–2 sentences] [source pointer(s)]

## PROBLEMS / RISKS
- ...

## ASKS (incl. buried)
- [item] [pointer] (buried: [where/how it was hidden, e.g. "aside at ~11:20 of loom"])

## DEADLINES / DATES
- ...

## OPEN QUESTIONS
- ...

## FYI
- ...

## Source coverage
| Source # | Processed | Note |
|---|---|---|
| 1 | ✓ | 3 items extracted |
| 2 | ✓ | nothing extractable |

## Drill-down log (post-brief)
- [question asked → answer given → pointer]
```

Pointer formats: `[loom-transcript ~11:20]` · `[proposal.pdf p.4]` · `[email 07/09]` · `[screenshot-03.png]` · `[FEEDBACK.md item 2]`. Every item has at least one. Merged duplicates carry all pointers.

---

## 03-TRIAGE.md

```markdown
# Triage — [Brief Slug]

**Standing question:** "[from 00-READER.md]"
**Answer to it:** [explicit, one or two sentences]

**Verdict line:** [the whole situation in one sentence]

**Situation paragraph:** [2–4 sentences — what this material is, state of things, impact]

## Item verdicts
| Digest item | Verdict | Why (one line) |
|---|---|---|
| [item] | ACT NOW / DECIDE / CAN WAIT / FYI | [reason, weighed against the standing question] |

**Cut from the brief (over the ceiling):** [items demoted to "Also logged" or working-docs-only, with reason]
```
