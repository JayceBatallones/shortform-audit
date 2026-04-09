# Contributing to Shortform Audit

The knowledge base gets better with every reel analyzed. Here's how to contribute.

## Adding New Patterns

All patterns live in `knowledge-base.md`. To add new ones:

1. **Analyze a reel** — Extract the transcript, engagement data, and metadata (the `instagram-reel-extractor` skill works well for this).

2. **Identify what's new** — Does this reel demonstrate a hook pattern, CTA strategy, structural framework, or engagement correlation that isn't already in the knowledge base?

3. **Add it to the right section** with engagement data:
   - New hook pattern → Section 3 table
   - New CTA strategy → Section 7 table
   - New structural insight → Section 4
   - New engagement correlation → Section 9 table
   - New creator/reel → Appendix

4. **Include the numbers.** Every pattern must have engagement data attached. "This hook works" is opinion. "This hook pulled 54K likes" is evidence.

5. **Update the metadata** at the top of `knowledge-base.md`:
   - Increment "Reels analyzed" count
   - Add new creator handles to "Sources"
   - Update "Last updated" date

## What Makes a Good Contribution

- **Data over opinion.** Every new rule should be backed by at least one real reel's engagement numbers.
- **Specific over vague.** "Use better hooks" is useless. "Negation chains ('It's NOT X, NOT Y, NOT Z') pulled 54K likes" is useful.
- **Counterexamples welcome.** If you find a reel that breaks a pattern and still went viral, add it. The knowledge base should capture nuance, not just rules.

## PR Format

```
## What I added
- (brief description of new patterns/data)

## Source reels
- (URLs of reels analyzed)

## Engagement data
- (key metrics that back the new patterns)
```

## Questions?

Open an issue if you're unsure whether a pattern is significant enough to add. When in doubt, include it — we can always prune later.
