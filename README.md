# Stoeckle History

A version-controlled family history knowledge base for the Seehafer and Stoeckle families. Content is stored as Markdown with YAML front matter so it can be published as a Quartz static site while remaining easy to edit locally.

## Add new content
- People: copy `content/people/_template.md` to a new file in `content/people/` and fill it out.
- Places: copy `content/places/_template.md` to a new file in `content/places/` and fill it out.
- Sources: copy `content/sources/_template.md` to a new file in `content/sources/` and fill it out.
- Research notes: copy `content/research-log/_template.md` to a new file in `content/research-log/` and fill it out.

## Quartz publishing
Quartz reads from the `content/` directory at the repo root, so there is a single source of truth for the site content (no duplication or symlinks required).

### Local preview
1) `npm install`
2) `npx quartz build`
3) `npx quartz serve`

### GitHub Pages
1) Set `baseUrl` in `quartz.config.ts` to your `username/repo` (or custom domain).
2) Run `npx quartz build` and publish the `public/` output directory.
3) In GitHub Pages settings, set the source to the `public/` directory on your chosen branch.

## Privacy guidance
Avoid posting sensitive information about living people. If a person might be living, set `privacy.living: true` and keep the page private or omit sensitive facts in public builds.

## Publishing Checklist
- `git init` (if needed)
- `git add .` and `git commit -m "Initial import"`
- Create a GitHub repo and add the remote
- `git push -u origin main`
- Enable GitHub Pages in repo settings
- Set `baseUrl` in `quartz.config.ts` and redeploy
