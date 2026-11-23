# FullStack AI Starter

The free sample of the **FullStack AI Business System** — an Offer Agent, 3 business-marketing skills and the `/offer` command for Claude Code. Research a niche, analyse competitors, and package an offer that sells — before you spend a dollar on ads.

> Part of the free FullStack AI Starter. Full system (6 agents, 39 commands, 47 skills, CMO Engine): https://hoangbio.gumroad.com/l/fullstack-ai-business-system — Guide: https://aifullstack.site/en/

## What's inside

| Component | Path | What it does |
|---|---|---|
| Offer Agent | `cli-tool/components/agents/business-marketing/offer-agent.md` | Runs the full offer workflow: research → competitor analysis → offer packaging |
| market-research skill | `cli-tool/components/skills/business-marketing/market-research/` | Validate a niche with customer data, demand signals and a 100-point scorecard |
| competitor-analysis skill | `cli-tool/components/skills/business-marketing/competitor-analysis/` | Map the competitive landscape and find gaps to position against |
| offer-packaging skill | `cli-tool/components/skills/business-marketing/offer-packaging/` | Build the offer stack, value ladder and pricing with psychology tactics |
| /offer command | `cli-tool/components/commands/marketing/offer.md` | One command that runs the whole workflow end to end |

Each skill ships with its reference files (checklists, frameworks and templates) under its `references/` folder.

## Install

### Option A — from the aitmpl catalog (once merged)

```bash
npx claude-code-templates@latest --skill business-marketing/market-research --skill business-marketing/competitor-analysis --skill business-marketing/offer-packaging --agent business-marketing/offer-agent --command marketing/offer
```

Status: submitted as [PR #1663](https://github.com/davila7/claude-code-templates/pull/1663) to the aitmpl catalog, awaiting maintainer review.

### Option B — manual install from this repo

```bash
git clone https://github.com/hoangvucr7bio/fullstack-ai-starter.git
```

Then copy the components into Claude Code (user level, or into your project's `.claude/` folder instead of `~/.claude/`):

```bash
# Skills
cp -r cli-tool/components/skills/business-marketing ~/.claude/skills/
# Agent
mkdir -p ~/.claude/agents/business-marketing
cp cli-tool/components/agents/business-marketing/offer-agent.md ~/.claude/agents/business-marketing/
# Command
mkdir -p ~/.claude/commands/marketing
cp cli-tool/components/commands/marketing/offer.md ~/.claude/commands/marketing/
```

Then in Claude Code, run `/offer` and follow the prompts.

## The full kit

This Starter is the free sample. The full **FullStack AI Business System** ($29) adds 6 agents, 39 commands and 47 skills, including the CMO Engine — market research, competitor analysis, offer packaging, content, pricing and more, on any AI coding agent (Claude Code, Antigravity, Codex, Grok, Muse).

- **Get the full kit ($29):** https://hoangbio.gumroad.com/l/fullstack-ai-business-system
- **Guide:** https://aifullstack.site/en/
- **Free Starter on Gumroad ($0):** https://hoangbio.gumroad.com/l/pwoeze

## License

MIT — see [LICENSE](LICENSE). Contributions are MIT, same as the aitmpl catalog.
