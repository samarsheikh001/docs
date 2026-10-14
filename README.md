# Jun Desk docs

Documentation for [Jun Desk](https://github.com/samarsheikh001/jun), the open-source AI support desk you deploy to your own Cloudflare account. Built with [Mintlify](https://mintlify.com).

## Preview locally

```sh
npx mint dev
```

Open http://localhost:3000. Check links with `npx mint broken-links`.

## Layout

| Folder | Section |
|---|---|
| `index.mdx`, `quickstart.mdx`, `how-it-works.mdx`, `get-started-checklist.mdx` | Get started |
| `deploy/` | Deploying, signing in, domains, upgrades, limits, local development |
| `widget/` | The website widget, identity, privacy, debug context, page actions, JavaScript API |
| `ai/` | Models, knowledge, instructions, tasks, actions, widgets, tests, handoff |
| `inbox/` | Inbox, notes, assignment, hours, notifications, issues, visitors, reports, team |
| `code/` | Agent as code: the `jun` CLI, file formats, CI |
| `reference/` | Loader options, secrets, security, troubleshooting, FAQ |

Navigation lives in `docs.json`; writing rules are in `AGENTS.md`.

## Publishing

With Mintlify's GitHub app installed, a push to `main` deploys the site.
