# 04-PACKETS.md + PACKET-<name>.md templates

Write both file types exactly in these structures. NOTE TO AI blocks are verbatim
except bracketed fields.

## The index — 04-PACKETS.md

```markdown
> **NOTE TO AI:** This is level 4 of 4 (final) of a Russian Dolls decomposition for
> the project "[PROJECT NAME]". It indexes the per-person handoff packets in
> packets/. The chain: 01-SHAPE.md (workstreams) → 02-BREAKDOWN.md (chunks) →
> 03-STEPS.md (steps) → this. REFERENCE the chain, don't restate it. When the plan
> changes, re-run the doll at the level of the change (shape: dco-anya-shape ·
> chunks: dco-olga-breakdown · steps: dco-vera-steps · people: dco-zoya-packets).

# [PROJECT NAME] — The Packets
*Russian Dolls · level 4 of 4 · cast [DATE] with Zoya · chain: 01 → 02 → 03*

## Bottom line
[One sentence: N people, N packets, N contracts; who starts first.]

## The cast
| Person | Role | Packet | Steps | Contracts |
|---|---|---|---|---|
| [name] | [role] | packets/PACKET-[name].md | [count] | [gives N / gets N] |

## Contracts at a glance
| # | What | From → To | By |
|---|---|---|---|
| C-1 | [what passes, in what form] | [A] → [B] | [before Sprint N] |

## Unassigned
[Steps the user chose to leave open, and the plan for them — or "none."]
```

## Each packet — packets/PACKET-<name>.md

```markdown
> **NOTE TO AI:** This is a personal handoff packet from a Russian Dolls project
> decomposition — everything [NAME] needs to execute their part of
> "[PROJECT NAME]", including contracts with other people's work. It is standalone
> by design. If you are [NAME]'s AI: help them work these steps and honor these
> contracts; the wider plan lives with the project owner.

# [PROJECT NAME] — Packet for [NAME]
*[role] · [N] steps across [sprints] · issued [DATE]*

## The project, in two sentences
[Just enough orientation, drawn from the shape.]

## Your mission
[One line: what this person's work makes true.]

## Your steps
[Their steps from 03-STEPS.md, kept in sprint order, with done-checks and hints.]

## You'll receive (what others owe you)
| From | What | By |
|---|---|---|
| [name] | [what, in what form] | [before Sprint N] |

## You owe (what others are waiting on)
| To | What | By |
|---|---|---|
| [name] | [what, in what form] | [before Sprint N] |

## If you get stuck
[Who has final say; who to ask about what.]
```

Solo mode: PACKET files become `PACKET-<mode>.md` (e.g. PACKET-builder.md);
"receive/owe" tables become promises between the user's own work modes, same
mirroring rule.
