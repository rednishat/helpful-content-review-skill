---
name: helpful-content-review
description: Review and rate any content, published or unpublished, against Google's "Creating helpful, reliable, people-first content" guidance. Produces a 0 to 100 score, a verdict, search-first warning flags, a Who/How/Why check, and a ranked fix list. Use this skill whenever the user shares a draft, URL, doc, newsletter issue, post, landing page or article and asks to review it, rate it, score it, audit it, check if it is helpful, check E-E-A-T, check if it is people-first, check if it is ready to publish, or find out why a page lost traffic. Also use it when the user asks "is this good enough", "will Google like this", "is this thin content", or "is this written for search engines". Run it before publishing and after any core update traffic drop, even if the user never says "helpful content".
---

# Helpful Content Review

Rates content against Google Search Central's page "Creating helpful, reliable, people-first content" (https://developers.google.com/search/docs/fundamentals/creating-helpful-content, licensed CC BY 4.0, page last updated 2026-10-01). Every dimension below comes from a section of that page. The page is the manual. Re-fetch it when the user asks for a fresh check, because Google edits it.

## What this skill is and is not

This is a review aid. The score is not a Google score. Google says E-E-A-T is not a specific ranking factor and that rater data is not used directly in ranking. The score only tells the user how well the content lines up with what Google says its systems try to reward. State this once, briefly, at the end of the report. Do not repeat it.

Writing rules for the report: plain short sentences, no invented data. Keep stock AI phrasing out of every rewrite or suggested line you produce (for example delve, leverage, robust, seamless, pivotal, "it's worth noting").

This skill judges helpfulness and trust. It does not check house style, title length, heading case or image specs. Pair it with your own style checklist for those.

## Step 0: Intake

Work out these before scoring. Take them from the message or the content. Ask one short question only if a missing answer would change the score a lot (for example YMYL status or the intended audience).

1. Source: pasted text, file, Google Doc or URL. For a URL, fetch it with a page-fetch tool. For a doc, read it fully. Read every word. Do not skim the middle.
2. Mode: **Unpublished** (draft) or **Published** (live URL). Published adds Page experience scoring. Unpublished marks it N/A.
3. Content type: tutorial, product review, comparison or listicle, opinion or analysis, newsletter issue, curated roundup, social post, landing page, docs.
4. Intended reader and what they came to do.
5. Focus keyword or topic, if any.
6. YMYL check: could the topic affect health, financial stability or safety, or society's welfare? If yes, accuracy standards rise (Step 3, dimension 5).
7. Author and how it was made: named human author? Any AI or automation involved? Any product tested?
8. If the user reports a traffic drop: note which pages and which queries fell. Google advises auditing the pages most hit and judging them against these questions. If a Search Console or SEO tool connector is available, pull page and query history for those URLs first.

If the content is partial (intro only), score what exists and list what could not be checked.

## Step 1: Gather outside evidence (unpublished and published)

Do these when web search is available. They make the score honest instead of guessed.

- **Compared with other results.** Search the focus keyword. Skim the top results. Google asks whether the content gives substantial value compared with other pages in search results. Note what the top pages cover that this one does not, and what this one has that none of them do.
- **Fact spot-check.** Pick the 3 to 5 most checkable claims (stats, dates, version numbers, prices, feature names, quotes). Verify each. Google asks about easily verified factual errors. One wrong claim you could have caught is a trust problem.
- **Author and site trust.** If a byline or site is given, check that an author page or About page exists and says something real.

Skip a check only if the tool is missing. Then list it under "Could not verify". Never score a thing you did not check as if you had.

## Step 2: The seven human-judgment tests

Run these on the whole piece before scoring. Answer each in one line. They feed the scores below.

