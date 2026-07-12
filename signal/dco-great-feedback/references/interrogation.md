# Interrogation Reference

How to turn vague reactions into legible feedback. Read before Phase 2.

## Tripwire vocabulary

These words/patterns can NEVER be logged as final feedback. They trigger an automatic probe. The list is illustrative, not exhaustive — the test is: *could two reasonable people picture completely different outcomes from this sentence?* If yes, it's a tripwire.

**Empty intensifiers:** better, more, less, stronger, weaker, elevated, next-level, "make it pop", punchier, cleaner, tighter, fresher, bolder, softer.

**Unanchored style words:** modern, classic, premium, luxury, professional, corporate, fun, playful, edgy, minimal, sleek, warm, cool, timeless, trendy, organic, techy.

**Comparison-by-gesture:** "like a New York company", "like Apple", "like the big guys", "more startup-y", "less agency-ish", "you know, like those sites".

**Feeling-only reactions:** "something's off", "it's not quite there", "I don't love it", "it feels cheap", "it's just not us".

**Scope fog:** "the whole thing", "everything", "the vibe overall", "just generally".

Objective statements bypass tripwires entirely: "the phone number is wrong", "logo is pixelated at small sizes", "this violates the spec's 3-color limit" — log and move on.

## Probe patterns

Use the lightest probe that works. One question at a time, always.

**1. Narrow the target.** Vague scope → pin the element. "When you say the whole thing feels off — is it strongest on the homepage, the logo, the color system, or the copy? Point me at the worst offender." Cite the structure map in 00-SUBJECT.md ("page 34, the color system") so the giver can react to specifics.

**2. Split reaction from direction.** People compress "I don't like X" and "I want Y" into one mumble. Separate them: "Two different things — what's wrong with what's there, and separately, what would right look like? Start with the first."

**3. The disguised five-whys.** Never ask "why?" five times — that's an interrogation cell. Instead, each answer becomes the premise of a more specific question:
- "It feels cheap." → "Cheap how — flimsy like a template, or loud like a used-car ad?"
- "Loud." → "Is it the colors shouting, the type, or how crowded it is?"
- "The colors." → "If the colors calmed down, does the rest hold up?"
You're descending from feeling → element → attribute → threshold. Three to four levels usually hits bedrock (the actual why). Stop when the giver's answer would let a stranger reproduce the judgment.

**4. Offer options to react to.** The single most effective move. When the giver reaches for a gesture ("like New York"), do the research (below) and return 2–4 concrete, *deliberately contrasting* candidates: "These three NY brands look nothing alike — brutalist B2B, warm editorial, loud streetwear. Which is closest?" Picking is 10x easier than articulating. Their pick, plus what they say about it, IS the feedback.

**5. The negative probe.** When positives stall, invert: "Show me or name something that's definitely NOT what you want." The boundary defines the territory.

**6. The stakes probe.** For priority disputes or fuzzy items: "If the maker changed nothing about this, is the project sunk, dented, or fine?" Maps directly to must / should / consider.

## Research protocol

Research proactively — this is where you do everything in your power to help.

- **When:** any comparison-by-gesture, any named brand/place/style you should verify, any claim about what's standard in an industry, any time candidates-to-react-to would unstick the giver.
- **How:** web search + image search. Find real, current examples. Prefer contrast — candidates that differ from each other force a revealing choice.
- **Return format:** short. Name each candidate, one line on what defines it visually/tonally, then the single question: "Which is closest — or is it none of these?"
- **Always confirm:** "Here's what I found based on what you told me — does this sound right?" Research is a hypothesis, not a conclusion. Never log researched interpretations without the giver's confirmation.
- Log confirmed research findings (with links) in 03-EVIDENCE.md like any other evidence.

## The echo-check

Before any item is logged `confirmed`, restate it in this exact shape and get an explicit yes:

> **So, confirming:** [Target — file/page/element]. Your reaction: [reaction]. Because: [the why]. What you want instead: [direction]. Backed by: [evidence names]. Priority: [must/should/consider]. — Did I get it?

If they correct anything, incorporate and echo again. Only a clean yes gets logged. Record the echo text verbatim in 02-ITEMS.md — it becomes the item's canonical wording.

## Handling the difficult cases

- **The rusher** ("just write it up"): offer the deal once — "Two more minutes of questions saves the maker a full wasted revision round." If they still refuse, take the override, tag hunches, ship honestly.
- **The contradictor** (examples pull apart): never say "these conflict, pick one." Say the examples differ, then hunt the common thread: "What do all of these have that the current work doesn't?" The thread is usually an attribute (warmth, density, confidence) hiding under surface differences.
- **The prescriber** (gives implementation orders: "tell them to use Cloudflare", "here are prompts for their AI"): capture the underlying need, strip the prescription. "What's the outcome you want from that?" The outcome goes in the item; the prescription goes nowhere, unless the giver insists — then it goes in FEEDBACK.md's Expert's Call section explicitly labeled as a suggestion the maker may ignore.
- **The pleaser** (agrees with every echo instantly): spot-check once — re-echo one item with a small deliberate error. If they wave it through, slow down and re-verify the batch.
