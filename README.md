# 📸 CreatorOS — Instagram Growth Operating System

An AI Skill that teaches Claude and other AI assistants how to think like
a full Instagram growth team — strategist, researcher, scriptwriter,
planner, branding consultant, and community coach — so every piece of
content advice is psychologically sound, algorithm-aware, and tailored
to the creator, automatically.

`License: MIT` `Version: 1.0.0` `Claude Desktop` `Claude Code` `Any Agent Skills-compatible system`

---

## 🚀 The Problem This Solves

Every time you ask Claude to "give me content ideas" or "write me a Reel
script," you get something generic — technically fine, but not built for
*this* creator, *this* niche, or *today's* context.

Why? Because AI assistants don't automatically know:

- Why a hook that works for a tech creator falls flat for a poet
- Which Instagram surface (Feed, Reels, Explore, Stories) rewards which
  signal — and why that changes what "good content" even means
- How to turn today's weather or a trend into a specific, save-worthy
  idea instead of a generic prompt
- Why buying followers or using engagement pods destroys the exact trust
  a creator is trying to build
- How to price a sponsorship deal without underselling the audience

This skill fixes that permanently.

Install it once. Every Instagram strategy task Claude does from that
point applies the right engine, the right niche playbook, and the right
psychology — without you re-explaining it every session.

---

## ✨ How It Works

You say: **"What should I post today?"**

Claude:
1. Reads `SKILL.md` → checks if the creator's profile is known yet
2. If not, asks a few natural questions (niche, audience, goals, tools)
3. Detects niche → e.g. **photography** → loads `niches/photography.md`
4. Checks real-world context (weather/trends) via `engines/daily-intelligence.md`
   — using live search if available, or asking the creator directly
5. Builds Reel, Carousel, and Story ideas using the matched niche playbook
6. Applies `engines/script-writing.md` for hook/body/CTA structure
7. Applies `knowledge/copywriting-principles.md` for the caption
8. Runs the result against `ethics/safety-guardrails.md` before finalizing
9. Explains *why* each choice was made, not just what to post

**Example output — Content Decisions Table:**

| Element | Applied | Reason | Expected Impact |
|---|---|---|---|
| Hook | "Everyone puts their camera away when it rains. That's the mistake." | Pattern interrupt + contradiction hook for cold-discovery surfaces (Reels/Explore) | Higher scroll-stop rate in first 1-2 seconds |
| Format | Reel + Carousel combo | Reel for discovery reach, Carousel for save-worthy technique reference | Covers both reach and retention goals |
| Timing | Early evening | Rain clears by then; audience home and scrolling post-work | Matches actual availability, not generic "peak hours" |
| CTA | "Follow for more shots most people walk past" | Growth-goal CTA tied to specific recurring value, not generic "follow me" | Clearer reason to follow vs. generic ask |
| Hashtags | Mix of location + technique tags | Avoids burying post in oversaturated generic tags | Better Search-surface discoverability |

See `examples/sample-daily-dashboards.md` for full worked dashboards
across multiple niches.

---

## 📦 Installation

### Option 1: Git Clone (Recommended)

```bash
# For Claude Code — personal skills
cd ~/.claude/skills
git clone https://github.com/<your-username>/instagram-creator-os.git

# For a specific project
cd your-project/.claude/skills
git clone https://github.com/<your-username>/instagram-creator-os.git
```

### Option 2: Manual Copy

```bash
git clone https://github.com/<your-username>/instagram-creator-os.git
cp -r instagram-creator-os ~/.claude/skills/instagram-creator-os
```

### Per-Platform Setup

| Platform | File to Use | Destination |
|---|---|---|
| Claude Desktop / Claude Code | `SKILL.md` (whole folder) | `~/.claude/skills/instagram-creator-os/` |
| Cursor | `SKILL.md` → adapt | `.cursorrules` |
| Windsurf | `SKILL.md` → adapt | `.windsurfrules` |
| Other Agent Skills-compatible tools | `SKILL.md` + supporting folders | Per that tool's skills directory |

> No `npx` installer or CLI search tool exists yet — this is a pure
> Markdown-based skill, installed by copying files. A CLI could be a
> future addition; see Contributing.

---

## 🧠 Engines (Core Capabilities)

CreatorOS teaches Claude 8 core operating engines:

**1. 🎬 Script Writing** — Hook → Pattern Interrupt → Body → CTA →
Follow-up, matched to what the piece should optimize for (watch time,
shares, saves, or comments).

