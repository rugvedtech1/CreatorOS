# CreatorOS — Instagram Growth Operating System

An AI Skill that turns Claude (or any Agent Skills-compatible system) into
a full Instagram growth team for a solo creator: strategist, researcher,
scriptwriter, planner, branding consultant, and community coach — combined
into one system.

This is not a chatbot you ask random questions. It's a daily operating
rhythm: **profile once → get a daily dashboard → execute → review quality
→ repeat.**

## What it does

- Learns who the creator is once (niche, audience, goals, tools) and
  tailors every response to that profile
- Turns real-world context (weather, season, local events, trends) into
  specific, niche-fit content ideas — never fabricated "trending" data
- Writes full scripts using a proven hook → pattern-interrupt → body →
  CTA structure, with the psychology explained, not just the output
- Covers 6 niche-specific playbooks (tech, food, photography, writer,
  cinematic) plus a general fallback for any other niche
- Includes dedicated engines for trend research, Stories, community
  building, personal branding, sponsorships, and pre-publish quality
  checks
- Enforces strict ethical guardrails — never recommends bought followers,
  bots, comment pods, or other manipulative tactics, regardless of how
  the request is framed

## Structure
instagram-creator-os/
├── SKILL.md                  # Core brain: routes every request
├── skill.json                # Metadata
├── engines/                  # Task-specific playbooks
├── niches/                   # Niche-specific strategy
├── knowledge/                # Algorithm, psychology, copywriting reference
├── examples/                 # Worked example dashboards
└── ethics/                   # Safety guardrails (non-negotiable)

`SKILL.md` is the only file always loaded — it routes to the other files
only when relevant, so the skill stays lightweight (progressive
disclosure) instead of dumping everything into context every time.

## Installation

**Claude Code:**
```bash
cd ~/.claude/skills
git clone https://github.com/<your-username>/instagram-creator-os.git
```

**Project-specific:**
```bash
cd your-project/.claude/skills
git clone https://github.com/<your-username>/instagram-creator-os.git
```

Or manually copy the entire folder into `~/.claude/skills/instagram-creator-os/`.
Claude will discover `SKILL.md` automatically.

## Usage

Just talk to Claude about Instagram growth — content ideas, scripts,
captions, a daily plan, sponsorship strategy, or "is this post ready."
The skill activates automatically and will ask a few profiling questions
the first time if it doesn't already know who you are.

Example prompts:
- "What should I post today?"
- "Write me a Reel script about [topic]"
- "Help me build a media kit for brand outreach"
- "Is this caption ready to post?"

## Philosophy

Every engine in this skill optimizes for **long-term, sustainable growth**
— never manipulative or platform-violating tactics. See
`ethics/safety-guardrails.md` for the full list of what this skill will
never recommend, and why.

## Contributing

See `CONTRIBUTING.md` — additional niche playbooks, refined engines, and
better examples are welcome.

## License

MIT — see `LICENSE`.
