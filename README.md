# Little Bloom Minds — devanypuente.lucraft.com.mx

Prototype v7 published as a static site on Cloudflare Pages (no build, no backend).

- `public/index.html`: the assembled prototype (`build/page7-assembled.html`) with two technical fixes only:
  1. HTML wrapper (`<!doctype html>`, `lang="es-MX"`, `<meta charset="utf-8">`, `<meta name="viewport">`) that the Claude Artifact host used to add.
  2. Download fallback in `saveDoc()` (Blob + `<a download>`) replacing `window.claude.use('downloads')`.
- Content, design and behavior are unchanged.
- Avatars, board, agenda and routine are stored in each visitor's browser (localStorage).
- Community forums need a backend that does not exist here, so they show the "access required" notice.

## Cloudflare Pages settings
| Setting | Value |
|---|---|
| Framework preset | None |
| Build command | (empty) — if required, `exit 0` |
| Build output directory | `public` |
| Custom domain | `devanypuente.lucraft.com.mx` |
