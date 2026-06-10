# grok-x-content-skill

A [Grok Build](https://x.ai/cli) skill that generates ready-to-post X (Twitter) content — bios, pinned threads, weekly plans, single posts, reply drafts, and profile audits.

Built by [@DevPandex](https://x.com/DevPandex) while growing [Human Filter](https://human-filter-landing.vercel.app/) and documenting a $0 → $10k indie dev journey.

## What it does

Run `/x-content` in Grok Build and get copy-paste-ready posts tuned to your brand voice.

| Mode | Command | Output |
|------|---------|--------|
| Bio rewrite | `/x-content bio` | 3 bio options (≤160 chars) |
| Pinned thread | `/x-content thread` | 7-tweet thread |
| Weekly plan | `/x-content week` | 7-day posting calendar |
| Single post | `/x-content post` | 1–3 post variants |
| Profile audit | `/x-content audit` | Gaps + fixes |
| Reply drafts | `/x-content reply` | 2–3 reply options |

## Install

### Option 1 — Copy to user skills (all projects)

```bash
# macOS / Linux
cp -r grok-x-content-skill ~/.grok/skills/x-content

# Windows (PowerShell)
Copy-Item -Recurse .\grok-x-content-skill C:\Users\<YOU>\.grok\skills\x-content
```

### Option 2 — Clone into skills directory

```bash
git clone https://github.com/abhishekpanda-dev/grok-x-content-skill.git ~/.grok/skills/x-content
```

Restart Grok Build or wait a few seconds — skills auto-reload when files change.

## Structure

```
x-content/
├── SKILL.md                      # Agent instructions
└── references/
    ├── brand-profile.md            # Voice, links, goals
    └── content-templates.md        # Bios, threads, weekly plan
```

## Customize for your account

1. Edit `references/brand-profile.md` — swap @DevPandex details for yours
2. Edit `references/content-templates.md` — update bios, CTAs, and templates
3. Update the `description` in `SKILL.md` frontmatter so auto-invocation matches your triggers

## Example prompts

```
/x-content week
/x-content post build log for my SaaS launch
/x-content thread about why I built this product
Write me a build-in-public post for today
```

## Built with

- [Grok Build CLI](https://x.ai/cli) — terminal AI coding agent from xAI
- [Grok Skills](https://docs.x.ai/build/skills) — reusable prompt packages

## Author

**Abhishek Panda** — [@DevPandex](https://x.com/DevPandex) · [GitHub](https://github.com/abhishekpanda-dev) · [Human Filter](https://human-filter-landing.vercel.app/)

## License

MIT — use it, fork it, adapt it for your own X growth.
