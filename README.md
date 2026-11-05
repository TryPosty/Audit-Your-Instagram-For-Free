# Instagram Audit — a free Claude skill

Score your Instagram business profile out of 100 and get five prioritized fixes, in about five minutes.

No API keys, no account connection, no signup. You paste your bio and send two screenshots of your own Instagram Insights; Claude does the scoring. Everything stays in your Claude conversation.

---

## What it scores

| Category | Points | What it looks at |
|---|---|---|
| Engagement performance | 35 | Interaction rate against reach, trend vs last month, saves and shares, spread across posts |
| Posting consistency | 25 | How often you post, how recently, and how evenly |
| Profile optimization | 20 | Bio, link, call to action, profile photo, searchable name |
| Account growth | 15 | Follower growth, reach trend, follows per account reached |
| Content format mix | 5 | Reels, carousels and images — variety, not subject matter |

It scores only what you give it. Skip the screenshots and you still get a profile and consistency audit, with the score reported out of what was actually assessed — never a zero for data that was simply missing.

## Install

**Claude apps (web, desktop, mobile)** — download `instagram-audit.zip` from the [latest release](../../releases/latest), then go to Settings → Capabilities → Skills → Upload skill and select the zip.

**Claude Code** — clone into your skills directory:

```bash
git clone https://github.com/TryPosty/Audit-Your-Instagram-For-Free.git ~/.claude/skills/instagram-audit
```

Then start a conversation with:

> Audit my Instagram

## What you'll need

**Takes one minute — gets you the profile score (20 points)**
Your handle, your bio text, your link in bio, your display name.

**Takes three more minutes — adds consistency and format mix (30 points)**
The date and format of your last 12 posts. Screenshot your profile grid if that's easier.

**Takes three more minutes — adds engagement and growth (50 points)**
Two screenshots from the Instagram app:

1. Your profile → **Professional dashboard** → **Insights** → set range to **Last 30 days**
2. The same Insights area → **Followers**

Make sure the "vs previous 30 days" percentages are visible — several checks read them directly.

You need a professional account (Business or Creator) for the Insights screens. Switching is free and takes a minute in Instagram's settings. A personal account can still get the profile and consistency scores.

## Privacy

The skill runs entirely inside your Claude conversation. It sends nothing to any server, calls no API, and stores nothing. Your screenshots are handled by Claude under whatever terms already apply to your account — there is no third party in the loop, including us.

The skill will not scrape Instagram. It asks you for what it needs.

## What it won't do

- Audit ads or paid reach
- Compare you to competitors
- Guess at a metric you didn't give it
- Tell you to post five times a day if you've said you can manage two

## Built by

Built and maintained by [TryPosty](https://tryposty.net), which automates this same scoring against the Instagram API so you don't have to take screenshots every month. The skill is free, open source, and works perfectly well without us.

Found a check that scores wrong? [Open an issue](../../issues) — the rubric is in `references/scoring-rubric.md` and pull requests are welcome.

## License

MIT. Fork it, change the thresholds, ship it inside your own product.
