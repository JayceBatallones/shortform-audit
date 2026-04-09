# shortform-audit

A Claude Code skill that audits short-form video scripts (Reels, TikToks, Shorts) against a battle-tested knowledge base of engagement patterns.

Give it your script. Get back a scored audit with specific fixes, rewritten hooks, and CTA recommendations — all grounded in real engagement data from high-performing creators.

## What it does

When you share a script, hook, caption, or video idea, shortform-audit:

1. Evaluates it across 7 dimensions (viewer clarity, idea strength, hook quality, structure, authenticity, value delivery, CTA strategy)
2. Scores each dimension out of 10
3. Tells you what's working and what to fix, in priority order
4. Rewrites your hook if it's weak
5. Recommends the right CTA type for your goal
6. Gives a final verdict: **SHIP IT**, **NEEDS WORK**, or **REWRITE**

## Install

```bash
claude install-skill /path/to/shortform-audit
```

Or clone and install from GitHub:

```bash
git clone <repo-url>
claude install-skill ./shortform-audit
```

## Usage

Just share your script with Claude and ask for an audit:

- "Audit this script"
- "Review my hook"
- "Will this reel perform well?"
- "Critique this before I film"

The skill triggers automatically when you share short-form video content for feedback.

## The Knowledge Base

Everything in this skill is backed by real data. The `knowledge-base.md` file contains:

- **Hook patterns** with engagement numbers (e.g., singular promise hooks → 54K likes)
- **CTA strategies** with comment conversion data (e.g., keyword CTAs → 33K comments)
- **Structural frameworks** (3 content types funnel, 70/20/10 rule, 7-component breakdown)
- **Engagement correlations** (what actually drives likes/comments vs. what doesn't)
- **Creator case studies** from accounts with proven track records

The knowledge base is a living document — it gets better every time a new reel is analyzed.

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md). The main way to contribute is adding new patterns to `knowledge-base.md` backed by real engagement data from analyzed reels.

## License

MIT
