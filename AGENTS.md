# Jun documentation

The documentation site for [Jun](https://github.com/samarsheikh001/jun), built on [Mintlify](https://mintlify.com). Pages are MDX files with YAML frontmatter (`title`, `description`, optional `icon`); navigation lives in `docs.json`. Preview with `npx mint dev` (http://localhost:3000) and check links with `npx mint broken-links`.

The product's source is the `jun` repo (locally `../jun-desk-2`). Every claim here must match what the code does today: read the code, its `README.md` and `CLAUDE.md` before writing, and never document a feature from `docs/features.md` that isn't built.

## Readers

People who run a B2B SaaS and want a support desk on their own Cloudflare account: founders, support leads and their developers. Most pages are for an admin working in the desk; the widget's API, page actions, identity and the CLI are for developers.

## Terminology

- **Jun** (the product), **the desk** (one deployed install), **workspace** (one desk's data).
- **Widget** = the chat on the customer's site; **loader** = `widget.js`; **launcher** = the bubble, bar or island.
- **Visitor** before they're known, **contact** once identified, **customer** in general prose.
- **Teammate** / **agent** for people answering in the inbox; **the AI** for the AI agent.
- In the desk, procedures are called **Tasks** (files under `skills/`), tools are **Actions** (`tools/*.yaml`), cards are **Widgets** (`widgets/*.widget`), evals are **Tests**.
- **Hand off** / **handoff** (to a person).

## Style

- Active voice, second person, present tense. One idea per sentence. Plain words; no marketing tone.
- Sentence case headings. Bold for UI labels: **Settings → AI**. Code formatting for files, commands, keys and paths.
- Lead with what the reader does, then why. Use `<Steps>` for procedures, `<Tabs>` for alternatives, `<Note>`/`<Warning>`/`<Tip>` sparingly, `<CardGroup>` for next steps at the end of a page.
- Show real snippets (from the repo's templates and tests) instead of invented ones.
- Link between pages with root-relative paths (`/widget/install`).

## Content boundaries

- Don't document internal implementation (Durable Object names, D1 tables) except on `how-it-works` and where an admin needs it (secrets, limits).
- Sign in with ChatGPT is for the owner's own desk, per OpenAI's terms; say so wherever it appears.
- No launch, pricing or roadmap promises.
