<p align="center">
  <a href="assets/banner.svg"><img src="assets/banner.svg" alt="Vertlix: your AI crew, run like a company." width="100%"></a>
</p>

<p align="center">
  <a href="#quickstart"><b>Quickstart</b></a> ·
  <a href="#whats-on-the-site"><b>What's on the site</b></a> ·
  <a href="#deploy"><b>Deploy</b></a> ·
  <a href="CONTRIBUTING.md"><b>Contributing</b></a> ·
  <a href="ROADMAP.md"><b>Roadmap</b></a>
</p>

<p align="center">
  <a href="LICENSE"><img alt="MIT License" src="https://img.shields.io/badge/license-MIT-blue"></a>
  <img alt="No build step" src="https://img.shields.io/badge/build-none-lightgrey">
  <img alt="Static site" src="https://img.shields.io/badge/site-static-black">
</p>

# Vertlix

**Your AI crew, run like a company.**

Vertlix is an app for organising AI agents into a team with roles, goals, budgets and approvals. This repository contains the **Vertlix website**: a fast, static, animated landing page with a waitlist.

It is plain HTML, CSS and JavaScript. No framework and no build step to develop.

## What's on the site

| Section | What it shows |
| --- | --- |
| **Hero** | Gradient pill columns with film grain, headline and waitlist form |
| **Early feedback** | Two rows of sliding feedback cards (sample content) |
| **How it works** | Set the goal, build the team, approve and go |
| **App tour** | A scripted, animated walkthrough of the app in four scenes |
| **Features** | Bring your own agent, org chart, goal tracing, spending caps, audit trail, human sign-off |
| **Agents** | Animated org chart with an active agent and work moving down the chart |
| **Heartbeats** | Animated schedule showing agents waking on their own cadence |
| **Cost tracking** | Live budgets per agent that count up and tick |
| **Tickets and governance** | Traceable conversations and human approvals |
| **FAQ and install block** | Common questions and a one-line install example |

## Screenshots

<p align="center"><img src="screenshots/01-hero.png" alt="Hero with gradient pill columns and waitlist form" width="100%"></p>

| | |
| --- | --- |
| ![Early feedback](screenshots/02-feedback.png) | ![How it works](screenshots/03-how-it-works.png) |
| ![App tour: set a goal](screenshots/04a-app-tour-goal.png) | ![App tour: build the team](screenshots/04b-app-tour-team.png) |
| ![App tour: approve a hire](screenshots/04c-app-tour-approve.png) | ![App tour: watch the spend](screenshots/04d-app-tour-spend.png) |
| ![Features](screenshots/05-features.png) | ![Org chart](screenshots/06-org-chart.png) |
| ![Heartbeats](screenshots/07-heartbeats.png) | ![Cost tracking](screenshots/08-cost-tracking.png) |
| ![Governance](screenshots/09-governance.png) | ![FAQ](screenshots/10-faq.png) |

Mobile: [`screenshots/11-mobile-hero.png`](screenshots/11-mobile-hero.png) · Full page: [`screenshots/00-full-page.png`](screenshots/00-full-page.png)

Screenshots are captured with Playwright at 1440px wide. The site's web font loads from Google Fonts, so if you capture offline the text falls back to Helvetica or Arial.

## Quickstart

Requires Node.js 20 or newer (only for the local server).

```sh
git clone https://github.com/YOUR-USERNAME/vertlix.git
cd vertlix
npm run dev
```

Then open `http://localhost:3000`. You can also just open `index.html` in a browser.

## Project structure

```
.
├── index.html          # page content
├── css/styles.css      # tokens, layout, animations
├── js/main.js          # waitlist, app tour, counters, scroll reveals
├── assets/             # banner and favicon
├── screenshots/        # section screenshots used in this README
├── scripts/build.mjs   # copies the site to ./dist
├── .github/            # Pages deploy workflow, issue and PR templates
├── DESIGN.md
├── ROADMAP.md
├── CONTRIBUTING.md
└── LICENSE
```

## Customise

- **Name, copy and links:** edit `index.html`.
- **Colours and type:** change the tokens at the top of `css/styles.css`.
- **Early access date:** search for `Early access opens in 2027` in `index.html`.
- **Feedback cards:** the names, handles and quotes are **placeholders**. Replace them with real feedback (with permission) before launch.
- **Waitlist form:** it currently shows a confirmation and stores the address in the visitor's own browser only. Connect it to a form service or your backend in `js/main.js` (`join()`).
- **Install command:** the `npx vertlix init` example is a placeholder for a package you have yet to publish.

## Deploy

**GitHub Pages:** push to `main`. The included workflow in `.github/workflows/pages.yml` builds and publishes the site. In your repository, open Settings, then Pages, and set the source to GitHub Actions.

**Anywhere else:** run `npm run build` and upload the `dist/` folder to Netlify, Vercel, Cloudflare Pages or any static host.

## Notes on logos

The Claude, OpenAI, Gemini, Meta and Mistral marks are trademarks of their owners and are shown only to indicate compatibility. Vertlix is not affiliated with or endorsed by them.

## Contributing

We welcome contributions. See [CONTRIBUTING.md](CONTRIBUTING.md).

## License

MIT © 2026 Vertlix
