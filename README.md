# Zhuoxuan Huang — Personal Academic Site

This repo hosts the GitHub Pages site for Zhuoxuan Huang (zelo2.github.io), built with Jekyll on top of the Academic Pages/Minimal Mistakes theme.

## What’s inside
- Profile/about, CV, and publications (with citation-only rendering).
- News with recent acceptances.
- Auto-generated collections for publications under `_publications/`.

## Local preview
1) Install Ruby + Bundler + Node. On macOS:
   ```bash
   brew install ruby node
   gem install bundler
   ```
2) Install gems locally:
   ```bash
   bundle config set --local path 'vendor/bundle'
   bundle install
   ```
3) Serve locally:
   ```bash
   bundle exec jekyll serve -l -H localhost
   ```
   Then open http://localhost:4000.

### Docker (optional)
```bash
chmod -R 777 .
docker compose up
```
Site is available at http://localhost:4000.

## Deploy
Push to the repo; GitHub Pages (GitHub Actions) will build and publish to https://zelo2.github.io.

## Repo notes
- Publications live in `_publications/` (front matter drives the lists).
- Navigation is controlled via `_data/navigation.yml`.
- Site-level config is `_config.yml` (includes the base URL and publication categories).