1. **Bookmark test.** Would you bookmark it, share it with a friend, or recommend it?
2. **Printed-source test.** Would you expect to see it in or cited by a printed magazine, encyclopedia or book?
3. **Leave-satisfied test.** After reading, has the reader learned enough to reach their goal, and did the experience feel satisfying?
4. **Search-again test.** Does the reader feel they must go search again for better information elsewhere?
5. **Beyond-the-obvious test.** Is there any analysis or information a reader could not guess from the title?
6. **Direct-visitor test.** Would the existing or intended audience find this useful if they came straight to the site, with no search engine involved?
7. **Primary purpose test.** Does the site or newsletter have a clear focus this piece fits into?

## Step 3: Score the eight dimensions

Rate each dimension from 0 to 4. Points earned = rating / 4 x weight. Anchor every rating to a quoted excerpt or a named observation. No rating without evidence.

| # | Dimension | Weight |
|---|---|---|
| 1 | Purpose: people-first, not search-first (Why) | 15 |
| 2 | Original value and effort | 20 |
| 3 | Completeness and reader satisfaction | 15 |
| 4 | First-hand experience and expertise | 15 |
| 5 | Trust: Who, How, accuracy, sourcing | 20 |
| 6 | Title and heading honesty | 5 |
| 7 | Craft and production quality | 5 |
| 8 | Page experience (Published only) | 5 |

Rating scale: 0 absent or harmful, 1 weak, 2 partial, 3 solid, 4 strong.

### 1. Purpose (Why), 15 points

Google calls "Why" perhaps the most important question: the content should exist primarily to help people, and be useful to visitors who arrive directly.

- 4: Clear reader need. Exists because the audience needs it. No search-first flags.
- 2: Helps readers but shows signs it was picked for traffic (trend chasing, keyword stuffing of topics).
- 0: Made mainly to attract search visits, or produced with automation to manipulate rankings. Google treats that last case as a spam policy violation (scaled content abuse). Say so plainly if it applies.

Also count the search-first warning flags (Step 4). Many flags pull this score down.

### 2. Original value and effort, 20 points

Covers the questions on original information, reporting, research or analysis, insight beyond the obvious, and adding value instead of copying or rewriting other sources. Also covers the "main content" attributes Effort, Originality and Talent or skill.

- Effort: how much human work went in? Original analysis, manual translation, a custom tool or map are high. Pages generated from feeds, or AI text with no human oversight or curation, are little to none. Crediting other sources does not replace original effort.
- Originality: does the piece offer information or a view not already on other sites?
- Talent or skill: clear writing, well-made media, working tools. Not every topic needs specialist skill. A person sharing how they cleared their driveway of snow needs none.
- 4: Original data, testing, analysis, or a real point of view. Clearly more than the top results.
- 2: Accurate and clear but mostly a rearrangement of what already ranks.
- 0: Summary or rewrite of other sources with nothing added.

### 3. Completeness and reader satisfaction, 15 points

Covers "substantial, complete, or comprehensive description of the topic", the leave-satisfied test, the search-again test, and comparison with the other search results.

- 4: Reader can finish the task or decision from this page alone.
- 2: Covers the basics but leaves gaps the top results fill.
- 0: Reader must search again. Thin, padded, or answers a different question than the one promised.

Check for padding aimed at a word count. Google has no preferred word count. Do not recommend lengthening a piece to hit a number.

### 4. First-hand experience and expertise, 15 points

Covers "clearly demonstrates first-hand expertise and a depth of knowledge", such as having used the product or visited the place, and "written or reviewed by an expert or enthusiast who demonstrably knows the topic".

Look for evidence in the text itself: specific steps only a real user would know, screenshots that are the author's own, results with numbers, mistakes made, trade-offs felt. Generic statements any search could produce do not count.

- 4: Unmistakable lived or tested experience, with proof.
- 2: Knowledgeable tone but little proof of doing the thing.
- 0: Reads as written from secondary sources or by someone who never used the thing.

### 5. Trust: Who, How, accuracy, sourcing, 20 points

Google says trust is the most important E-E-A-T aspect. Experience, expertise and authoritativeness contribute to it, and content does not need to show all of them.

Score these parts together:

