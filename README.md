# Nikita Zlobinets

**ERP developer** who ships production systems by day and **Telegram products** by night — with Cursor + Obsidian in the loop.

I build tools people can open in one tap: convert a Telegram sticker pack into Yandex Telemost, or turn a Letterboxd ZIP into a dark-theme chart pack.

| | |
| --- | --- |
| **Location** | Moscow · open to remote / hybrid / relocate |
| **Languages** | Russian (native) · English (C2) |
| **Focus** | ERP (VIP / SAP ABAP) · Cloudflare Workers · GitHub Actions · Python charts |
| **Contact** | [Telegram-friendly email on request] · GitHub issues on the bot repos |

**On this page:** [Try the bots](#-try-the-bots) · [Skills](#-skills) · [Work](#-work) · [Education](#-education) · [Connect](#-connect)

---

### Currently

- Building & polishing [@tg2tmbot](https://t.me/tg2tmbot) and [@lebxdbot](https://t.me/lebxdbot)
- ERP project work at Galaktika (VIP) for Autovaz & Spb Metro; AI-assisted delivery with Cursor
- Speaking internally on AI-assisted development

---

### Try the bots

Two public products. Pick one path and click through — that *is* the portfolio demo.

#### 1. Telegram2Telemost — [@tg2tmbot](https://t.me/tg2tmbot)

Yandex Telemost has no Telegram sticker import. The bot takes your pack and builds it in Telemost. Finished packs are announced in [t.me/tg2tm](https://t.me/tg2tm).

| Step | What you do |
| --- | --- |
| 1 | Open [@tg2tmbot](https://t.me/tg2tmbot) → `/create` |
| 2 | Send a pack name |
| 3 | Forward stickers **or** paste `t.me/addstickers/…` |
| 4 | `/done` — watch one progress card (“sticker N of M”) |

| Layer | Stack |
| --- | --- |
| Ingress | Telegram Bot API → Cloudflare Worker → KV queue |
| Build | GitHub Actions · Chromium/CDP · saved Yandex session · “Stickers” bot dialog |
| Media | WEBP→PNG 512×512 (≤512 KiB) · TGS→PNG (rlottie) · ≤150 stickers · WEBM skipped with a clear ask |

**Code:** [pretendless/Telegram2Telemost](https://github.com/pretendless/Telegram2Telemost)

#### 2. Letterboxd Stats — [@lebxdbot](https://t.me/lebxdbot)

Letterboxd gives a raw ZIP, not charts. The bot parses the export and sends HTML + PNG stats back to the same chat.

| Step | What you do |
| --- | --- |
| 1 | Export your data from Letterboxd (ZIP) |
| 2 | Open [@lebxdbot](https://t.me/lebxdbot) and send the ZIP |
| 3 | Wizard: defaults · customize · or paste a previous settings summary |
| 4 | Get a chart pack (watches & averages by year/genre/people/studios; ♥ / ≡ marks; optional top-review panel) |

| Layer | Stack |
| --- | --- |
| Ingress | Cloudflare Worker webhook `POST /lebxd` · KV session state |
| Build | GitHub Actions · Python · matplotlib · TMDB metadata |
| UX | Top size 1–100 (default 20) · average threshold default 4 · period · filters/search · optional 10-point display |

**Code + gallery:** [pretendless/LetterboxdStats](https://github.com/pretendless/LetterboxdStats)

---

### Skills

#### Languages & platforms

| Area | Tools |
| --- | --- |
| ERP | VIP (Galaktika/Atlantis) · SAP ABAP · HANA-aware work · MM / SD / FI / EHSM / HR |
| Web / bots | TypeScript · JavaScript · Cloudflare Workers · NestJS · Next.js |
| Data & charts | Python · SQL · PostgreSQL · MySQL · MS SQL · matplotlib |
| Systems | Git · GitHub Actions · Jira · Confluence · Cursor · Obsidian |

#### How I work

| Practice | In practice |
| --- | --- |
| AI-assisted delivery | Cursor on real client tasks; internal talks on AI in ERP work |
| Knowledge graph | Obsidian vaults linking product, client, and task contexts |
| Product ownership | End-to-end bots: UX copy, queues, deploy, ops commands |
| Collaboration | Strong teammate feedback on communication (Unicon recommendation letter available) |

---

### Work

#### Galaktika — VIP developer · Mar 2026 – present

Project ERP for **Autovaz** and **Spb Metro**: accounting / warehouse print forms / production & inventory. SQL/VIEW, Excel reports, FastReport, extension points, configurator & Support tools. From Sep 2026, tasks run through Cursor; Obsidian graph for Galaktika + client + workspace.

#### Unicon AP — SAP ABAP developer · Jun 2022 – Feb 2026 · grade K2

MVC/OOP ABAP on MM, SD, FI, EHSM, HR, ERP; ALV, dialogs, mail, Excel/Word/XML; standard extensions; HANA-aware; FIORI visualization on at least one project. **3 completed projects** with Jira/Confluence reporting. Example: atypical-deals reporting (maintenance views, search helps, RFC, versioned ALV, Excel via ZXLWB_WORKBENCH, XML via J3RFTAXREP, email). Management recommendation letter available.

---

### Education

| Year | |
| --- | --- |
| 2024 | B.Sc. ITMO University — 09.03.02 Information Systems & Technologies |
| 2017–18 | ITMO Olympiad winner (admission without competition); city/regional olympiad prizes (Informatics, Economics, English) |

---

### Connect

- Bots: [@tg2tmbot](https://t.me/tg2tmbot) · [@lebxdbot](https://t.me/lebxdbot) · channel [t.me/tg2tm](https://t.me/tg2tm)
- Repos: [Telegram2Telemost](https://github.com/pretendless/Telegram2Telemost) · [LetterboxdStats](https://github.com/pretendless/LetterboxdStats)
- Prefer Telegram / email for roles — open to full-time, part-time, project, internship · remote, on-site, hybrid

<!-- Optional later: shields.io badges, pinned repo screenshots, GH stats card — keep salary out -->

---