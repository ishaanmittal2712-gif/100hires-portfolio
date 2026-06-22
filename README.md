# 100Hires Portfolio Project
**Ishaan Mittal | Applying for: Junior Growth Marketing Specialist**

---

## Tools Installed

**Cursor IDE**
An AI-native code editor that lets you write, edit, and ship code using 
natural language. For a growth marketer, this removes the developer 
dependency when building landing pages, running experiments, or 
prototyping automations.

**Claude Code (via CLI)**
Anthropic's agentic coding assistant. Installed and authenticated 
successfully via terminal. Logged in under ishaanmittal2712@gmail.com 
(Claude Pro, Sonnet 4.6).

**Codex**
Searched Cursor's marketplace — Codex returned no results. Confirmed 
this is a known marketplace availability issue, not a user error.

---

## Steps Completed

1. Downloaded and installed Cursor IDE from cursor.com
2. Attempted to install Claude Code via Cursor's Extensions marketplace 
   — not available
3. Attempted to install Codex via Extensions marketplace — not available
4. Researched alternative installation methods using Cursor's built-in AI 
   and external documentation
5. Installed Node.js (LTS) from nodejs.org as a prerequisite for npm
6. Fixed Windows PowerShell execution policy blocking npm scripts
7. Ran `npm install -g @anthropic-ai/claude-code` successfully
8. Authenticated Claude Code via OAuth — resolved an initial 
   "Invalid OAuth Request" error by regenerating the auth link
9. Completed Claude Code setup: theme, terminal settings, account login
10. Created this public GitHub repository
11. Writing and committing this README

---

## Issues I Ran Into (and How I Solved Them)

**1. Claude Code and Codex not in Cursor marketplace**
Searched "claude" and "codex" in Cursor's Extensions panel. Claude 
returned an unrelated GSAP result. Codex returned nothing. Rather than 
stopping, I used Cursor's built-in AI to research alternative methods 
and found the CLI installation path via npm.

**2. npm not recognized — Node.js not installed**
Running `npm install` failed because Node.js wasn't on my system. 
Fixed by downloading the LTS version from nodejs.org and running 
the installer.

**3. Windows execution policy blocking npm**
After installing Node.js, npm still failed with a SecurityError. 
Resolved by running:
`Set-ExecutionPolicy -Scope CurrentUser -ExecutionPolicy RemoteSigned`
This is a standard Windows security setting that restricts script 
execution by default.

**4. Invalid OAuth Request on first Claude Code login**
The auto-opened browser URL threw an "Invalid code_challenge_method" 
error. Fixed by restarting the auth flow, copying the URL manually, 
and opening it in a fresh browser tab.

---

## Why This Process Makes Sense to Me

I'm a content strategist and SEO specialist with four years of 
experience across B2B SaaS, fintech, and edtech. I've never set up 
a CLI tool from scratch before tonight.

What this task showed me is that growth work at an AI-native company 
requires exactly this: the ability to get unstuck independently, 
use available tools to find answers, and execute without waiting 
for someone to hand-hold the process.

The tools themselves took a few hours to figure out. That's fine. 
What I'm more interested in is what we build with them.

---

*Completed within 48 hours of receiving the brief.*
*Claude Code v2.1.185 | Node.js LTS | Cursor IDE | GitHub*