**2. 🔍 Trend Research** — Real, sourced trend-checking with a hard rule
against copycat content — every trend must carry the creator's original
angle.

**3. 🌦️ Daily Intelligence** — Combines real weather/season/local
events/trends with the creator's niche into specific content angles —
never fabricated "trending" data.

**4. 📱 Story Engine** — A rotation of 8 Story formats (poll, quiz,
BTS, AMA, countdown, etc.) mapped to Instagram's relationship-strength
ranking surface.

**5. 🤝 Community Building** — Reply strategy, discussion design, and
the specific mechanics that turn followers into superfans.

**6. 🏷️ Personal Branding** — The 5 pillars (trust, authority, voice,
visual identity, positioning) and how to find real differentiation.

**7. 💰 Sponsorship** — Media kits, pricing strategy, outreach, and
negotiation — built on audience quality, not follower count.

**8. ✅ Quality Checker** — A 12-point pre-publish audit (hook, watch
time, shareability, save potential, SEO, grammar, and more) before
anything goes live.

---

## 🏭 Niches Covered

| Niche | Primary Engines Used | Signal Focus |
|---|---|---|
| 💻 Tech / AI | Trend Research + Script Writing | Speed, hands-on credibility |
| 📸 Photography | Daily Intelligence + Quality Checker | Weather/light timing, technique depth |
| 🍜 Food | Daily Intelligence + Community Building | Season, local events, genuine reaction |
| ✍️ Writer / Poet | Personal Branding + Copywriting | Voice, emotional specificity |
| 🎬 Cinematic | Script Writing + Personal Branding | Pacing, visual consistency |
| 🌐 General (fallback) | All engines, adapted live | Universal principles applied on the fly |

Full playbooks live in `niches/`.

---

## 🏆 Worked Examples

See `examples/sample-daily-dashboards.md` for complete dashboards,
including:

- **Photography creator, rainy day** — reflection-shot angle, weather-
  timed posting, beginner-friendly gear-agnostic tip
- **Tech creator, AI model release day** — same-day breaking news reel
  with a genuine hands-on limitation included, not pure hype
- **Food creator, local festival week** — "hidden stalls locals actually
  go to" angle, deliberately avoiding the obvious festival coverage
  every other creator posts

Each example shows the full reasoning chain, not just the final output.

---

## 📁 Project Structure
instagram-creator-os/
├── SKILL.md                       ← Core brain: routes every request
├── skill.json                     ← Skill metadata
├── README.md                      ← This file
├── CONTRIBUTING.md
├── LICENSE
│
├── engines/                       ← 8 task-specific playbooks
│   ├── script-writing.md
│   ├── trend-research.md
│   ├── daily-intelligence.md
│   ├── story-engine.md
│   ├── community-building.md
│   ├── personal-branding.md
│   ├── sponsorship.md
│   └── quality-checker.md
│
├── niches/                        ← 6 niche-specific strategy files
│   ├── tech.md
│   ├── writer.md
│   ├── food.md
│   ├── photography.md
│   ├── cinematic.md
│   └── general.md
│
├── knowledge/                     ← Reference knowledge
│   ├── instagram-algorithm.md
│   ├── audience-psychology.md
│   └── copywriting-principles.md
│
├── examples/
│   └── sample-daily-dashboards.md
│
└── ethics/
└── safety-guardrails.md       ← Non-negotiable, overrides all else

`SKILL.md` is the only file always loaded. Everything else loads on
demand — progressive disclosure keeps the skill fast and lightweight
instead of dumping every niche and engine into context on every request.

---

## 🤝 Contributing

Contributions are welcome and encouraged.

**Ways to contribute:**
- Add a new niche playbook (fitness, finance, fashion, gaming, comedy...)
- Add a new worked dashboard example
- Strengthen or add a new engine
- Improve guardrails with real edge cases
- Build the CLI/npx installer (not yet built — open opportunity)
- Translate content for non-English-first creators

**How to contribute:**

```bash
# Fork the repository on GitHub
# Clone your fork
git clone https://github.com/YOUR_USERNAME/instagram-creator-os.git

# Create a branch
git checkout -b add-fitness-niche

# Make your changes, following the existing file format

# Push and open a Pull Request
git push origin add-fitness-niche
```

See `CONTRIBUTING.md` for detailed guidelines.

---

## 📄 License

MIT License — free to use, modify, and distribute. See `LICENSE`.

---

## ⭐ If This Helped You

If this skill improved how Claude helps you grow on Instagram, consider
starring the repo — it helps other creators find it.