- **Who.** Is it self-evident who wrote it? Is there a byline where a reader would expect one? Does the byline lead to author background and the topics they write about? Is the authorship honest? Fake creator profiles, made-up names, AI headshots or false credentials are deception. Google says deception makes a page untrustworthy and signals low quality. Cap this dimension at 0 if found.
- **How.** Do readers learn how it was made? For reviews: how many products were tested, what the results were, how the tests ran, with photos as evidence. For AI or automation used substantially: is use disclosed, is the background given, is the reason for using it explained? Add disclosure only where a reader would reasonably wonder how it was made.
- **Sourcing.** Clear sources, evidence of expertise, links to an author page or About page. Do stats and claims have a checkable source?
- **Accuracy.** Any easily verified factual errors? On YMYL topics the content must be highly accurate and match established expert consensus. One material error on a YMYL piece is a rating of 0 or 1.
- **Site reputation.** If someone researched the site, would they find it well-trusted or recognized on this topic?

### 6. Title and heading honesty, 5 points

Does the main title give a descriptive, helpful summary? Does it avoid exaggeration and shock? Do headings summarize the section so readers can decide if they want it? Does the page deliver what the title promises, including no promise to answer something that has no answer, such as a release date that is not confirmed?

### 7. Craft and production quality, 5 points

Spelling and style issues. Does it look sloppy or rushed? Does it feel mass-produced, outsourced to many creators, or spread across a network of sites so no single page gets care? Is there a clean read from start to finish?

### 8. Page experience, 5 points (Published only)

Google tells owners not to focus on one or two aspects. Check overall: readable layout, intrusive ads or popups, mobile reading, load feel, the main content easy to find. For deeper checks send the user to Google's page experience documentation or Core Web Vitals. In Unpublished mode mark this dimension "N/A" and rescale: Final score = points earned / points available x 100.

Main content covers the primary text and media, interactive tools, user contributions that serve the page's purpose, tabbed or expanded sections, and titles and headings. Judge all of it, not only the body text.

## Step 4: Search-first warning flags

These are the questions where a "yes" is a warning sign. Answer each with Yes, No or Cannot tell, and quote evidence for every Yes.

1. Made primarily to attract visits from search engines?
2. Part of lots of content on many topics, hoping some performs?
3. Produced with extensive automation across many topics?
4. Mainly summarizing what others say without adding much value?
5. Written about because it is trending, not because the existing audience needs it?
6. Leaves readers needing to search again for better information?
7. Written to hit a word count because Google supposedly prefers one? (It does not.)
8. Entering a niche with no real expertise, only for search traffic?
9. Promises an answer to a question that has none (for example an unconfirmed release date)?
10. Date changed to look fresh when the content has not substantially changed?
11. Large adds or removals of content just to make the site look "fresh"? (It will not help.)

Flag count guide: 0 to 1 is fine. 2 to 3 is amber. 4 or more is red.

A note on SEO. SEO work such as titles, structure, internal links and clear headings is fine when applied to people-first content. Do not tell the user to remove SEO. Tell them to stop letting it lead.

## Step 5: Apply the caps

These caps are this skill's own design choices, built from Google's emphasis on trust. They stop a high average from hiding a serious problem. Apply the lowest cap that fits.

| Condition | Maximum final score |
|---|---|
| Deceptive authorship (fake author, fake credentials, fake photos) | 40 |
| YMYL topic with a material factual error | 50 |
| 4 or more search-first flags | 60 |
| Fails the search-again test and the bookmark test | 65 |

If a cap applied, show both the raw score and the capped score and name the rule.

## Step 6: Verdict

| Score | Verdict | Meaning |
|---|---|---|
| 85 to 100 | Publish | Strong on value and trust. Polish only. |
| 70 to 84 | Publish after fixes | Sound base, a few clear gaps. |
| 55 to 69 | Revise | Real weaknesses in value, proof or trust. |
| 40 to 54 | Major rewrite | The piece does not yet earn the reader's time. |
| Below 40 | Rethink | Wrong reason to exist, or trust damage. Do not publish as is. |

