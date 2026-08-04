# Claude Code Routines
**Video script — target runtime: ~4 minutes**

---

## [SCENE 1 — INTRO] (0:00–0:25)

You know the tasks. Checking for new bugs every morning. Reviewing pull requests. Making sure the docs didn't go stale after someone shipped a change.

You could do them yourself. But they're repetitive, they're boring, and you've got better things to do.

That's what Routines are for. Routines are an automation feature inside Claude Code — and today, we're breaking down what they are, and how they work.

---

## [SCENE 2 — WHAT IS A ROUTINE] (0:25–1:10)

A routine is a Claude Code automation you set up once — a prompt, access to your repo, and any connectors you want it to use — and then it runs on its own. On a schedule, from an API call, or in response to an event.

Here's the key part: routines run on Claude Code's own cloud infrastructure. Not your laptop. So there's no cron job to babysit, no server to maintain, and it doesn't matter if your machine is closed, you're asleep, or you're on a flight. The routine runs anyway.

You set it up once. Claude handles the rest.

---

## [SCENE 3 — THE TRIGGERS] (1:10–2:15)

Every routine needs a trigger — and you're not locked into just one. You can combine several on the same routine.

**Scheduled** — the simplest option. Run it hourly, daily, on weekdays, or weekly. You can even set a one-off run — just tell Claude something like "tomorrow at 9am, summarize yesterday's merged pull requests," and it fires once, then turns itself off.

**API-triggered** — each routine gets its own endpoint. Send a request with an auth token, and a new session kicks off. Perfect for wiring routines into deployment pipelines or other tools you already use.

**Event-triggered** — routines can react to things that happen in GitHub. A pull request gets opened. A release goes out. Claude picks it up and runs automatically.

Mix and match — the same routine can run on a schedule and respond to an event at the same time.

---

## [SCENE 4 — WHAT PEOPLE ARE USING THEM FOR] (2:15–3:15)

So what do people actually build with routines?

Bug triage — scanning for new issues every morning and flagging what matters.

Documentation drift checks — comparing recent code changes against your docs, and opening a pull request when something's out of date.

Pull request review — running your team's own checklist against every new PR before a human ever looks at it.

Release notes — collecting everything merged since the last release and drafting a changelog automatically.

Even porting changes across codebases — say, mirroring updates from a Python SDK into a parallel Go SDK, automatically, every time a PR merges.

The pattern is the same every time: define the job once, attach a trigger, and let Claude handle the repetitive part of engineering work.

---

## [SCENE 5 — GETTING STARTED] (3:15–3:45)

Getting started is simple. Head to claude.ai slash code, or just type slash-schedule in the Claude Code CLI, and describe what you want in plain language.

Routines are currently in research preview, available to Claude Code users on Pro, Max, Team, and Enterprise plans with Claude Code on the web turned on. And just like any interactive session, routines use your regular subscription usage.

---

## [SCENE 6 — OUTRO] (3:45–4:00)

That's Claude Code Routines — set it up once, attach a trigger, and let Claude take the repetitive work off your plate, whether you're at your desk or nowhere near it.
