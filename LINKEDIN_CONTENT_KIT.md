# LinkedIn Content Kit — 12 posts (v3, audited 29.04.2026)

> **Audit log (29.04.2026):** ICP audit revealed v2 kit was 9/12 posts targeted to wrong audience (engineers, AI-tool enthusiasts) instead of Track 2 ICP (non-tech founders with tech pain). Posts 1-3 already published as v2; kept for record. Posts 4-12 rewritten under v3 with ICP focus on non-tech buyers.
>
> **v3 Strategy:** Track 2 funnel = founders / business owners with technical pain. They want to see what was built, what changed, when to hire help, what AI actually does. They do NOT want code snippets, build-in-public personal-progress threads, or engineering career hot takes.
>
> **v3 Content mix:**
> - 3 case studies (anonymized client work showing what was built and what changed)
> - 4 decision-help posts (when to hire a Tech Lead, how to scope a tech project, etc.)
> - 2 industry insights (anti-hype takes on AI, dev team signals)
> - 2 personality / strategy (decision log, build-in-public retained but reframed)
> - 1 case study slot for user-drafted medoc post
>
> **Schedule:** 3 posts per week on Wed / Fri / Sun. Posts 4-12 to be queued for publication starting 30.04.

---

## 🗓 Already published (v2, kept for record)

### Post 1 · Wed 08.04 · [Build-in-public] Today I dropped Notion · ✅ PUBLISHED

> ⚠ ICP misalignment: tech-tooling audience, not Track 2 ICP. Kept as historical record.

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

### Post 2 · Fri 10.04 · [Opinion] Cyberpsychosis is not science fiction · ✅ PUBLISHED

> ⚠ ICP misalignment: AI-engineering audience. Kept as historical record.

(Full text unchanged from v2 — see git history.)

---

### Post 3 · Sun 12.04 · [TIL] setNativeValue for React forms · ✅ PUBLISHED

> ⚠ ICP misalignment: pure dev tutorial. Kept as historical record.

(Full text unchanged from v2 — see git history.)

---

## 🗓 v3 Queue (starting 30.04 publication)

### Post 4 · [Decision-help] When non-tech founders should hire a Tech Lead

```
Most founders ask me the wrong question. "Should I hire a CTO?"

Better question: what stage am I at, and what does it cost me to skip a tech lead now?

When you need someone like me on the team:

You have a working MVP, but every new feature breaks two old ones. The codebase makes changes more expensive every week.

You hired two devs, they shipped fine, then ran into a problem they could not solve themselves and started arguing. They need a senior architect to decide, not more devs.

You're about to sign a customer who requires SOC2, HIPAA, GDPR, or any compliance flag. Your devs don't know how to scope this.

When you don't:

You haven't sold anything yet. Build the MVP, sell it, then worry about scale.

Your tech is a basic CRUD app. No real-time, no compliance, no scale. WordPress and Webflow exist for a reason.

Your dev team is happy and shipping. Don't change what works.

A tech lead 1-2 days a week costs less than one wrong architecture decision. But not every business has a tech-lead-shaped problem.

If you don't know which side you're on, wait one month. The answer becomes obvious.
```

---

### Post 5 · [Case] How a content platform survived a hard legal deadline

```
Case: a Russian content platform with creators and brands. Two problems on my desk when I joined.

One. A new national law forced every digital ad on the platform into a state registry within hours of going live, or the platform pays a fine per ad. Existing manual flow took 3 hours of ops work per day. Hard legal deadline.

Two. The platform served multiple business teams inside one client organisation. Teams kept seeing each other's drafts, videos, and brands. No isolation. Internal complaints rising.

What I built.

For the registry. End-to-end pipeline from creator upload to legal registry. Idempotent and self-healing. Retries with backoff. Status reconciliation against the state registry every hour. Around 2M creatives a month flow through. Zero compliance incidents since go-live.

For the teams. Multi-tenant workspace layer. Admin-managed teams with strict data scopes. A team admin sees only their team's tasks, videos, brands, companies. Access enforced at the data boundary, not the UI. A clever URL or a misclick cannot leak data.

What changed for the client.

3 hours a day of manual ops became zero.
Internal cross-team data leaks went to zero.
The platform passed the legal deadline.

This is what a tech lead 2-3 days a week looks like in practice. Not "advisory". Owning the subsystem from the data model to the on-call rotation.
```

---

### Post 6 · [Translation] What AI actually does for your business in 2026

