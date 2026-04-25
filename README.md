<div align="center">

### `SUBSCRIPTION-SAFE · OPEN SOURCE · SKELETON`

# Subscription-Safe Starter

**The minimal skeleton for building an autonomous AI agent on a flat Claude Max subscription instead of burning pay-per-token API credits.**

[jaredcunningham.ai](https://jaredcunningham.ai) &nbsp;·&nbsp; [@cunninghamai\_](https://x.com/cunninghamai_)

</div>

---

## What this is

A bare-bones starter showing the folder structure + config stubs for building an autonomous AI agent that runs via `claude -p` subprocess + Telegram bridge + Obsidian-style markdown vault.

**Zero variable cost.** Your Claude Max subscription covers the LLM calls. Flat monthly. No API metering, no runaway bills.

## What's in the box

- ✅ Obsidian vault layout (`Areas/`, `Projects/`, `_System/`, `MEMORY/`, etc.)
- ✅ `.env.example` with safe defaults (Sonnet, conservative rate limits)
- ✅ pai-mobile system prompt template with vault path placeholders
- ✅ Setup script stub showing the shape

## What's NOT in the box

This repo is the skeleton. The full implementation lives in [the Kit](https://jaredcunningham.gumroad.com/l/subscription-safe-ai-kit):

- ❌ Working agent persona files (`SOUL.md`, `USER.md`, `STATE.md`, `MEMORY.md`)
- ❌ Complete pai-mobile system prompt, vault-routed
- ❌ Working installer script
- ❌ Cost-safety checklists
- ❌ OpenClaw migration playbook

## Product ladder

<table>
<tr>
<td width="340" valign="top">

#### The Guide — `$29`
<sub>PDF · 19 pages</sub>

Full narrative + architecture + cost-safety discipline. The story of the build.

[Buy the Guide →](https://jaredcunningham.gumroad.com/l/subscription-safe-ai-guide)

</td>
<td width="340" valign="top">

#### The Kit — `$49` &nbsp; <sub>recommended</sub>

<sub>PDF + templates</sub>

Everything above, plus persona templates, vault structure, setup script. Deploy in 90 minutes.

[Get the Kit →](https://jaredcunningham.gumroad.com/l/subscription-safe-ai-kit)

</td>
</tr>
</table>

<sub>Don't want to spend a Saturday on setup? **[Async DFY — $299](https://jaredcunningham.gumroad.com/l/dfy-install)** · _no Zoom, ever_</sub>

## Quick start

```bash
git clone https://github.com/JaredCunningham/subscription-safe-starter.git my-agent-vault
cd my-agent-vault

# Read vault-structure/ to understand the layout
# Move vault-structure/ contents to wherever your Obsidian vault lives
mv vault-structure ~/Documents/my-agent-vault

# For the full working system, get the Kit
open https://jaredcunningham.ai
```

## The stack this starter targets

Claude Code on a Max subscription · Telegram bridge · Obsidian vault · `launchd` scheduler. Zero variable-cost infra.

## Why this exists as a free repo

Architecture patterns should be public. The full implementation + persona files + setup script + written narrative is worth $49 to the people who want to skip the 40-hour learning curve.

<div align="center">

<br />

<sub>Built in the open. Signed off by a human who won't be named.</sub>

</div>
