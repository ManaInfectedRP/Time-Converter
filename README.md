# Time Converter

A live, browser-based time converter showing current time across every IANA timezone — no install, no backend, pure HTML/JS.

## Features

- **Live clocks** — all timezones update every second
- **Local time hero** — your PC's current time displayed prominently
- **600+ timezones** — full IANA timezone database via `Intl` API
- **Search** — filter by city, region, or country name
- **Region filters** — Africa, Americas, Asia, Australia, Europe, Pacific
- **UTC offset** — shown per card (e.g. `UTC+5:30`)
- **Offset diff** — how far each zone is from you (e.g. `+5:30h from you`)
- **Day badges** — highlights when a timezone is `+1 day` or `−1 day` ahead/behind
- **Copy to clipboard** — hover a card and click copy to grab the time + date + timezone

## Usage

Open `index.html` directly in any browser — no build step required.

## Deploy on Render

This repo includes a `render.yaml` for one-click static site deployment.

1. Push to GitHub
2. Go to [dashboard.render.com](https://dashboard.render.com) → **New** → **Blueprint**
3. Connect this repo — Render auto-detects `render.yaml` and deploys

## Tech

- Vanilla HTML / CSS / JS
- [`Intl.supportedValuesOf('timeZone')`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Intl/supportedValuesOf) for the full timezone list
- [`Intl.DateTimeFormat`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Intl/DateTimeFormat) for formatting — no external dependencies
