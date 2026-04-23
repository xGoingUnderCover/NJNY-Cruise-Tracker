# NY & Cape Liberty Cruise Tracker

A clean, standalone HTML page tracking 2026 cruise departures from the New York / New Jersey area — including Cape Liberty (Bayonne, NJ), Manhattan, and Brooklyn.

## Features

- 55+ sailings across Royal Caribbean, Celebrity, Norwegian, Cunard, and MSC
- Filter by port, month, cruise line, or destination
- Full-text search across ships, lines, ports, and itineraries
- Live summary stats (sailings, ships, lines, avg nights)
- Fully responsive — works on mobile

## Usage

No build step. No dependencies. No server needed.

1. Clone or download this repo
2. Open `index.html` in any browser

Or host it free with **GitHub Pages**:

1. Push this repo to GitHub
2. Go to **Settings → Pages**
3. Set source to `main` branch, `/ (root)`
4. Your tracker will be live at `https://yourusername.github.io/repo-name`

## Data

Sailing data is hardcoded from publicly available 2026 schedules sourced from:
- [NYCruiseInfo.com](https://www.nycruiseinfo.com)
- [CayoleCruises.com](https://www.cayole.com)
- Royal Caribbean, Celebrity, Norwegian, Cunard, and MSC official sites

> **Note:** Always verify dates and availability directly with the cruise line or a travel agent before booking. Schedules are subject to change.

## Updating the Data

All sailings live in the `CRUISES` array inside `index.html`. Each entry follows this format:

```js
{ date:"2026-05-15", ship:"Oasis of the Seas", line:"Royal Caribbean", port:"cape", nights:7, dest:"Bahamas", itinerary:"Port Canaveral, CocoCay, Nassau" }
```

Port values: `cape` · `manhattan` · `brooklyn`

Destination values: `Bahamas` · `Bermuda` · `Caribbean` · `Europe` · `Canada & NE`
