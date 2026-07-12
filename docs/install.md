# Installing a skill

**Bottom line: one file, one drag, done. No code runs on your machine — a skill is a folder of instructions your Claude reads.**

## The normal path (Claude web / desktop)

1. **Turn on code execution** — Claude → Settings → Capabilities → **Code execution** → on. (Free accounts included.)
2. **Download** the `.skill` file from the [latest release](https://github.com/demetriousdotco/skills/releases/latest).
3. **Drag it into any Claude chat** and hit **Save skill**. Installed.

## Alternate path (uploader)

Claude → Customize → Skills → upload. If the uploader complains about the file type, rename `.skill` → `.zip` and upload that — they're the same file.

## Claude Code (terminal)

Unzip the file into your skills folder:

```bash
unzip dco-bluf-briefer.skill -d ~/.claude/skills/
```

## Using a skill

Don't summon it — just talk. Skills trigger themselves when the moment matches:

- *"brief me on this"* / *"what's in this folder?"*
- *"help me send feedback on this draft"*
- *"I need a sitrep on the Henderson project"*

## Good to know

- **Private to your account.** Each person installs their own copy — forward the file or the page freely.
- **Inspectable.** Every skill's full source is in this repo. Read it before you run it.
- **Updates.** New versions ship as new [releases](https://github.com/demetriousdotco/skills/releases); reinstalling is the same drag.

## Trouble?

Open an [issue](https://github.com/demetriousdotco/skills/issues) — include what you tried and what Claude said.
