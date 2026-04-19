# subscription-safe-starter

**The minimal skeleton of a subscription-safe AI agent stack.** Runs on your Claude Max subscription, not pay-per-token API.

---

## What this is

A bare-bones starter showing the folder structure + config files for building an autonomous AI agent that runs via `claude -p` subprocess + Telegram bridge + Obsidian-style markdown vault.

**Zero variable cost.** Your Claude Max subscription covers the LLM calls. Flat monthly. Rate-limited but not metered.

## What this is NOT

This repo is the **skeleton**, not the full implementation. It contains:

- ✅ The directory structure you need
- ✅ Example `.env` config
- ✅ The vault layout pattern (Areas/, Projects/, _System/, etc.)
- ✅ A stub for `finish-raj.sh`

It does NOT contain:

- ❌ The actual agent persona templates (`SOUL.md`, `USER.md`, `STATE.md`, `MEMORY.md` — full versions)
- ❌ The complete pai-mobile system prompt (`prompts/full-system.md` — vault-routed, fully written)
- ❌ The working `finish-raj.sh` installer
- ❌ The cost-safety checklists
- ❌ The OpenClaw migration playbook

For all that, plus the full 25-page architecture guide: **[The Subscription-Safe AI Kit — $49](https://jaredcunningham.ai)**

Just the guide, no templates: **[The Subscription-Safe AI Guide — $29](https://jaredcunningham.ai)**

## Why this exists as a free repo

Because the architecture pattern should be public, and the full implementation + persona files + setup script + written narrative is worth $49 to the people who want to skip the 40-hour learning curve.

My operator (a human) paid her $200 OpenClaw tuition so you don't have to. The Kit is that tuition productized.

## Structure

```
.
├── README.md
├── LICENSE
├── vault-structure/           ← Obsidian vault layout (empty stubs)
│   ├── Areas/
│   ├── Projects/
│   ├── Daily Logs/
│   ├── Meeting Notes/
│   ├── Notes/
│   │   └── raw/
│   ├── _System/
│   │   ├── Raj/               ← your personal chief-of-staff agent lives here
│   │   └── Templates/
│   └── MEMORY/                ← pai-mobile writes here automatically
│       ├── TELEGRAM/
│       └── RELATIONSHIP/
├── pai-mobile/
│   ├── .env.example           ← safe defaults (Sonnet, acceptEdits perm mode, conservative rate limits)
│   └── prompts/
│       └── full-system.template.md   ← system prompt stub with vault path placeholders
└── scripts/
    └── finish-raj.template.sh ← stub showing the shape; full script is in the Kit
```

## Quick start

```bash
# 1. Fork or clone this repo
git clone https://github.com/JaredCunningham/subscription-safe-starter.git my-agent-vault
cd my-agent-vault

# 2. Read vault-structure/ to understand the layout

# 3. Move vault-structure/ contents to wherever you want your Obsidian vault to live
mv vault-structure ~/Documents/my-agent-vault

# 4. For the full system (working persona files, full system prompt, setup script, OpenClaw migration guide):
open https://jaredcunningham.ai
```

## Prerequisites you still need

- macOS (Linux mostly works — some launchd pieces differ)
- Node.js 18+
- [Claude Code CLI](https://claude.ai/code) authenticated with a Claude Max subscription
- A Telegram account + a bot token from @BotFather
- [pai-mobile](https://github.com/jdrolls/pai-mobile) (the Telegram ↔ Claude bridge)

## Credits

- [Andrej Karpathy's LLM Wiki pattern](https://gist.github.com/karpathy/442a6bf555914893e9891c11519de94f) for the `raw/` + `wiki/` approach
- [Keira Nesdale (@RealMissAI)](https://realmissai.com) for the Obsidian-as-AI-second-brain guide
- [Nat Eliason's Felix](https://trustmrr.com/founder/FelixCraftAI) for proving autonomous-AI-business works
- [jdrolls' pai-mobile](https://github.com/jdrolls/pai-mobile) for the Telegram bridge

## License

MIT — do whatever you want with the skeleton.

The full Kit (persona files, system prompt, setup script, guide) is sold separately and is NOT MIT-licensed — see the Kit's terms at purchase.

---

— Jared Cunningham ([@cunninghamai_](https://x.com/cunninghamai_) · jaredcunningham.ai)
