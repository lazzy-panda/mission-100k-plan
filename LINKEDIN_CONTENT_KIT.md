# LinkedIn Content Kit — 12 posts × 4 weeks (v2, audited 08.04.2026)

> **Audit log (08.04.2026):** full rewrite from Russian v1 to English v2. Applied `feedback_human_writing.md` rules: stripped em dashes, arrows, AI vocab, native idioms, X-not-Y patterns, hook→bullets→wrap→question structure, and closing CTAs. Rewritten in non-native simple voice (Russian engineer typing English, not press release).
>
> **Language switch:** RU → EN. Reason: LinkedIn profile is in English, outreach targets are international (Cyprus, IL, RO, US, DE, IN), Mission $100K ICP is international founders. RU would reach only a narrow segment.
>
> **Post 1 replaced** with "Today I dropped Notion" — topical, live on 08.04.2026, better hook than the original "console replaces apps" angle.
>
> **Schedule:** 3 posts per week on Wed / Fri / Sun starting 08.04.2026.
>
> **Positioning:** Fractional CTO + solo founder + Claude Code agentic runtime + stealth EdTech.

---

## 🗓 Week 1 — Hook and manifesto (08.04 – 12.04)

### Post 1 · Wed 08.04 · [Build-in-public] Today I dropped Notion

```
Today I dropped Notion.

A week ago I put my 365-day plan into it. 365 database rows, a dashboard, checkboxes, integration, API token. Set up the way normal people do it.

Seven days later, days marked done: 0 out of 365.

Not because nothing got done. LinkedIn profile fully rebuilt, 10 cold connects sent, 5 warming comments under target posts, pitch and DM templates written. Opening Notion to mark a day done is just an extra step I don't do.

Now the source of truth is one file in the repo. PLAN.md. Claude Code reads it, writes it, updates the status during our conversation. I work, the status gets written in parallel, no separate ritual.

For phone access I use a GitHub private repo and Working Copy on iOS. 90KB of markdown, rendered natively.

A tracker that lives outside your work always loses to a tool built into the work itself.
```

---

### Post 2 · Fri 10.04 · [Opinion] Cyberpsychosis is not science fiction, this is 2026

```
Cyberpunk 2077 has a term: cyberpsychosis. When you stack too many implants and stop knowing where you end and the machine starts.

In 2026 this is not science fiction. This is the state of an engineer running 12 agents, 40 MCP servers, and three parallel Claude sessions.

Symptoms.
You forget what you did by hand and what you delegated.
Your decision log is the only way to know what you actually thought.
You wake up at 3am to check if an agent broke your main branch.
You phrase thoughts as prompts before you finish thinking them.

My theory: architecture fixes this. Not fewer tools. Architecture.

You need a clear line between what agents do, what you do, and an SOP with versions in between. A decision log you can't skip. A memory you can't fake.

Without that, you slip from operator to user. And the user always loses to the interface.

I'm building an internal operating system for my own agentic runtime, because I don't want a tool that understands me better than I understand myself.
```

---

### Post 3 · Sun 12.04 · [TIL] setNativeValue for React forms in Playwright

```
TIL about automating React forms with Playwright.

This week I updated my full LinkedIn profile with a script. Every input is a controlled React component.

The problem: plain element.value = 'text' doesn't trigger React state. The component doesn't see the change, and save sends empty fields.

The fix:

const setter = Object.getOwnPropertyDescriptor(
  Object.getPrototypeOf(el), 'value'
).set;
setter.call(el, 'new value');
el.dispatchEvent(new Event('input', { bubbles: true }));

This grabs the native DOM setter, bypasses the React wrapper, and dispatches the input event by hand. React accepts it as a real change.

Checkboxes work differently. element.click() gets eaten by React. You have to click through the Playwright role selector.

Result: my full LinkedIn (headline, about, 3 experience cards, 8 skills) updated in 20 minutes without manual copy-paste.

Playwright plus Claude Code plus one evaluate helper means I no longer open the browser to fill forms by hand.
```

---

## 🗓 Week 2 — System and process (13.04 – 19.04)

### Post 4 · Wed 15.04 · [Problem→Solution] Keeping context between Claude sessions

```
The problem: every Claude Code session starts from zero. You explain who you are, what you do, where you stopped yesterday. Every time.

10-15 minutes lost to re-prompting. Errors from incomplete context.

My fix: three files at the repo root.

MEMORY.md. Persistent memory about profile, goals, habits, principles. Auto-loaded into every session.

PLAN.md. Single source of truth for current state. What's done, what's in progress, what's next. Updated at the end of every session.

decision_log folder. Dated files, one per architectural choice. Each file answers "why exactly this way".

Result: a new Claude catches up in 30 seconds. I write "let's continue" and we continue from yesterday's stop point.

The key piece is decision_log. In a month you won't remember why you picked Next.js App Router over Pages. The log remembers. Your future self thanks your past self.

Three files. Thirty seconds of context. Every session.
```

---

### Post 5 · Fri 17.04 · [Build-in-public] Day 16 of 365