## Output format

Use this order. Keep it tight. Quote the exact line for every finding. Never write "improve the tone" or "add more depth" with nothing concrete behind it.

```
## Helpful Content Review

**Content:** [title or "Untitled"] | **Type:** [type] | **Mode:** Unpublished / Published
**Score:** NN / 100 (raw NN, cap applied: [rule] or none) | **Verdict:** [verdict]

[Two sentences. The main reason for this score and the single biggest fix.]

### Scorecard
| Dimension | Rating (0 to 4) | Points | Evidence |
|---|---|---|---|
| ... one row per dimension, evidence is a short quote or observation | | | |

### Who, How, Why
- **Who:** [byline, author info, honesty. One or two lines.]
- **How:** [process, testing, AI disclosure where expected.]
- **Why:** [the real reason this exists.]

### Search-first flags
[Only the flags answered Yes or Cannot tell, each with a quote. "Flags: N of 11".]

### Seven tests
[One line each. Bookmark, printed source, leave satisfied, search again, beyond obvious, direct visitor, primary purpose.]

### Fix list (ranked by score impact)
1. [Dimension] | "quoted excerpt" | What is wrong | Exact fix or rewrite
2. ...
(Max 8. Start with the fix worth the most points.)

### What works
[2 to 4 specific strengths with quotes. Real ones only.]

### Could not verify
[Anything not checked and why: no web search, no live URL, partial draft, claims not found.]
```

End with one line: this score is a review aid against Google's published guidance, not a Google ranking score. Then offer one next step: apply the top fixes, rewrite a named section, or run your own style checklist.

## Content type adjustments

Keep the same dimensions. Change what counts as evidence.

- **Tutorial or how-to:** Experience means the author's own screenshots, real settings, real errors hit and fixed. Generic steps copied from docs score 2 at best on dimension 4.
- **Product review or comparison:** Check the "How" fully: number tested, test method, results, photos. A list of features copied from vendor pages is a search-first signal.
- **Listicle or roundup of tools or links:** The risk is "mainly summarizing what others have to say". Value comes from the author's own picks, ranking logic, tests and commentary. Links plus one-line blurbs score low on dimension 2.
- **Curated newsletter issue:** Same as roundup. Reward the writer's own take on each item and the reason it was chosen. Judge the issue as a direct-visitor piece: would a subscriber miss it if it did not arrive?
- **Opinion or analysis:** Originality and reasoning carry the score. Unsupported claims hurt trust.
- **Social post:** Dimensions 6 (hook honesty) and 8 do not apply fully. Rescale. Judge value, first-hand proof, honesty of the claim and whether the reader leaves with something usable.
- **Landing page:** Judge whether the page answers real buyer questions with proof (specifics, screenshots, real numbers). Pure claims with no evidence hurt trust.
- **Docs or help article:** Completeness and accuracy dominate. Reader must be able to finish the task without outside help.
- **AI-assisted draft:** Check effort. Text generated with no human oversight or curation counts as little to no effort. Check that every fact was verified and that real examples and screenshots were added. Check disclosure where a reader would expect it.

## Rules for the reviewer

- Read the whole piece before scoring. Score after, not while reading.
- Be specific and blunt. The goal is a better piece, not a comfortable report. Do not soften findings.
- Never invent a stat, source, author fact or test result to improve a score or a rewrite. If the draft lacks proof, say what proof to gather, and let the author supply it. Use `[ADD: ...]` placeholders in suggested rewrites.
- Never advise fabricating a byline, credentials, reviews, test results or experience.
- Never advise a word count, date change or "freshness" edit as a ranking tactic. Only advise updating a date when the content was truly updated.
- Do not claim the content will or will not rank. Say how well it matches Google's stated guidance.
- If the user pushes back on a score, re-check the evidence. Change the score only if the evidence changes.
- Google suggests asking trusted people unaffiliated with the site for an honest read. Suggest this in the closing line when the verdict is Publish after fixes or higher and the stakes are high.
