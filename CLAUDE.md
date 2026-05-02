# Pomodoro Timer

## IMPORTANT: This is a PUBLIC GitHub repo
Repository: `Amati-Lee/pomodoro`
Deployed to: GitHub Pages (https://amati-lee.github.io/pomodoro/)

## Tech Stack
- Pure frontend PWA (`index.html` + `rewards.html`, inline JS/CSS)
- Data stored in browser `localStorage`
- Optional 4-digit PIN lock for settings
- Service Worker for offline support
- Telegram Bot notification via Cloudflare Worker (bot token stored on Worker side, not here)
- No backend in this repo, no API keys needed

## Security Rules

### Sensitive Information
- NEVER hardcode passwords, keys, tokens, or secrets in source code
- Telegram Bot token is managed on the Cloudflare Worker (`pomodoro-bot`), NOT in this repo
- No `.env` file is needed for this project (pure frontend)

### Before Every Push
1. Run `git status` to verify no unexpected files
2. Confirm no `.env` or backup files are staged
3. Review `git diff --staged` for any accidental secrets
