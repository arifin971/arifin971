# Arifin | Sportinerd LLC

> Building the most advanced FPL analytics & livescore platform on the planet.

## Live Stack

| Engine | Status |
|--------|--------|
| xPts Engine v4 — Poisson xGoalPts + Bivariate P(Haul) + DGW | Live |
| FDR Engine v3 — Position-aware EWMA, 6 modes | Live |
| Score Oracle v5 — Dixon-Coles match prediction | Live |
| MCS Track A — Manager Credibility Score (Bayesian) | Live |
| Momentum Engine — EWMA warm-bootstrap Opta-capped | Building |
| MiroFish v3 — Neuro-symbolic FPL solver (OR-Tools MILP) | Building |
| SLIE Engine — Sportinerd Live Intelligence Engine | Live |
| Match Centre v200 — Real-time xG + winprob + lineups | Building |

## Tech Stack

```
Backend   Python 3.9/3.12 · Node.js 20 · FastAPI · Fastify · Starlette
Database  PostgreSQL · Redis 29K+ keys · 59+ tables
ML/AI     Ollama qwen3:8b · Groq Whisper · Poisson · EWMA · Dixon-Coles
Data      GoalServe · FanDuel · FPL API · TransferMarkt · Sofascore
Infra     Servarica + DigitalOcean · WireGuard · PM2 · systemd · Prefect
Frontend  Next.js 14 · React · Tailwind · JetBrains Mono
```

## Infrastructure

```
Servarica (Primary Compute)          DigitalOcean (Stateless Edge)
├── PostgreSQL slie_db (59+ tables)   ├── GoalServe IP-whitelisted scraper
├── Redis 29K+ keys                   ├── F-series pipeline F01-F43
├── Ollama qwen3:8b                   ├── FastAPI livescore API
├── PM2 Node.js services              ├── systemd Python daemons
└── Next.js :3001                     └── WireGuard tunnel to Servarica
```

![Stats](https://github-readme-stats.vercel.app/api?username=arifin971&show_icons=true&theme=chartreuse-dark&hide_border=true&bg_color=001F1E&title_color=00e65b&icon_color=00e65b&text_color=ffffff)
![Streak](https://github-readme-streak-stats.herokuapp.com/?user=arifin971&theme=dark&hide_border=true&background=001F1E&ring=00e65b&fire=00e65b&currStreakLabel=00e65b)

---
*Sportinerd LLC — UAE | 18 years FPL | Building since 2025*