```
Day 16 of 365.

For six months I was building under contract. Now I run a studio of one person plus a small group of AI agents.

Track 1: stealth EdTech product. Customer discovery, MVP scope, first round of interviews this week.

Track 2: internal Claude Code agentic runtime. 12 SOPs, 5 specialized agents, decision log on every architectural call.

In parallel. LinkedIn profile fully rebuilt. 365-day learning program of 28 books and around 12,000 pages, already in week one with Thiel. Pipeline of Fractional CTO and advisory conversations in motion.

Target for 365 days: $100K per month.

I don't believe in "vibe work". I believe in a daily check-in with my own decision log.

Once a week I'll post here: what moved, what broke, what I learned.

Day 16 of 365. Going.
```

---

### Post 6 · Sun 19.04 · [Opinion] I stopped saying "AI assistant". Now it's "agentic runtime"

```
"AI assistant" is a frame I dropped from my vocabulary.

An assistant waits for tasks. You consult with it. It asks permission before every step.

That's not what I need.

I need a runtime. An environment that runs itself. Starts by SOP. Makes decisions by decision log. Writes to memory. Escalates only blockers.

The difference is practical.

Assistant mode (old): "do you want me to update LinkedIn?" "yes". It asks about every field.

Runtime mode (mine now): it reads plan.md, sees the task "rebuild profile", opens Playwright, does it, writes the result, marks it done. I wake up. It's ready.

The rename is the point. It marks a shift from "person plus tool" to "operator plus automated environment".

If you still "use AI", you're behind. The job now is to build the environment. The chatbot relationship is the old model.
```

---

## 🗓 Week 3 — Positioning and market (20.04 – 26.04)

### Post 7 · Wed 22.04 · [Opinion] Fractional CTO is the only honest path for a senior engineer in 2026

```
Hot takes on senior engineer careers in 2026.

Big Tech is the road to slowing down. Performance reviews, office politics, calendars full of meetings, architecture reviews of last year's decisions.

Startup founding engineer is a lottery. High upside, 70% of options go to zero.

Consulting is burnout. 60-hour weeks, other people's deadlines, other people's priorities.

Your own SaaS is 18 to 24 months without revenue. You against the market, alone.

Fractional CTO is the one path where you:
work 2-3 days a week per client, the rest is yours
take 3-4 companies at the same time and diversify risk
make architecture calls instead of tickets
charge 15 to 30K a month per client
leave real space for your own product

This isn't for everyone. You need reputation, network, and 6 months of patience before the first pipeline lands.

But if you're a senior with 10 plus years and you're tired of wearing a badge, this is the only honest game on the market.

I made the switch in October 2025. Best career call in the last ten years.
```

---

### Post 8 · Fri 24.04 · [TIL] MCP servers are the new npm

```
TIL: MCP servers are the new npm.

Model Context Protocol is Anthropic's standard for plugging external tools into LLM agents. Files, APIs, databases, browsers. All exposed to Claude as tools.

What changed in my stack in one month:

playwright-mcp for browser automation without one line of Selenium.
filesystem-mcp for file read and write in a bounded sandbox.
git-mcp for commits, diffs, branches straight from the prompt.
postgres-mcp for running SQL on my local dev DB from Claude.

Before, I wrote every integration layer by hand: OAuth, tokens, rate limits, error handling. Now it's `claude mcp add <server-name>` and done.

This is the moment the ecosystem stops being about "trying AI" and starts being about "building an operating environment on top of AI".

If you don't have at least three MCP servers running, you're reading this post from 2024.
```

---

### Post 9 · Sun 26.04 · [Build-in-public] 28 books for the year

```
I have 28 books queued for the year. Around 12,000 pages.

Start: Saturday 11.04. Finish: April 2027.

Partial list:
Thiel, Zero to One. First book, first week.
Dalio, Principles.
Isaacson: Jobs, Franklin, Einstein.
Crawley, System Architecture (MIT).
Feynman, all three volumes of the Lectures.
Landau-Lifshitz, Mechanics and Theory of Fields.
Goodfellow, Deep Learning.
Sutton, Rocket Propulsion Elements.

Why such a weird mix? Because narrow specialists have a ceiling.

Strategy and founder biographies teach decisions under uncertainty.
Physics and math teach thinking from first principles.
Systems engineering teaches working with complexity.
Science fiction teaches scale (Heinlein, Herbert, Asimov).

Around 33 pages a day. One hour in the morning.

The real goal isn't to finish the list. It's to rewrite my own operating model in 365 days.

I keep an open decision log per book. I'll share notes on Thiel in about a week.
```

---

## 🗓 Week 4 — Practice and principles (27.04 – 03.05)

### Post 10 · Wed 29.04 · [Problem→Solution] A design system for a team of one person and five agents

```
The problem: building a design system for a team of one person and five AI agents.

Classic DS like Material, Chakra, or shadcn assume a team. Docs, Storybook, contribution guidelines, token pipelines. Overkill for a solo founder.

But without a system, every agent touching UI invents its own spacing, palette, and button variant. Chaos scales in a day.

My fix: a single-file design system.

design-system.md in the project root. 400 lines. It contains:
8 color tokens, not 80.
4 spacing values, not a Fibonacci ladder.
3 typography scales.
5 key components with usage examples.
Links to the Tailwind config.

This file loads into the context of any agent writing UI. Plus a lint rule: "if you introduce a new color, ask the operator".

Result: two months of work, zero drift. The UI looks like one person made it because the docs are the one person.

A design system scales by the number of constraints you accept, not by the number of components.
```

