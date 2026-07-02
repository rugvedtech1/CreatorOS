# Contributing to CreatorOS

Thanks for considering a contribution. This skill is built to grow —
more niches, sharper engines, and better examples all make it more useful.

## Ways to contribute

### Add a new niche playbook

If you cover a niche not yet in `niches/` (fitness, finance, fashion,
gaming, comedy, spiritual, automobile, etc.), follow the existing
structure in any file in that folder:

1. **What to monitor** — what real-world signals matter for this niche
2. **Content angles that work** — specific, not generic advice
3. **Format notes** — how Reels/Carousels/Stories differ for this niche
4. **Guardrail note** — any niche-specific ethical consideration

Then add a routing line for it in `SKILL.md` if it's commonly requested.

### Improve an existing engine

Engines in `engines/` should stay focused on one job. If you're adding
significant new content to an engine, consider whether it belongs there
or deserves its own file — keeping files focused is what keeps this skill
efficient (see the progressive disclosure note in `README.md`).

### Add worked examples

More examples in `examples/` help calibrate output quality and depth.
Follow the format in `examples/sample-daily-dashboards.md` — a real
profile, real (or clearly labeled hypothetical) context, and a full
dashboard output with reasoning included.

### Fix or strengthen guardrails

If you notice a growth tactic that should be flagged in
`ethics/safety-guardrails.md` but isn't, or a borderline case that needs
clearer guidance, contributions here are especially valuable — this file
protects the entire point of the skill.

## Style guidelines

- Write instructions directly to the AI reading the file ("use this file
  when...", not "this file helps users...")
- Prefer specific, concrete guidance over generic advice — this is the
  core quality bar for the whole project
- Always explain *why*, not just *what* — the skill should teach
  reasoning, not just output tactics
- Keep individual files focused — split rather than let one file grow
  unwieldy

## Submitting changes

1. Fork the repo
2. Create a branch for your change
3. Test your addition by actually using the skill with it loaded
4. Open a pull request describing what you added and why
