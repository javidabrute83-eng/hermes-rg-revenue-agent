# Hermes RG Revenue Agent

An AI-powered website design and research system for premium websites targeting card shops in the Raleigh-Durham area.

## 🎯 Purpose

This project combines autonomous AI agents, competitive intelligence, and scroll-driven animations to deliver high-impact websites for gaming and collectible card retailers.

## 🛠️ Features

- **Website Intelligence** — Automated competitive research, brand extraction, and site building
- **3D Animation Creator** — Apple-style scroll-driven video websites
- **NotebookLM Integration** — Research automation and content generation
- **Multi-LLM Support** — Claude, Gemini, DeepSeek 4 (switchable)
- **Telegram Bot** — Control Hermes on the go

## 🚀 Tech Stack

- **Hermes Agent** v0.14.0 (AI orchestration)
- **HTML/CSS/JavaScript** (no frameworks — fast & portable)
- **GSAP + ScrollTrigger** (scroll animations)
- **FFmpeg** (video frame extraction)
- **Firecrawl MCP** (web scraping)
- **Google NotebookLM** (research & generation)

## 📊 Installed Skills

### Productivity
- `website-intelligence` — Research-driven site builder with competitive analysis
- `notebooklm` — Google NotebookLM automation

### Creative
- `3d-animation-creator` — Scroll-controlled video websites
- `hyperframes` — Video compositions & animated titles
- `popular-web-designs` — 54 production design systems
- `architecture-diagram` — Cloud/infra diagrams
- `claude-design` — HTML design artifacts
- `excalidraw` — Hand-drawn diagrams
- `sketch` — Quick UI mockups

## 🔧 Configuration

- **LLM Providers:** Anthropic Claude (default), Google Gemini, DeepSeek 4
- **Gateway:** Telegram bot integration (live)
- **API Keys:** Configured in `~/.hermes/.env`
- **Hermes Location:** `/home/hermeswebui/.hermes/hermes-agent/`

## 📋 Project Structure

```
workspace/
├── hermes-rg-revenue-agent/     ← This repo
│   ├── README.md
│   ├── projects/                ← Website projects
│   │   └── [client-name]/
│   │       ├── research/        ← Brand & competitor analysis
│   │       ├── site/            ← Built website
│   │       └── competitive-analysis.html
│   └── .gitignore
└── apify_client.py              ← Web scraping helper
```

## 🎬 Workflow

1. **Website Intelligence** — Input client URL → outputs brand snapshot + competitor analysis + build brief
2. **Design Approval** — Review brief with client
3. **Build** — Create premium site with scroll animations
4. **3D Animation Creator** — (Optional) Build scroll-stop video showcase
5. **Deploy** — Push to Vercel/Netlify

## 🔐 Security

- Personal access token stored in `~/.git-credentials` (600 perms)
- API keys in `.env` (not committed)
- `.gitignore` excludes sensitive files

## 📞 Support

For issues or feature requests, open an issue in this repo.

---

**Created:** May 2026  
**Status:** Active Development
