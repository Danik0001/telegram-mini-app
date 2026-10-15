# ASIQPAI — Telegram Mini App UX/UI

A music creation experience for artists: a cohesive visual system, clearer navigation, and a mobile studio workflow built around the observed MVP.

**[View case study ↗](https://danik0001.github.io/telegram-mini-app/)** · **[Try interactive prototype ↗](https://danik0001.github.io/telegram-mini-app/prototype-standalone.html)** · **[Browse all screens ↗](https://danik0001.github.io/telegram-mini-app/gallery.html)** · **[Presentation PDF](ASIQPAI_Presentation.pdf)**

![ASIQPAI interface overview: Music, Library, Studio, vocal recording, Samples and Wallet](previews/overview.png)

> **Project status:** UX/UI concept and browser prototype. AI, audio recording/playback, WAV export and wallet connections are simulated. This is a portfolio case study; production integration and user research remain future work.

## The challenge

The brief called for a more consistent, premium interface for a fast-evolving Telegram Mini App. The design needed to make the primary AI Studio journey easier to understand while retaining Music, Library, Wallet and Community.

The existing MVP was reviewed before refining the concept. This changed the solution: Library remains a music catalog, Wallet uses TON/ASIQ, Community links to official channels, and the studio explains that recordings are not retained across launches.

## The solution

- **Five destinations:** Music / Library / AI Studio / Wallet / Community.
- **Vocal AI:** beat selection, independent MID/BACK/ADLIBS tracks, lyrics and teleprompter, recording/upload states, FX, mixing and export flow.
- **AI Samples:** BPM/key/bars/density/variant controls, results, favorites, quota and error states.
- **A single visual system:** dark surfaces, warm gold accents, consistent controls and component states.
- **Explicit limits:** permission denial, missing MID, upload constraints, processing failures and unsaved-session warnings.

| Deliverable | Scope |
|---|---|
| Main screens and states | 55 |
| Adaptive exports | 10 |
| Editable SVG files | 66, including UI Kit |
| Responsive checks | 55 screens × 4 browser widths |
| Demo interaction checks | 13 passed |

These counts describe the delivered materials and technical checks. They are not evidence of improved conversion or successful user testing.

## Explore the work

1. Start with the [case study](https://danik0001.github.io/telegram-mini-app/).
2. Open the [prototype](https://danik0001.github.io/telegram-mini-app/prototype-standalone.html) and use the five bottom tabs. The top screen selector is a review tool, outside the proposed product interface.
3. Explore [all screens](https://danik0001.github.io/telegram-mini-app/gallery.html), including errors and adaptive variants.
4. Read the [MVP traceability](MVP_TRACEABILITY.md), [user flows](IA_FLOWS.md) and [developer handoff](HANDOFF.md).

## Run locally

No build step, dependencies, API keys or account are required.

- Download this repository using **Code → Download ZIP**, extract it, and open `prototype-standalone.html` in a browser.
- For the modular source or the complete gallery, optionally run `python3 -m http.server 8000` from the repository directory and open `http://localhost:8000/`.
- Prototype state lives in memory and resets on page reload.

## Repository map

| Path | Purpose |
|---|---|
| `index.html`, `portfolio.css` | Public case study |
| `prototype-standalone.html` | Single-file interactive prototype |
| `prototype.html`, `prototype.css`, `prototype.js` | Modular prototype source |
| `design-manifest.json`, `design-data.js` | Screen content and browser data |
| `tokens.css` | Visual foundations |
| `screens/`, `adaptive/` | Browser PNG exports |
| `figma-import/` | Editable SVG screens and UI Kit |
| `assets/`, `previews/` | Concept artwork and project previews |
| `ASIQPAI_Presentation.pdf` | Six-page presentation |

## Validation and next steps

[QA report](QA_REPORT.md) documents responsive and simulated interaction checks. [USER_TESTING.md](USER_TESTING.md) defines a proposed study with at least five participants; that study has **not** been conducted. Real Telegram WebViews, microphone permissions, backend jobs, exported audio and TON transactions still need integration testing.

The current editable design handoff is SVG. SVG import does not automatically create native Figma Auto Layout, variables, component instances or prototype connections. The older native Figma file is not the source of truth for this version. See [technical notes](TECHNICAL_NOTES.md).

AI Fit / Vocal Slicer are proposals from the brief, not confirmed existing MVP behavior. Brand artwork is conceptual; beat licenses and original product assets are not included. See [asset notes](ASSETS.md).

## About this project

A portfolio project presented by [@Danik0001](https://github.com/Danik0001), developed with AI assistance for design exploration, prototype implementation and documentation. It does not imply official product ownership, endorsement, client acceptance or a production launch.

**По-русски:** это концепция редизайна ASIQPAI и интерактивный прототип по осмотренному MVP. Начните с демо и галереи; описание решения доступно в [SUBMISSION.md](SUBMISSION.md). Для вопросов по проекту можно открыть [issue](https://github.com/Danik0001/telegram-mini-app/issues).
