# Spike 🎯

> *"See you, space cowboy."* — Spike Spiegel

**Autonomous Multi-LLM Bounty-Hunting System**

Spike is a true multi-agent system that discovers open-source security bounties, audits repositories for vulnerabilities, generates AI-powered fixes, and submits PRs — all without human intervention.

## Architecture

```
┌──────────────┐ ┌──────────────┐ ┌──────────────┐ ┌──────────────┐
│   Planner    │→│   Auditor    │→│    Fixer     │→│  Validator   │
│  (DeepSeek)  │ │  (Semgrep+)  │ │ (Claude/SF)  │ │  (DeepSeek)  │
└──────────────┘ └──────────────┘ └──────────────┘ └──────────────┘
```

## Quick Start

```bash
npm install
cp .env.example .env   # Add GITHUB_TOKEN
./bin/spike discover   # Find bounty opportunities
./bin/spike scan owner/repo  # Security audit
./bin/spike pipeline owner/repo  # Full multi-agent pipeline
```

## Proven Results

| Target | Findings | Action |
|--------|:--------:|--------|
| SolFoundry/solfoundry | 5 critical, 10 high | ✅ PR #1232 merged-eligible |
| expressjs/express | 12 high | Security report |
| nodejs/node (200K★) | 809 high, 12 medium | Full audit report |

## Built for Locus Paygentic Hackathon

Spike demonstrates Locus's vision: **agents that are the business, not just tools**. Spike autonomously generates revenue by finding, fixing, and claiming security bounties across open-source ecosystems.

## License

MIT
