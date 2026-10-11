---
name: landing-page-review
description: Review, roast, audit or build a startup landing page the way Gui Bibeau (Solana Foundation, ex-Vercel) does in his Colosseum landing page review series. Use this whenever someone shares a landing page, marketing site, hero section, waitlist page, hackathon submission site, or asks "does my site convert", "is my hero copy clear", "roast my landing page", "review my homepage", "why is nobody signing up", or asks you to write or redesign a landing page, hero copy, CTA, or pricing section. Also use it when generating a landing page from scratch for a product, so the result passes the same review. Distilled from 32 recorded reviews (Oct 2026).
---

# Landing page review (Gui Bibeau method)

Gui Bibeau reviewed 32 Colosseum hackathon landing pages on video in October 2026, narrating raw first impressions while scrolling. This skill turns those reviews into a repeatable method. The core thesis behind every review: **since AI made good design cheap, design no longer differentiates. Clarity of message, a single honest call to action, and showing the product before asking for anything are what convert.** "Text is cheap, attention is the currency."

Two modes:
- **Review mode**: someone shares a URL, screenshot, or code for an existing page. Produce a review in the format below.
- **Build mode**: someone asks for a new landing page or hero. Build it against the same rules, then run the checklist on your own output before handing it over.

## Review mode

### Step 1: Look at it the way he does

If you have a browser, open the URL and actually scroll and click. If you only have a screenshot or source, say so and review what you can see. Walk the page in this order and take notes at each stop:

1. **Five-second read.** Read only the hero. Write down what you think the product is, for whom, and what the one action is, before reading anything else. If you cannot say it in one sentence, that is the number one finding. Count hero text levels (title, subtitle, sub-subtitle, badges): two is the limit.
2. **The CTA.** How many primary buttons are visible in the hero and nav? Click each. Does it go where it says? Does it ask for an email, wallet, or login before showing anything? "Try the app" next to "join the waitlist" is a contradiction.
3. **First scroll.** What does the first screen below the fold show: the product, or more words? Does anything look clickable but do nothing (cursor pointer, refresh, scroll-to-top)? Are any "live" indicators actually live?
4. **Slop scan.** Hunt the AI telltales listed in the checklist below. Count how much copy could be cut (he usually lands between 20% and 50%).
5. **Differentiation.** In one line, how is this different from the obvious incumbents in its niche? If the page never says, that is a finding, especially in crowded categories (prediction markets, tokenized stocks, trading agents, neobanks, marketplaces, privacy, AML).
6. **Audience fit.** Who is this for, and does the vocabulary match? Consumer pages should not say chain, mainnet, wallet or protocol names without a reason. Technical and institutional pages should be shorter, not longer, and hand over artifacts (docs, SDK, report, audit, a booking link). Institutions never self-serve pricing; they need "contact us".
7. **Trust.** Team with faces and bios, founder story, audits, public repo, SDK, docs, privacy policy, association with a known program, real social proof that fits the audience. Then the polish details that signal competence: rounded money, thousands separators, timestamps to the minute, search that tolerates a typo, no "coming soon".
8. **Mechanics.** Does the hero lag? Is `prefers-reduced-motion` respected? Any scroll hijacking, layout shift on toggles, dark mode ignoring the system, contrast too low, hero image too tall for a 14-inch laptop, broken images? Check mobile. If there is a language picker, does it fully work, and did the copy survive translation?
9. **Positioning red flags.** Half dashboard, half landing page. A kitchen sink of tools. Two products or two brands on one domain. A name that collides with a known company. A half-AI wizard. Marketplaces with no supply side.

### Step 2: Decide what matters

Order findings by what he orders them by: hero copy, then CTA, then clutter, then trust, then details. A beautiful page with unclear copy gets told to fix copy first; an ugly page with perfect copy gets a pass on looks. Be specific: name the exact pill, button, sentence, or section. Give credit for what works, with the same precision.

### Step 3: Write the review

Use this structure. Keep it tight; his videos are three to four minutes.

```
## <Site> — <score>/10

**Five-second read:** what I think this is, for whom, and what you want me to do. (Or: "I can't tell", with the reason.)

**What works**
- specific praise, one line each

**Fix first** (in order)
1. Hero copy: current → proposed rewrite (5–10 words, plus one optional line)
2. CTA: what to keep, what to demote to a link, what to remove
3. Cut: the sections, pills, and copy to delete, with a rough percentage
4. Show: what to put on screen before asking for anything (demo, markets, yields, screenshot, working widget)
5. Trust / differentiation gap, if any

**Nitpicks**
- small polish and mechanics items

**Recap:** one sentence with the three changes that move the score.
```

