# Contributing

Thanks for helping improve the Vertlix website.

## Set up

```sh
git clone https://github.com/YOUR-USERNAME/vertlix.git
cd vertlix
npm run dev      # serves the site at http://localhost:3000
```

The site is plain HTML, CSS and JavaScript. There is no build step for development.

## Where things live

| Path | What it holds |
| --- | --- |
| `index.html` | All page content and structure |
| `css/styles.css` | Design tokens, layout, dark sections and animations |
| `js/main.js` | Waitlist form, app tour, cost counters and scroll reveals |
| `assets/` | Banner and favicon |

## Guidelines

- Keep the Swiss style: a grid, flush-left text, one red accent, square corners.
- Respect `prefers-reduced-motion`. Every animation needs a still fallback.
- Test on a narrow phone screen and in dark mode.
- Sample testimonials and numbers are placeholders. Do not add real people's names or quotes without their permission.

## Pull requests

Open a PR with a short description and a screenshot of any visual change.
