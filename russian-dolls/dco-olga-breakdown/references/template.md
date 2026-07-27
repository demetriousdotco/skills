# 02-BREAKDOWN.md template

Write the file exactly in this structure. The NOTE TO AI block is verbatim except
bracketed fields.

```markdown
> **NOTE TO AI:** This is level 2 of 4 of a Russian Dolls decomposition (broad to
> specific) for the project "[PROJECT NAME]". It defines THE BREAKDOWN: each
> workstream from 01-SHAPE.md cut into chunks with outcomes and crossings.
> REFERENCE 01-SHAPE.md for what the workstreams are — nothing here restates it.
> Deeper levels: 03-STEPS.md (executable steps), 04-PACKETS.md (per-person
> handoffs). To continue the chain, use the skill `dco-vera-steps` (or emulate it:
> turn each chunk into one-sitting executable steps with done-checks, grouped into
> sprints, with tool hints for the user's named tools).

# [PROJECT NAME] — The Breakdown
*Russian Dolls · level 2 of 4 · broken down [DATE] with Olga · shape: 01-SHAPE.md*

## Bottom line
[One sentence: how many chunks across how many workstreams, and the critical path.]

## WS-1 · [Workstream name]
| # | Chunk | Done means | Position |
|---|---|---|---|
| 1a | [name] | [observable outcome] | [blocked by … / unblocks … / ∥] |
| 1b | … | … | … |

[...repeat per workstream...]

## Crossings
| # | Dependency |
|---|---|
| X-1 | [WS-2/2a needs WS-4/4b — what and why, one line] |

## Client-side dependencies
[Chunks that wait on the client/stakeholder — approvals, assets, access.]

## Parked
[Unresolved items from the gate, with why — or "nothing parked."]

## Next doll
Vera (`dco-vera-steps`) — executable steps + sprints. Output: 03-STEPS.md.
```