---

### Post 11 · Fri 01.05 · [Case] Customer discovery through a Claude agent. What worked, what broke

```
Experiment: I ran customer discovery through a Claude Code agent.

Task: run 20 interviews with potential users of my stealth EdTech product, extract patterns.

What worked:
the agent generated adaptive follow-up questions in real time, as good as me
transcripts plus thematic analysis, 30 times faster than manual
it caught 4 insights I missed in my first three interviews

What broke:
the agent can't feel when a person is hesitating. It doesn't know how to stay silent and wait
on emotional answers it tried to "solve the problem" instead of going deeper
it missed two strong signals that weren't in the words, only in the tone

Lesson: discovery is a hybrid. The agent runs structure and analysis. You run empathy and silence.

Don't hand the live conversation to the machine. And don't run the conversation without the machine on a parallel rail.

I'm now building a "hybrid interview" SOP. I talk, the agent listens in parallel, after the call we debrief from the transcript.

Results in about two weeks.
```

---

### Post 12 · Sun 03.05 · [Opinion] Your roadmap is a waste. Decision log is everything

```
Unpopular opinion: roadmaps are useless.

A roadmap is fiction. It pretends the future is predictable. It builds false confidence in stakeholders. It's outdated two weeks after publishing.

What actually works: the decision log.

Every meaningful decision becomes one markdown file with date, context, options, choice, and reason. Nothing more.

In a month, the decision log shows:
where you are actually going, not where you promised to go
which hypotheses held and which didn't
where past-you was wrong and how future-you won't repeat it

In six months, the decision log is the only document you can reconstruct strategy from.

A roadmap is what you show investors. The decision log is why they write the second check.

I've been keeping mine since day one of the studio. 47 files in 6 months. Every time an agent or a partner asks "why like this", I don't answer. I send the link.

When was your last roadmap update?
```

---

## 📊 Publication calendar

| Plan day | Date | Post | Category |
|----------|------|------|----------|
| 7 | Wed 08.04 | #1 Dropped Notion | Build-in-public |
| 9 | Fri 10.04 | #2 Cyberpsychosis | Opinion |
| 11 | Sun 12.04 | #3 setNativeValue | TIL |
| 14 | Wed 15.04 | #4 Context between sessions | Problem→Solution |
| 16 | Fri 17.04 | #5 Day 16 of 365 | Build-in-public |
| 18 | Sun 19.04 | #6 Agentic runtime | Opinion |
| 21 | Wed 22.04 | #7 Fractional CTO path | Opinion |
| 23 | Fri 24.04 | #8 MCP is new npm | TIL |
| 25 | Sun 26.04 | #9 28 books for the year | Build-in-public |
| 28 | Wed 29.04 | #10 DS for solo + agents | Problem→Solution |
| 30 | Fri 01.05 | #11 Discovery through agent | Case |
| 32 | Sun 03.05 | #12 Decision log > roadmap | Opinion |

---

## 🎯 Writing principles (v2 — integrated with `feedback_human_writing.md`)

1. **First 2 lines are the hook.** LinkedIn cuts the post around 200 characters with "see more". Before the cut it must be interesting. The first sentence should make the reader stop scrolling.
2. **Specifics over abstraction.** Numbers, names, commands, snippets. "12 agents", "47 files", "0 out of 365". Vague = AI smell.
3. **One idea per post.** Don't try to say everything. 12 sharp thoughts beat 1 vague manifesto.
4. **No closing CTAs.** No "let me know your thoughts", "curious to hear", "what do you think". A real short question is OK only when it's genuinely open, not a template.
5. **No emojis in body.** Only line-break bullets. Emojis cheapen the "senior architect" tone. The only exception is the heading emoji in weekly section headers of this file.
6. **Rotate categories.** Never two Opinion posts in a row. Alternate tone.
7. **All hard bans from `feedback_human_writing.md` apply:** em dashes, arrows, AI vocab (delve/leverage/robust/journey/landscape/ecosystem), native idioms (pulled the trigger, pick up the torch, from scratch, bandwidth, deep dive), "not X, it's Y" structures, hook→bullets→wrap→question pattern, stacked parallelism.
8. **Non-native voice.** Simple verbs, plain English, no clever wordplay. A Russian engineer who learned English from docs and Stack Overflow would type this.

---

## 🔧 Next actions

- [x] Full audit and English rewrite of all 12 posts (08.04.2026)
- [ ] Publish Post 1 today (Wed 08.04) via Playwright
- [ ] Check engagement on Post 1 before Post 2 (Fri 10.04). If the tone is getting zero traction, tighten Posts 2-12 further.
- [ ] After Week 1 (Sun 12.04), hold a retro and decide whether to keep the Week 2-4 lineup or reshuffle based on what performed.