Scoring calibration from the series: 10 = clear in five seconds, single CTA, shows the product, every click works, micro-details communicate (lanatools.sh, joinlearnspace.com). 8 = clear and clean with duplicate CTAs or 20% excess copy (stature.finance, operatoruplift.com). 5–6 = good design, unclear what it is or how it differs (lid.pro, aetelier.xyz). Below 5 = information overload, dashboard-as-landing, login wall before anything is shown (stonkpile.xyz, gtmmaxing.com). These are calibration anchors, not answers: if the page in front of you is one of them, review it fresh and score what you see today; pages change.

Voice: direct, warm, a little blunt, never cruel. He says "unslop it", "my friend", "I'm not the target audience, but", and he admits what he does not understand instead of bluffing. He never judges the tech, only the page.

## Build mode

When writing a landing page or hero, draft against this shape, then review your own draft with the checklist before delivering.

- **Hero**: a title of five to ten words that says what it is, an optional one-line sub that says for whom or the differentiator, one primary button, one secondary link at most. A visual of the product on the right or below: a real screenshot, a 30-second demo without a logo intro, or a working widget. No badges, no pills, no em dashes. If the hero is full-page, keep it quiet and let one element move.
- **Proof**: the thing people came for, visible without login: live markets, yields, example portfolio, calculator, footage, what users made.
- **How it works**: three steps max, or a story told by two contrasting visuals (before/after). Do not also add a "features" grid that repeats it.
- **Trust**: team with faces, founder story in one line, audits or SOC 2 or public repo where relevant, docs and SDK links for technical audiences, social proof that fits the buyer.
- **Pricing** if applicable: two or three plain tiers; "contact us" for institutions instead of a number.
- **FAQ**: five or six at most, unless the audience is anxious (parents, compliance).
- **Footer**: docs, X, GitHub, privacy, brand assets in HTML.
- **Nav**: only what the page needs; docs as a link; one CTA on the right.
- **Vocabulary**: match the buyer. Consumer pages do not say chain, mainnet, wallet, or protocol unless that is the selling point; developer pages may.
- **Mechanics**: honour `prefers-reduced-motion`, keep contrast accessible, dark mode follows the system, no layout shift, CTA visible above the fold on a 14-inch laptop, test mobile, keep copy short enough to survive translation.
- **Agents**: put depth in docs plus a sitemap and `llms.txt` rather than on the page.

## The checklist (run on every page, yours or theirs)

Each line is something he called out in at least two reviews. Treat a "no" as a finding.

- Hero says what it is in ≤10 words and ≤2 text levels.
- I can tell who it is for from the hero.
- The differentiator is stated (or the niche is uncrowded).
- Exactly one primary CTA; docs and sign-in are links or secondary.
- No "try app" + "waitlist" pair; no duplicate CTA at every scroll.
- Every CTA goes where it says; nothing fake-clickable.
- Something real is visible before any email, wallet, or login.
- Demo video ≤30 s, no logo intro, ideally in the hero.
- No status pills ("live", "beta", "early access", "mainnet", "coming soon", "illustrative", and roadmap chips like "planned" or "next", which are "coming soon" by another name).
- No blinking dots, no em dashes, no cards-inside-cards, no repeated sections.
- Copy trimmed by 20–50%; depth moved to docs/FAQ; FAQ ≤6.
- Table stakes are not copy ("settles on chain", "on five chains").
- Chain words removed for consumer audiences; artifacts offered for technical audiences.
- Trust present: team, story, audit/repo/docs, fitting social proof.
- Numbers polished: rounding, separators, currency, timestamps to the minute.
- No lag, reduced-motion honoured, contrast OK, no scroll hijack, no layout shift.
- Dark mode follows system; language picker works fully or is gone.
- CTA visible without scrolling on a 14-inch laptop; mobile checked.
- One product, one brand, one domain; name does not collide with a known company.

## References

- `references/rulebook.md` — every rule with the near-verbatim quotes and the sites they came from. Read it when you need to justify a finding or weigh two fixes.
- `references/reviews-digest.md` — one paragraph per reviewed site, grouped by how well it scored. Read it for calibration before scoring, or to find a comparable example for the page in front of you.
- `references/sources.md` — the 32 post URLs and the reviewed sites, so you can point a user at the original video.
