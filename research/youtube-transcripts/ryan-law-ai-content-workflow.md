# Ryan Law — "How I Automated the Ahrefs Blog with Claude Code"
**Channel:** Ahrefs Podcast (YouTube)
**URL:** https://www.youtube.com/@AhrefsCom
**Host:** Tim Soulo (CMO, Ahrefs)
**Source:** ryan-law-transcript-raw.txt (programmatic transcript fetch)

---

## Video Overview

Ryan Law walks Tim Soulo through "the blog pipeline" — a Claude Code-based 
content automation system he built for the Ahrefs content team. The system 
uses ~23 skill files (each a markdown document encoding one step of a human 
writer's process) and chains them into a master pipeline that runs 12 steps 
autonomously, producing a publishable draft in 8-11 minutes.

This is a practitioner-level demonstration of agentic content production: 
not a thought piece about AI content, but a live walkthrough of a system 
already used to publish 10-15 articles and 30+ content updates at Ahrefs.

---

## The Blog Pipeline: Step-by-Step

**Step 1 — Research**

Claude uses the Ahrefs MCP to pull keyword metrics, parent topic, and 
long-tail variations. It fetches the top-ranking pages via web fetch, 
extracts headers, summarizes topics, and identifies content gaps — creating 
a comprehensive research report that feeds into every subsequent step.

Key insight Ryan flags: SERP analysis (understanding what's ranking and why) 
matters more than keyword volume alone. The research step replicates what a 
skilled human researcher does — just faster and more systematically.

**Step 2 — Ahrefs References**

Claude searches Ahrefs' own published content to find existing articles 
on the target topic. Output: a list of modules and sections already covered, 
used to ensure the new article is internally consistent, properly interlinked, 
and not duplicating existing work.

**Step 3 — Outlining**

Editorial standards encoded directly into the skill file:
- BLUF principle: every section opens with the most important idea
- MECE structure: sections are mutually exclusive, collectively exhaustive
- Logical support of the thesis through the header sequence
- Inverted pyramid: most important info first, context after

Output: a structured outline with hooks, key points, transitions, and 
flagged table or example opportunities.

**Step 4 — Product Annotation**

Claude reviews the outline against a master list of Ahrefs products and 
features, identifying contextual opportunities to mention specific tools. 
Adds signposts to the outline so the drafting stage knows where and how 
to incorporate product references naturally.

**Step 5 — Drafting**

Adapted from Ahrefs' internal style guide. Key rules:
- Problem-agitate-solution formula for introductions
- "Always explain what and why" for every claim
- Inverted pyramid structure throughout

Team members fork their own version of this step with their own writing 
voice examples — the system is explicitly not a one-size-fits-all process.

**Step 6 — Verify Claims**

Claude scans the draft for claims that need external validation, 
finds up-to-date sources for statistics, and flags anything that may 
be outdated. Ryan notes this step is also the core of the content 
updating pipeline — reviewing old articles for stale stats.

**Step 7 — Preview**

Generates an HTML file styled to look like the Ahrefs blog. Ryan can 
open it in a browser to review layout and readability before editing, 
without reading raw markdown.

**Step 8 — Format for Publish**

Adds WordPress shortcodes and other CMS-specific formatting so the 
article is ready to paste and publish.

---

## The Content Updating Pipeline

A parallel system built on the same skill file architecture, designed 
to periodically surface existing articles that need attention. Three 
functions:

1. **Outdated claims** — finds stats or facts that have aged out, 
   suggests updated replacements for human review
2. **New product features** — identifies articles that predate recent 
   Ahrefs features and recommends where to add them
3. **Topic gaps** — compares existing article against current SERP and 
   drafts new sections for topics competitors now cover that Ahrefs doesn't

---

## Key Design Principles

**More steps = more control, not more complexity**

Ryan's counterintuitive point: having 23 skill files instead of one 
big prompt means you can diagnose exactly where output degrades. Every 
step saves its output, so if an article comes out wrong, you can trace 
which step failed and refine just that file.

**Skill files are a process, not a prompt**

Each skill file encodes what a human writer would do at that stage — 
not instructions for generating text, but a process with inputs, outputs, 
and decision criteria. The goal is to make Claude follow a writer's 
workflow, not just produce words.

**Fork it, don't share it**

The team can fork their own version of the blog pipeline repo and 
modify it to their own writing voice, preferred examples, and content 
approach. Ryan's version uses his voice; using it for another writer's 
articles would produce the wrong result.

**Examples beat instructions**

Tim's observation (validated by Ryan): providing Claude with five 
example outlines or past posts produces more consistent output than 
writing out abstract style rules. The model infers patterns from 
examples better than it follows bullet-point instructions.

**Context trigger**

At pipeline launch, Ryan can optionally inject a few sentences of 
directional guidance — what angle to take, which product to mention, 
what existing article to incorporate. This small human touch shapes 
the entire 12-step run.

---

## Where This Works (and Where It Doesn't)

Ryan is direct about the system's scope:

**Best fit:** Evergreen informational topics that Ahrefs has already 
written about in some form. The pipeline anchors content generation in 
existing Ahrefs articles, so it's most effective when there's a rich 
library of prior content to draw from. Ryan calls these "boring topics" 
— well-covered subjects where comprehensive accuracy matters more than 
novel perspective.

**Not a fit:** Articles that require unique experience, strong opinions, 
or ideas no one has shared before. These still require human writers. 
The pipeline is housekeeping, not thought leadership.

---

## Tim's Parallel Use Case (from the conversation)

Tim describes using a similar approach to prepare for podcast interviews: 
Claude downloads YouTube transcripts from a guest's prior interviews, 
extracts the main and follow-up questions, and creates a TLDR for each. 
Then a master TLDR consolidates unique ideas across all interviews.

He also used Claude Code to write a book chapter by dictating raw ideas 
into Claude, pointing it at reference articles and podcast clips, and 
asking it to propose a chapter structure — then giving feedback before 
asking for the draft. His observation: "I'm very surprised how well it 
was able to distill my ramblings into coherent ideas."

---

## Most Quotable Moment

On whether the pipeline will replace manual writing:

Ryan: "We spend a lot of time writing stuff that AI is still not very 
good at helping with — things that require tons of thought and experience 
and unique perspectives and ideas that maybe other people haven't even 
shared before. [The pipeline] is almost like doing our housekeeping for 
us in some sense."

Tim: "AI would act like a journalist, an editor, a ghostwriter, and you 
would act as a source of ideas and opinions."

---

## Why This Matters for B2B SaaS

For a content team at a company like 100Hires:

- The pipeline architecture is directly replicable for any B2B SaaS 
  with an existing blog library — the more prior content, the better 
  the pipeline performs
- The product annotation step is the key differentiator: it ensures 
  every AI-assisted article naturally incorporates product use cases, 
  which is the primary goal of B2B content anyway
- The content updating pipeline is arguably more valuable than new 
  article creation — most B2B SaaS companies have dozens of aging 
  articles with stale stats that drag on overall content authority
- The "boring topics" framing is useful: routine informational content 
  is exactly where AI assistance provides the highest leverage, freeing 
  human writers for opinion pieces, case studies, and original research

---

## Collected via
Programmatic transcript fetch from Ahrefs Podcast YouTube episode.
Raw transcript stored at: research/youtube-transcripts/ryan-law-transcript-raw.txt
