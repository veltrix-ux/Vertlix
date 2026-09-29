# Design notes

## Direction
Swiss (International Typographic Style) with a few dark, cinematic sections.

## Tokens
| Token | Value | Use |
| --- | --- | --- |
| `--bg` | `#fbfbf9` | Light page background |
| `--ink` | `#000` | Text and rules |
| `--red` | `#e30613` | The one accent: logo, live states, governance block |
| dark surface | `#080808` | Hero, feedback, app tour, heartbeats, costs |

## Type
Inter (Helvetica Neue and Arial as fallbacks). Weights 400, 600 and 700. Tight tracking on large headings.

## Layout
12-column grid, flush-left text, asymmetric two-column splits (5/7), hairline rules between sections.

## Motion
- Hero: gradient pill columns with film grain, slow parallax on scroll.
- Scroll reveals via IntersectionObserver.
- App tour: four scripted scenes on a 7-second loop.
- Heartbeats: 14-second CSS loop.
- Costs: counters and bars fill on view, then tick live.
- All motion is disabled under `prefers-reduced-motion`.
