# 100Hires Portfolio Project
**Ishaan Mittal | Junior Growth Marketing Specialist**

---

## Round 1 — Tool Setup

Installed Cursor IDE, Claude Code (via CLI), and researched 
Codex. Full setup documentation below.

### Tools Installed

**Cursor IDE**
An AI-native code editor that lets you write, edit, and ship 
code using natural language. For a growth marketer, this removes 
the developer dependency when building landing pages, running 
experiments, or prototyping automations.

**Claude Code (via CLI)**
Anthropic's agentic coding assistant. Installed and authenticated 
successfully via terminal using npm. Logged in under 
ishaanmittal2712@gmail.com (Claude Pro, Sonnet 4.6, v2.1.185).

**Codex**
Searched Cursor's marketplace — returned no results. Confirmed 
this is a known marketplace availability issue, not user error. 
Manual installation documented in issues section below.

### Steps Completed

1. Downloaded and installed Cursor IDE from cursor.com
2. Searched for Claude Code in Cursor Extensions marketplace — 
   not available
3. Searched for Codex in Cursor Extensions marketplace — 
   not available
4. Researched alternative installation methods using Cursor's 
   built-in AI and Anthropic documentation
5. Installed Node.js (LTS) from nodejs.org as npm prerequisite
6. Fixed Windows PowerShell execution policy blocking npm scripts
7. Ran `npm install -g @anthropic-ai/claude-code` successfully
8. Resolved "Invalid OAuth Request" error on first login attempt 
   by regenerating auth link
9. Completed Claude Code setup: theme, terminal settings, 
   account authentication
10. Created this public GitHub repository
11. Committed README documenting the full process

### Issues I Ran Into

**1. Claude Code and Codex not in Cursor marketplace**
Searched both in Extensions panel. Claude returned an unrelated 
GSAP result. Codex returned nothing. Researched and found the 
CLI installation path via npm.

**2. Node.js not installed — npm not recognized**
Fixed by downloading LTS version from nodejs.org.

**3. Windows execution policy blocking npm**
Resolved with:
`Set-ExecutionPolicy -Scope CurrentUser -ExecutionPolicy RemoteSigned`

**4. Invalid OAuth Request on first Claude Code login**
Auto-opened browser URL threw an error. Fixed by restarting 
auth flow and opening the URL manually in a fresh browser tab.

### Why This Process Makes Sense to Me

I'm a content strategist with four years of experience across 
B2B SaaS, fintech, and edtech. I've never set up a CLI tool 
from scratch before this task. What it showed me is that growth 
work at an AI-native company requires exactly this — the ability 
to get unstuck independently, use available tools to find 
answers, and execute without waiting for someone to guide 
the process. The tools took a few hours to figure out. 
What I'm more interested in is what we build with them.

---

## Round 2 — AI-Powered SEO Content Production Research

**Topic chosen:** AI-Powered SEO Content Production

### Why This Topic

AI-powered SEO content production sits at the intersection of 
my core skills — four years of SEO content writing across B2B 
SaaS, fintech, and edtech — and where the industry is clearly 
heading. Tools like Scalenut (a client I've written for) are 
building entire workflows around AI-assisted content production. 
Understanding who is shaping this space is directly relevant 
to growth work at 100Hires.

### Why These 10 Experts

These are not the first Google results. They are practitioners 
— people running agencies, leading content at real companies, 
and building frameworks that other SEOs actually use. Each was 
selected for having a specific, original contribution to AI SEO 
content production, not just commenting on it.

| # | Expert | Role | Core Contribution |
|---|--------|------|-------------------|
| 1 | Ryan Law | Director of Content, Ahrefs | AI content systems backed by 1B+ data points |
| 2 | Lily Ray | VP SEO, Amsive | Documents what GEO tactics are already getting penalized |
| 3 | Mike King | Founder, iPullRank | Technical AI SEO, Google patent analysis, GEO architecture |
| 4 | Ross Simmonds | CEO, Foundation | Pioneered GEO, "Create Once Distribute Forever", RoGEO measurement |
| 5 | Aleyda Solis | Founder, Orainti | Built LearningAISearch.com, international GEO specialist |
| 6 | Koray Tugberk Gubur | Founder, Holistic SEO | Created Topical Authority methodology, semantic SEO |
| 7 | Jori Ford | Co-founder, Octopus Labs | Created Hybrid Engine Optimization, AI crawler experiments |
| 8 | Amanda Natividad | Chief Evangelist, SparkToro | Zero Click Marketing, Algorithmic Capital framework |
| 9 | Nathan Gotch | Founder, Gotch SEO | 97-point GEO checklist, practical AI SEO implementation |
| 10 | Kevin Indig | Independent Advisor | Commodity vs defensible content framework, B2B growth |

### Repository Structure
/research/sources.md           — Full expert list with links and annotations

/research/linkedin-posts/      — Posts and insights from each expert

/research/youtube-transcripts/ — 3 video transcripts with chapter breakdowns

/research/other/               — Additional reference materials
### What I Learned

The most important insight from this research: the practitioners 
who are winning in AI SEO are not the ones chasing the newest 
GEO tactic. They are the ones who built strong content 
fundamentals first, then layered AI tools on top to move 
faster and distribute wider.

For a B2B SaaS ATS like 100Hires, the implication is clear — 
genuine third-party credibility (G2, Capterra, community 
mentions, YouTube presence) is more durable than any 
AI-generated content strategy. The brands that get cited 
by AI are the ones that were already trusted by humans.

---

*Completed within deadline.*
*Tools: Claude Code v2.1.185 | Node.js LTS | Cursor IDE | GitHub*
*Commits: Regular throughout the process, not one final dump.*