```
What AI actually does for your business in 2026, with no hype.

Three things AI does well right now.

Cleans up unstructured text. Customer emails into categories. Free-text complaints into ticket types. Meeting transcripts into action items. This was hard a year ago. Now it works with simple prompts.

Routes work between humans. Decide which expert handles which case. Triage support tickets by urgency. Pre-fill forms from messy input. The decision is small, the volume is high, the human stays as a check.

Searches your own data with natural language. "Show me customers from Q3 with refund requests over five hundred dollars". This used to need a BI team. Now an LLM with read access to the database does it in five seconds.

Three things AI is still bad at.

Anything where being wrong silently costs you money. Pricing. Forecasts. Compliance scoring. The model is confident even when wrong, and you don't see the wrong.

Long-running multi-step work without supervision. The error rate compounds. By step seven you have output you cannot trace.

Anything where the customer needs to feel heard. People know when they're talking to a script. AI sounds like a script.

So the question is not "should we use AI". It is: where does our business have a small high-volume decision that humans hate doing and where we can check the output afterwards.

That is the only good first project.
```

---

### Post 7 · [Industry insight] Three signs your dev team is stuck

```
Three signs your dev team is stuck, even if they say everything is fine.

One. You ask "how long will X take?". The answer is "a week or two". Two months later it's still in QA. The team learned this is the safe answer, because the real answer is "we don't know how to estimate this thing".

Two. Every release feels riskier than the last. Bug count up. Customer complaints after deploy. Bug fixes break something else. The team isn't lazy. The codebase is past the point where humans can hold the whole thing in their heads.

Three. The team can't explain a feature in plain language. They tell you about microservices, queues, retries. You wanted to know why your customer can't reset her password. The conversation is a symptom of architecture they don't actually own.

What this looks like from the team's side. They want to ship. They want to do it well. They are stuck on decisions nobody is making, and they don't want to be the one who pushes the architecture conversation upward.

A tech lead from the outside breaks the deadlock without firing anyone. The team gets to keep their work and their dignity. You get the architecture call made.

The most expensive thing in tech is not bad engineers. It is good engineers running out of architectural air.
```

---

### Post 8 · [Case] Praxisansatz — German clinic patient flow · 🔧 USER DRAFTING

> User is drafting this post manually based on direct work knowledge of medoc / Praxisansatz. Slot reserved.

(Insert text here when ready. Suggested angle: real-world product running in DACH clinics, what it solved for non-tech medical staff, what changed in their daily operations.)

---

### Post 9 · [Case] How a national measurement company freed 5,000 analyst-hours a week

```
Case: a national media measurement company. Their data is the basis of every TV, radio, and digital advertising decision in the country. 9,000 households on the panel. 500 analysts using internal tools every day.

The problem when I joined. The internal tooling was built piece by piece over a decade by separate teams. Reports took 30 seconds to load. Analysts ran the same query through three different screens. Recurring weekly reports were generated by hand. Around 10 hours a week per analyst lost to tool friction. With 500 analysts, that is 5,000 hours a week the company paid for and got nothing back.

What I rebuilt.

A shared frontend foundation. One state model, one auth, one design system. Every reporting screen on top of it.

Automated weekly report pipeline. Analysts stopped manually running and emailing reports. The system generated and delivered them on schedule.

A query layer that answered most analyst questions in under a second instead of 30.

Result. Around 10 hours a week per analyst back to actual analysis. Across 500 analysts, that is a small department's worth of work recovered. The CFO didn't see a new product on the balance sheet, but the same team was getting more done with the same headcount.

This is the kind of work tech leadership does that nobody outside the company ever sees. No marketing. No press release. Just a quiet shift from "we need to hire ten more analysts" to "we already have them, they just couldn't work".
```

---

### Post 10 · [Decision-help] How to scope a tech project when you're not technical

```
How to scope a tech project when you're not technical.

You don't need to learn engineering. You need three questions before any conversation with developers.

Question one. What's the smallest thing that would tell us if this works? Not "what's the perfect product". The smallest version. You're going to be wrong about details for the first three months. Make sure you're wrong cheap.

Question two. If we got 10x more users tomorrow, what breaks first? This separates "we have a feature" from "we have a product that survives". You don't need the answer yourself. You need the team to have an answer they're confident in.

Question three. Where in this system would a careless mistake cost us money? Login. Payments. Data export. Anywhere user input meets the database. This is where you need senior eyes, not where you save money.

If your team can't answer those three quickly, that's the gap a tech lead fills. Not building, deciding.

Most non-technical founders try to learn enough engineering to talk like an engineer. That doesn't work. You're better off learning to ask sharp questions and trust the answers, or trust nobody.
```

---

### Post 11 · [Case] Customer discovery with AI help — what works, what does not

