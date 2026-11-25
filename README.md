# Analytics for Operations · DACMO 2026

**Lagos Business School · Developing Analytical Competence for Managing Operations**
Prof Bongo Adi · bongo.ai

Live site: **https://markanalytics.online/dacmo/**

Two 75-minute sessions on variability, feedback and decisions under uncertainty, taught through five live simulations built around the participants' own operations.

## What's here

| Path | What it is |
| --- | --- |
| `index.html` | Programme hub: learning arc, session plan, the five labs, downloads |
| `lab/` | Operations Simulation Lab (single self-contained HTML file; keys 0–5 switch labs; `#l1`–`#l5` deep-links) |
| `book/` | Participant Book, readable online (40-minute self-study route) |
| `downloads/` | Facilitator deck (53 slides, full speaker scripts), Participant slides (38), Participant Book PDF, offline lab file |
| `assets/` | bongo.ai hex mark, lab screenshots, social preview image |

| Lab | Idea | Context |
| --- | --- | --- |
| 1 · The 45-Minute Turnaround | Flaw of Averages, criticality index | SAHCO, Aero Contractors, Pilgrims Africa |
| 2 · The Gate / The Desk | Kingman's law, utilisation × variability | Dangote, Golden Sugar, LFZ, Fidelity Pensions, insurers |
| 3 · December Demand Shock | Bullwhip, feedback and delay | UAC Foods, Golden Sugar, Dangote, Everyday Group |
| 4 · The Asset Fleet | Weibull reliability, PM vs CBM economics | Seplat, Chevron, Shell, Sahara, PESO, NSPM |
| 5 · The Import Lifeline | (s, Q) policy, resilience premium | NSPM, Segilola, UAC Foods, Dangote |

## Deployment

Every push to `main` uploads the site to Hostinger over FTP (`.github/workflows/deploy.yml`).
One-time setup in **GitHub → Settings → Secrets and variables → Actions**:

| Name | Type | Value |
| --- | --- | --- |
| `FTP_SERVER` | secret | Hostinger FTP host (hPanel → Files → FTP Accounts) |
| `FTP_USERNAME` | secret | FTP username |
| `FTP_PASSWORD` | secret | FTP password |
| `FTP_TARGET_DIR` | variable (optional) | Defaults to `public_html/dacmo/` |

Then run **Actions → Deploy to markanalytics.online/dacmo → Run workflow** (or push any commit).

Branding: Lagos Business School palette (deep green `#06201A`, gold `#C8941F`, teal `#0B6B5E`), Calibri, bongo.ai hex motif, consistent across site, lab and decks.
