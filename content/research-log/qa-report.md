---
type: research-log
id: "qa-report"
date: ""
subject: "QA Report"
status: "active"
question: "Is the site building and linked correctly?"
repositories: []
next_steps: []
---

# QA Report

## Build and Serve
- `npm install` completed with engine warnings (Quartz recommends Node >= 22).
- `npx quartz build` completed successfully and emitted output to `public/`.
- `npx quartz build --serve` started a local server at `http://localhost:8080` and was stopped after a brief check.

## Link Check
- Automated scan of `content/**/*.md` found no broken internal links.

## Search Index
- Search index generated at `public/static/contentIndex.json` during build.

## Ready to Share Checklist
- Local:
  - `npm install`
  - `npx quartz build`
  - `npx quartz build --serve`
- GitHub Pages:
  - Push repo to GitHub
  - Enable Pages
  - Set `baseUrl` in `quartz.config.ts`
  - Run the deploy workflow (or rebuild locally and publish `public/`)

## What's Missing
- Bertha A. Seehafer death certificate (1960)
- Katherine Friederike (Nufer) Stoeckle death certificate (1932)
- Probate packets (Clara, Ida, Bertha)
- Obituaries (Jackson Citizen-Patriot 1932; Ann Arbor News 1916/1948/1960)
