# Contributing to Cyber-Workspace

Thanks for considering a contribution to this OSINT/pentest tools collection.

## Reporting an issue
- **Broken link** — open an issue with the file path and the dead URL.
- **Duplicate tool** — open an issue with both file paths.
- **Missing tool** — open an issue or a PR (see below) with the tool name, URL, and a one-line description.

## Adding a tool via PR
1. Find (or create) the matching category folder, e.g. `01-Recon-OSINT/Identity-OSINT/Email/`.
2. Split by `Online/` (browser-based service) or `GitHub/` (installable tool/repo).
3. Name the file with the pricing tier prefix:
   - `1-Gratuit - Tool Name.url` → free
   - `2-Freemium - Tool Name.url` → free tier + paid upgrade
   - `3-Payant - Tool Name.url` → paid only
4. File content must be a standard Windows internet shortcut:
   ```
   [InternetShortcut]
   URL=https://example.com
   ```
5. Open a PR. Keep one tool per file, no binaries, no scraped personal data.

## Scope
Only publicly available tools/services for **authorized** use (signed pentests, CTFs, in-scope bug bounty, personal labs). No exploit code, credentials, or stolen/scraped personal data.
