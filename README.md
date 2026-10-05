# Helpful Content Review (Claude skill)

A Claude skill that reviews and rates any piece of content, published or still a draft, against Google Search Central's guidance on [creating helpful, reliable, people-first content](https://developers.google.com/search/docs/fundamentals/creating-helpful-content).

You give it a URL, a pasted draft, or a doc. It reads the whole piece, checks a few claims and the search results for the topic, then returns:

- A score from 0 to 100 and a verdict
- A scorecard with evidence quoted from the content
- A Who, How, Why check
- The 11 search-first warning flags from Google's page
- A ranked fix list with exact quotes and suggested rewrites

## What it scores

| Dimension | Weight |
|---|---|
| Purpose: people-first, not search-first (Why) | 15 |
| Original value and effort | 20 |
| Completeness and reader satisfaction | 15 |
| First-hand experience and expertise | 15 |
| Trust: Who, How, accuracy, sourcing | 20 |
| Title and heading honesty | 5 |
| Craft and production quality | 5 |
| Page experience (published pages only) | 5 |

Each dimension is rated 0 to 4 and needs a quoted excerpt as evidence. Hard caps stop a good average from hiding a serious problem: fake authorship, a material factual error on a health, money or safety topic, and four or more search-first flags.

Verdicts: Publish (85 to 100), Publish after fixes (70 to 84), Revise (55 to 69), Major rewrite (40 to 54), Rethink (below 40).

## Install

**Claude Code:** copy the `helpful-content-review` folder into `~/.claude/skills/` (personal) or `.claude/skills/` inside a project.

```bash
git clone https://github.com/rednishat/helpful-content-review-skill.git
cp -r helpful-content-review-skill/helpful-content-review ~/.claude/skills/
```

**Claude.ai:** add the `helpful-content-review` folder as a custom skill. Anthropic's help center has the current steps.

## Use it

Ask in plain words, or call the skill by name:

```
/helpful-content-review https://example.com/your-post
```

```
Review this draft against Google's helpful content guidance and rate it.
```

It also triggers on questions like "is this thin content", "is this written for search engines", or "why did this page lose traffic".

## What it is not

The score is a review aid. It is not a Google score. Google says E-E-A-T is not a specific ranking factor and that quality rater data is not used directly in ranking. The score only shows how closely the content lines up with what Google says its systems try to reward.

The caps and weights are this skill's own design choices, built from Google's emphasis on trust. Change them if your content or risk level calls for it.

The skill judges helpfulness and trust. It does not check house style, title length, heading case or image specs.

## Source and attribution

The rubric is built from Google Search Central's page "Creating helpful, reliable, people-first content", which is licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). The page was last updated 2026-10-01 when this skill was written. This skill restructures its questions into a scoring rubric and adds the review workflow, caps and report format. It is not affiliated with or endorsed by Google. Google edits that page, so re-check it when you want a fresh read.

## License

The skill text in this repo is released under the MIT License. See `LICENSE`.

Maintained by [@rednishat](https://github.com/rednishat). Issues and suggestions are welcome.
