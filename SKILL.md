---
name: shortform-audit
description: Audit short-form video scripts (Reels, TikToks, Shorts) against proven engagement patterns. Use when the user shares a script, caption, hook, or video idea and wants feedback on how to make it more engaging, viral, or effective. Also use when the user says "audit my script", "review my hook", "critique this reel", or "will this perform well". Triggers on any request to evaluate or improve short-form video content before filming.
---

# Shortform Audit

Audit short-form video scripts against a battle-tested knowledge base of engagement patterns extracted from high-performing creators.

## How It Works

This skill uses a continuously updated knowledge base (`knowledge-base.md`) built from real creator analysis — extracted transcripts, engagement data, hook patterns, CTA strategies, and structural frameworks from creators who consistently go viral.

When the user shares a script or video idea, run it through the full audit.

## Usage

When the user provides a script, hook, caption, or video concept:

1. **Read the knowledge base** — Always read `knowledge-base.md` first. This is the source of truth and gets updated over time with new patterns.

2. **Run the audit** — Evaluate the script against every section of the knowledge base. Score each dimension:

   | Dimension | What to evaluate |
   |-----------|-----------------|
   | Ideal Viewer Clarity | Is it clear WHO this is for? One specific person, not a demographic. |
   | Idea Strength | Is the core idea screenshot-worthy? Has this concept been market-validated? |
   | Hook Quality | Does the first line create an open loop in 3-8 words? Bold promise or curiosity trigger? |
   | Script Structure | Does it follow HOOK + STORY [SETUP + JOURNEY] + CTA? Is there a clear story type? Are word counts within target for duration? |
   | Pacing & Funnel | Is it dense? Does it serve one funnel stage? Any dead air? |
   | Authenticity | Does it show real vulnerability or just polished expertise? |
   | Value Delivery | Is the value actionable right now? Does every point pass the "so what" test? |
   | CTA Strategy | Does the CTA match the goal? Is it naturally integrated? |

3. **Output the audit** — Use this format:

   ```
   ## Shortform Audit

   **Overall:** [SHIP IT / NEEDS WORK / REWRITE]
   **Estimated engagement tier:** [Low / Medium / High / Viral potential]

   ### Scores
   | Dimension | Score | Verdict |
   |-----------|-------|---------|
   | ... | /10 | one-line assessment |

   ### What's Working
   - (bullets — be specific, quote the script)

   ### What to Fix (Priority Order)
   1. **[Dimension]:** What's wrong → What to do instead
      - Rewritten example if applicable

   ### Rewritten Hook (if needed)
   > suggested alternative opening line

   ### CTA Recommendation
   - What CTA type fits this content + suggested phrasing
   ```

4. **Offer a rewrite** — If the script scores below 7 average, offer to rewrite the full script applying all fixes.

## Important Rules

- **Always read `knowledge-base.md` before every audit.** It changes over time. Don't rely on cached knowledge.
- **Quote the script back** when pointing out issues. "Your hook is weak" is useless. "Your opening 'Hey guys, today I want to talk about...' kills retention because..." is useful.
- **Be direct, not diplomatic.** This is a critique tool. Sugarcoating defeats the purpose.
- **Prioritize fixes by impact.** Hook > Idea > Structure > CTA > everything else. Don't bury the lead.
- **If the script is good, say so.** Don't manufacture problems. "SHIP IT" is a valid verdict.

## Updating the Knowledge Base

The knowledge base grows over time. When new reels are analyzed (via the `instagram-reel-extractor` skill or manually), new patterns should be added to `knowledge-base.md` under the appropriate section. Contributors can submit PRs to expand the knowledge base with new:

- Hook patterns (with engagement data)
- CTA strategies (with results)
- Structural frameworks
- Engagement correlations
- Creator case studies (added to the Appendix)

## File Structure

```
shortform-audit/
├── SKILL.md              ← this file (skill definition)
├── knowledge-base.md     ← the audit criteria (living document)
├── CONTRIBUTING.md       ← how to add new patterns
├── LICENSE
└── README.md             ← public-facing docs
```
