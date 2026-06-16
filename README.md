# mvp-mini-etl-pipeline

> Visual ETL pipeline — extracts SpaceX launch data, transforms it through a step-by-step pipeline, and displays metrics with live re-run support.

A Next.js app that fetches real data from the SpaceX public API, runs it through a configurable pipeline of transformation steps (filter → enrich → aggregate), and presents the results alongside a visual pipeline trace and metrics panel. Falls back to local mock data when the API is unavailable.

## Features

- **Live data source** — pulls from SpaceX REST API; configurable URL via modal
- **Step-by-step pipeline** — each stage (extract, filter, enrich, aggregate) tracked with status and duration
- **Visual trace** — pipeline diagram shows pending / running / done / error per step
- **Metrics panel** — success rate, total launches, average payload, and trend over time
- **Re-run support** — trigger a fresh pipeline run without page reload
- **Graceful fallback** — switches to bundled mock data if API is unreachable

## Tech Stack

| Layer | Technology |
|-------|-----------|
| Framework | Next.js (Pages Router) |
| Data source | SpaceX API (public) |
| Styling | Inline styles (dark theme) |
| State | React hooks |

## Getting Started

```bash
npm install
npm run dev   # http://localhost:3000
```

## License

MIT
