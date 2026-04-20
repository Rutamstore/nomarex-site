# NoMareX Corporate Website

Official corporate website for **NoMareX Holdings LLC** — a Texas-based brand house.

- **Primary domain**: nomarex.com (EN)
- **Korean subdirectory**: nomarex.com/kr
- **Legal entity**: NoMareX Holdings LLC (A Texas Limited Liability Company)

## Brands Featured
- **RUTAM** — Bio-functional scalp & hair resilience (rutam.store)
- **MarketLegion** — AI-powered market intelligence (marketlegion.ai)

## Project Structure
```
nomarex-site/
├── public/
│   ├── index.html              ← English (primary)
│   ├── kr/
│   │   └── index.html          ← Korean
│   └── images/
│       └── rutam/
│           ├── 01-philosophy-model.jpg
│           ├── 02-system-3products.png
│           └── 03-science-exosome.png
├── vercel.json                 ← Vercel deployment config
├── .gitignore
└── README.md
```

## Deploy to Vercel

### Option 1: Via GitHub (recommended)
```bash
# 1. Initialize git and commit
cd nomarex-site
git init
git add .
git commit -m "Initial commit: NoMareX v11 EN + KR with RUTAM product imagery"

# 2. Create GitHub repo and push (requires gh CLI authenticated)
gh repo create Rutamstore/nomarex-site --public --source=. --push

# 3. In Vercel dashboard → New Project → Import from GitHub
# 4. Connect custom domain: nomarex.com
```

### Option 2: Direct Vercel CLI
```bash
cd nomarex-site
vercel --prod
```

## Tech Stack
- **Static HTML** (no framework — fastest possible load times)
- **Typography**: Geist (Latin) + Pretendard (Korean)
- **Palette**:
  - Terracotta `#B8542C` (RUTAM primary)
  - Gold `#C9A227` (MarketLegion primary)
  - Dark `#0A0A0A`
- **Animations**: IntersectionObserver-driven reveals, CSS keyframe floats

## Backlog
- [ ] Governance page (`/governance`) — Corporate structure, leadership, IP ownership, compliance
- [ ] MarketLegion app screenshots (replacing Drive placeholder fallbacks in ML section)
- [ ] Privacy Policy page
- [ ] Terms of Service page
- [ ] Next.js migration (if dynamic routes or CMS needed)
- [ ] i18n library integration (if more languages added)

## Maintained By
NoMareX Holdings LLC · Texas, USA  
© 2026 All rights reserved.
