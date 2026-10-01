# Adding a skill

How a new skill gets from your head to the library and the website.

## 1. Write it

Create a folder inside a suite (or start a new suite folder):

```
<suite>/dco-<name>/
  SKILL.md            required: frontmatter (name, description) + the instructions
  references/         optional: templates and long reference docs the skill reads
```

Keep `SKILL.md` readable. Anyone should be able to open it and see exactly what their AI will do. Use the existing skills (e.g. `signal/dco-bluf-briefer/`) as the pattern.

## 2. Add it to the suite README

Each suite folder has a `README.md` with a table of its skills. Add a row: name, when it triggers, the bottom line, and the download link:

`https://github.com/demetriousdotco/skills/releases/latest/download/dco-<name>.skill`

## 3. Cut a release

A `.skill` file is the skill folder zipped with the folder as the top level. Each release carries one `.skill` per skill so the `latest/download/` links always serve the newest version of every skill.

```
zip -r dco-<name>.skill dco-<name>/
gh release create vX.Y.Z *.skill --title "Library vX.Y" --notes "What's new"
```

## 4. Put it on the website

The site lists skills from one registry file: `src/lib/skills.ts` in the website repo ([demetriousdotco/demetrious-consulting](https://demetrious-consulting.vercel.app/skills) project). Add the skill (or a new suite) there and it appears on the Skills page with its download and source links. A suite that deserves its own demo page gets a page under `src/app/skills/<suite>/`.