```
Experiment: I ran customer discovery interviews with AI help, in parallel.

Setup. I do 20 interviews with potential users of an EdTech product. Standard customer discovery. The new part: an AI tool listens to the call recording, then drafts a structured analysis the same evening.

What worked.

The tool generated themes across 20 interviews 30x faster than I could.

It caught 4 patterns I missed in my own first three calls. I was anchored on my hypothesis. The tool was not.

Transcripts plus themes plus pull-quotes, ready next morning.

What did not work.

The tool cannot tell when a person is hesitating in the call itself. That is where the real signal is. So I run the live conversation, the tool runs the analysis after.

On emotional answers it tries to "solve" the user's problem. A real interviewer stays silent and waits. The model is bad at silence.

It missed two strong signals that were in voice tone, not in the words.

Lesson. Customer discovery is not "AI replaces the human". It is "AI does the analysis the human is too tired to do at 11pm". You do the empathy. The machine does the synthesis.

If you outsource the whole thing to AI, you get well-summarised wrong answers.
```

---

### Post 12 · [Opinion] Your roadmap is a waste. Decision log is everything

```
Unpopular opinion: roadmaps are useless.

A roadmap is fiction. It pretends the future is predictable. It builds false confidence in stakeholders. It's outdated two weeks after publishing.

What actually works: the decision log.

Every meaningful decision becomes one markdown file with date, context, options, choice, and reason. Nothing more.

In a month, the decision log shows:
where you are actually going, not where you promised to go
which hypotheses held and which did not
where past-you was wrong and how future-you can avoid the same mistake

In six months, the decision log is the only document you can reconstruct strategy from.

A roadmap is what you show investors. The decision log is why they write the second check.

I keep one for everything I run. Each major call gets one file. Every time a partner or an agent asks "why this way", I don't explain. I send the link.

When was your last roadmap update?
```

---

## 📊 Publication calendar (v3 queue)

| # | Date | Post | Category | ICP target |
|---|------|------|----------|------------|
| 4 | Wed 30.04 | When to hire a Tech Lead | Decision-help | Non-tech founders |
| 5 | Fri 02.05 | Content platform legal-deadline case | Case | Non-tech founders |
| 6 | Sun 04.05 | What AI actually does | Translation | Non-tech leaders |
| 7 | Wed 07.05 | Three signs your dev team is stuck | Industry insight | Non-tech founders |
| 8 | Fri 09.05 | Praxisansatz / medoc case | Case (USER DRAFT) | Healthcare / B2B |
| 9 | Sun 11.05 | Measurement company analyst-hours case | Case | Enterprise leaders |
| 10 | Wed 13.05 | Scoping tech projects | Decision-help | Non-tech founders |
| 11 | Fri 15.05 | Customer discovery with AI | Case | Founders, product |
| 12 | Sun 17.05 | Decision log > roadmap | Opinion | Founders, strategy |

---

## 🎯 Writing principles (carried from v2, integrated with `feedback_human_writing.md`)

1. **First 2 lines are the hook.** LinkedIn cuts the post around 200 characters with "see more". Before the cut it must be interesting.
2. **Specifics over abstraction.** Numbers, names, commands. Vague = AI smell.
3. **One idea per post.** 12 sharp thoughts beat 1 vague manifesto.
4. **No closing CTAs.** No "let me know your thoughts". A real short question is OK only when it's genuinely open.
5. **No emojis in body.** Only line-break bullets.
6. **Rotate categories.** Never two of the same in a row.
7. **All hard bans from `feedback_human_writing.md` apply.** Em-dash, arrows, AI vocab, native idioms. Especially: "delve / leverage / robust / journey / landscape / ecosystem". And: "pulled the trigger / pick up the torch / from scratch / bandwidth / deep dive / drop you a line / stay on your radar / leading the engagement". And the big one: no "X is not Y, it's Z" structure.
8. **Non-native simple voice.** A Russian engineer who learned English from docs and Stack Overflow would type this.

---

## ICP voice notes (v3-specific)

- **Don't write to engineers.** No code snippets, no MCP details, no React internals, no Claude Code SOPs. Save those for the product / engineering blog if needed.
- **Talk in business outcomes.** "3 hours of ops work became zero" beats "we built a self-healing pipeline with retries".
- **Anchor on real customer language.** "I asked how long it would take, the answer was 'a week or two'". Use the words your buyer actually says.
- **Show before / after.** Always pair the change with a number. Otherwise it's a vibe.
- **Avoid first-person grandeur.** "I made the switch in October 2025, best career call in ten years" reads aspirational when you're 6 months in. Stick to observable facts about the work.

---

## 🔧 Next actions

- [x] v3 audit and rewrite of Posts 4-12 (29.04.2026)
- [x] Add UGC Video Platform card to morozco.tech landing
- [ ] User to draft Post 8 (Praxisansatz / medoc case)
- [ ] Publish Post 4 on Wed 30.04
- [ ] After 3 v3 posts, hold retro: engagement vs v2, refine voice if needed
