# landing-page-review

A Claude Code skill that reviews or builds startup landing pages the way [Gui Bibeau](https://x.com/GuiBibeau) does in his Colosseum landing page review series.

In October 2026 Gui (Solana Foundation engineering, ex-Vercel, ex-MetaMask) recorded 32 three-to-four-minute video reviews of hackathon landing pages, narrating raw first impressions while scrolling and clicking. This skill distills those reviews into a repeatable method: a walk-through order, a fixed review format with a score out of ten, a build template, a checklist, and a rulebook with his own words as evidence.

The thesis behind every review: AI made good design cheap, so design no longer differentiates. Hero copy in five to ten words, one honest call to action, show the product before asking for an email or wallet, strip the AI telltales, and say how you are different.

## What is in the box

```
skills/landing-page-review/
├── SKILL.md                      the method: review mode, build mode, checklist
└── references/
    ├── rulebook.md               11 themes, each rule backed by near-verbatim quotes from the videos
    └── archetypes.md             the 32 reviews condensed into anonymised product archetypes, grouped by score
```

## Install

Claude Code loads skills from `~/.claude/skills/<name>/SKILL.md` (personal) or `.claude/skills/<name>/SKILL.md` inside a project.

```bash
git clone https://github.com/zeel991/landing-page-review-skill.git
cp -R landing-page-review-skill/skills/landing-page-review ~/.claude/skills/
```

Or, inside a project you want it scoped to:

```bash
cp -R landing-page-review-skill/skills/landing-page-review .claude/skills/
```

Start a new Claude Code session and the skill is available.

## Use

The skill triggers on its own when you share a landing page or ask for one. You can also call it directly:

```
/landing-page-review https://example.com
```

Example prompts:

- "Roast my landing page: https://myproduct.xyz"
- "Is my hero copy clear? Here is a screenshot."
- "Write a landing page for a stablecoin savings app aimed at people in the Philippines."
- "Why is nobody joining the waitlist on this page?"

## What a review looks like

```
## example.xyz — 6/10

**Five-second read:** ...

**What works**
- ...

**Fix first**
1. Hero copy: current → proposed rewrite
2. CTA: ...
3. Cut: ...
4. Show: ...
5. Trust / differentiation gap

**Nitpicks**
- ...

**Recap:** the three changes that move the score.
```

Findings are ordered the way he orders them: hero copy, then CTA, then clutter, then trust, then details.

## The checklist, in short

- Hero says what it is in at most 10 words and 2 text levels.
- Exactly one primary call to action; docs and sign-in are links.
- Something real is visible before any email, wallet, or login.
- No status pills, blinking dots, em dashes, cards inside cards, or repeated sections.
- Copy trimmed by 20 to 50 percent; depth lives in docs or FAQ.
- The differentiator is stated; table stakes are not copy.
- Vocabulary matches the buyer: no chain words for consumers, artifacts for technical buyers.
- Trust is present: team, story, audits or repo, fitting social proof.
- Mechanics: no lag, reduced motion honoured, contrast fine, dark mode follows the system, mobile checked.

The full list, with the reasoning behind each line, is in `SKILL.md` and `references/rulebook.md`.

## Attribution

The method and every rule come from Gui Bibeau's public review series on X ([@GuiBibeau](https://x.com/GuiBibeau), October 2026). Quotes are near-verbatim from the videos. The reviewed pages are deliberately not named anywhere in the skill: they change, and a verdict from one month should not anchor a review in another. He is not affiliated with this repo. If you build something with it, the advice he gives at the end of most reviews applies: simplify, show the product, earn the trust.

## License

MIT for the skill files in this repo.
