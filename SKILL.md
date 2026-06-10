---
name: x-content
description: >
  Create and optimize X (Twitter) content for @DevPandex — bios, pinned threads,
  weekly posting plans, single posts, reply drafts, and profile audits. Uses
  Abhishek Panda's brand voice, Human Filter positioning, and $10k build-in-public
  goal. Use when the user runs /x-content, asks for Twitter/X posts, content
  calendar, bio rewrite, pinned thread, build-in-public content, or social growth
  help for @DevPandex.
metadata:
  short-description: "X content for @DevPandex — posts, bios, threads, plans"
argument-hint: "[bio | thread | week | post | audit | reply] + optional topic"
---

# X Content — @DevPandex

Create ready-to-post X content for **Abhishek Panda** (@DevPandex).

## Before writing

1. Read `references/brand-profile.md` for identity, links, voice, and constraints.
2. Read `references/content-templates.md` for bios, thread skeletons, weekly plan, and post formats.
3. If the user names a mode (`bio`, `thread`, `week`, `post`, `audit`, `reply`), follow that mode. Otherwise infer from their request.

## Output rules

- Deliver **copy-paste-ready** posts. No placeholders like "[insert here]" unless the user must supply a real number they haven't given yet — then mark it clearly once, e.g. `$[your revenue]`.
- Every original post recommendation must include a **media suggestion** (screenshot, screen recording, demo GIF, or poll).
- Keep bios under **160 characters**.
- Lead with **Human Filter** as the hero product. Do not promote Readme generator in bio or pinned content unless the user explicitly asks.
- Tone: honest, specific, slightly self-deprecating, builder energy. Avoid generic "building in public" filler.
- Never invent metrics (followers, revenue, beta signups). Ask once if missing, or use clearly labeled placeholders.
- Include a **CTA** on product posts: `human-filter-landing.vercel.app`

## Modes

### `bio` — Rewrite profile bio
- Output **3 bio options** (product-first, story-first, problem-first) from templates.
- Recommend one with a one-line rationale.
- Remind: one link only, remove secondary project links from bio.

### `thread` — Pinned or standalone thread
- Default: Human Filter pinned thread (7 tweets) from templates.
- Customize if user gives a topic (build log, $10k journey, feature launch).
- Structure: hook → problem → solution → how it works → privacy/trust → CTA → follow reason.
- Tweet 1 must work as a standalone pin. Suggest attaching demo video to tweet 1 or 4.

### `week` — 7-day posting plan
- Output Mon–Sun plan from templates, customized to user's current week focus.
- Each day: post type, draft copy, media note, goal.
- Include weekly mix rule: **5 originals, 1 thread, 1 recap**; max **3–5 thoughtful replies/day**.

### `post` — Single post
- Ask what type if unclear: problem, build log, hot take, beta CTA, $10k update, recap.
- Output 1–3 variants (short, medium with hook).
- Suggest best time to post and whether to quote-tweet the pinned thread.

### `audit` — Profile critique
- Pull public profile data if possible via `web_fetch` or shell (`api.fxtwitter.com/DevPandex`, `api.vxtwitter.com/DevPandex`).
- Compare against brand profile targets (followers, media ratio, bio clarity).
- List top 3 gaps and top 3 fixes. Be direct, not harsh.

### `reply` — Reply drafts
- User provides the tweet/thread to reply to (paste or URL).
- Draft 2–3 reply options: value-add, story tie-in, soft product mention (only when relevant).
- Replies must not feel spammy. Human Filter mention only when the parent post is about AI spam, feeds, or indie building.

## Content pillars (rotate across the week)

1. **Problem** — AI reply spam, feed fatigue, bot noise
2. **Build log** — specific shipped thing + media
3. **Hot take** — contrarian angle on AI/social platforms
4. **$10k journey** — real numbers, wins, failures
5. **Beta CTA** — waitlist push with social proof ask
6. **Educational thread** — e.g. "signs a reply is AI-generated"
7. **Weekly recap** — metrics + next week focus

## Quality bar

Reject your own draft if it could be posted by any random dev account. Every post needs at least one of:
- A specific product detail
- A real number or date
- A personal story beat
- A visual/demo reference
- A question that invites replies

## After delivering content

End with a short **"post today"** action: the single highest-leverage thing to publish or update right now (usually: pin thread, update bio, or post Day 1 problem post).
