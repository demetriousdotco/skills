# Ledger & Analysis Doctrine

How the log of truth is built and read. Read before Phase 2; the analysis section governs Phase 3.

## LOG.md format

```markdown
# Log of Truth — [Subject]
Cumulative, append-only. Entries in chronological order. Claims are recorded as claims.

| ID | Date | Actor | Event | Source(s) |
|---|---|---|---|---|
| L-01 | 06/12 | Demetrious | SENT proposal + scope for site rebuild | [email 06/12] |
| L-02 | 06/14 | Scotty | DECIDED to proceed; PROMISED CRM credentials "this week" | [email 06/14] |
| L-03 | 06/23 | Demetrious | ASKED (2nd time) for CRM credentials | [email 06/23] |
| L-04 | 07/02 | Kyle | CLAIMED DONE: contact form fix | [slack 07/02] |
| L-05 | 07/05 | Scotty | DISPUTED L-04 — form still failing on mobile | [thread 07/05] |
| L-06 | 07/10 | Reader | RECOLLECTION: believes a domain decision was made on the Zoom call, unsure | [reader dump 07/11] |
```

- **IDs are permanent** (`L-NN`). Analysis, SITREPs, and plans cite them. Never renumber.
- **Chronological, strictly.** Late-surfacing older material is inserted in its date position with a new ID and the note `[added run N]` — IDs need not be sequential by date, order in the table is.
- **One event, one line.** A long email can produce several entries (an ask, a decision, a claim). A thread of pleasantries can produce zero.
- **Merge duplicates:** the same event reported in two sources is one entry with both pointers.
- **Recollections are entries**, actor = Reader, marked RECOLLECTION — they carry the same weight as any unverified claim.

## Verb vocabulary

Use these, uppercase, so the ledger scans: **SENT · ASKED · PROMISED · CLAIMED DONE · DELIVERED · DECIDED · DISPUTED · FLAGGED · WENT SILENT · RECOLLECTION**. WENT SILENT is an inferred event — record it when a thread demonstrably stops after an open ask ("no reply found after L-03").

## Claims are not facts — the prime discipline

- CLAIMED DONE is not DELIVERED. DELIVERED requires evidence in a source (the file exists, the confirmation exists, a second party verified).
- Never write "the form was fixed." Write "Kyle CLAIMED DONE: form fix [L-04]; Scotty DISPUTED [L-05]; no verification found."
- Never silently resolve a contradiction by picking the likelier claim. Both go in the ledger; the contradiction goes to analysis; resolving it goes in the plan.
- Reader recollections get zero special authority — cross-check them against sources like anything else, and when a source contradicts a recollection, that's a contradiction entry, stated neutrally.

## Analysis doctrine (Phase 3)

Everything below derives from ledger entries and cites them by ID.

**State of play.** List each workstream/deliverable inside the boundary. Exactly one status each:
`done (verified)` · `claimed done (unverified)` · `in progress` · `blocked` · `not started` · `unknown`.
"Unknown" is an honest and common status — it feeds the plan ("verify X").

**Open loops.** Formula: *[who] owes [who] [what] — opened [L-ID, date] — [N] days old.* Sort oldest first. The reader appears in this list like anyone else, same neutral phrasing. An open loop closes only when a ledger entry shows delivery or explicit cancellation.

**Contradictions.** Side-by-side: claim [L-ID] vs claim [L-ID], one line on what hangs on the answer. Each contradiction must produce a plan action (verify / ask / test).

**Dropped balls.** ASKED or PROMISED with no subsequent DELIVERED/answer in any source. Distinct from open loops only in tone of finding — they usually become the plan's first items.

**Unknowns.** Questions no source answers + gaps from `unavailable` sources ("the 06/28 Zoom wasn't transcribed — the domain decision may live there [re: L-06]").

**Delta (chained runs).** Compare against the previous SITREP: loops closed / opened, status changes, contradictions resolved / new. Cite the entries that changed things.

## Plan doctrine (feeds Phase 4)

Every plan action must be:
- **Traceable** — cites the ledger/analysis item it resolves.
- **Concrete** — a person + a verb + a thing: "Reply to Scotty: confirm form fix or reopen [L-04/L-05]", "Verify: test the contact form on mobile [L-05]", "Send Kyle the domain decision [L-06 → verify against Zoom first]".
- **Prioritized** — order by: contradictions blocking work → oldest loops the reader owes → oldest loops owed to the reader (nudges) → verifications → everything else.
- **One screen.** More actions than fit → the tail collapses into "then: [one-liners]".

The plan tells the reader who to contact and about what. It does not draft the messages (out of scope, v1).
