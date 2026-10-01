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

The website's Skills page is a gallery of **suites** (packages of skills), like articles: a hero image, a short pitch, and a click through to that suite's landing page. It does not list every individual skill, so it scales to any number of skills.

Everything is driven by one registry file in the website repo: `src/lib/skills.ts`.

- **A new skill in an existing suite:** add it to that suite's `skills` list. It appears on the suite's landing page with download and source links.
- **A new suite:** add a suite entry (slug, name, tagline, blurb, hero `image`, `date`, and its `skills`). It automatically gets a gallery card on `/skills` and a generated landing page at `/skills/<slug>`.
- **A suite that deserves a custom demo page** (like SIGNAL and RUSSIAN DOLLS): build the page under `src/app/skills/<slug>/` and set `page: "/skills/<slug>"` on the suite so the card links to it.
