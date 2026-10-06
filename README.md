# Voice AI Job Hunter

This project is a small, practical experiment in Voice AI.

The idea came from my current job search. I am spending a lot of time every day looking through remote jobs, figuring out which ones are actually relevant to my background, and then applying and reaching out to people at those companies. I want to remove as much of the repetitive work as possible, while also using the project to learn how real-time voice agents work.

The first version is intentionally simple.

I want to be able to open the app, talk naturally, and say something like:

> "Find me today's best remote AI and full-stack jobs."

The system should find real jobs, understand my preferences, rank the jobs, explain why they are a good match, and read the shortlist back to me.

That is the first useful milestone. It is not meant to be a generic voice assistant or a demo built only for the sake of learning.

## What we are building

The first version has a simple flow:

```
Voice input
   ↓
LiveKit voice agent
   ↓
Job discovery
   ↓
Normalize jobs
   ↓
Remove duplicates
   ↓
Rank against my profile
   ↓
Return 5–10 strong matches
   ↓
Voice response
```

The important part is that the result should actually be useful for my real job hunt.

## Why this exists

There are two goals:

1. Make my own job search faster.
2. Get hands-on experience with real Voice AI engineering.

The second goal is important. I want to learn the parts that make voice agents interesting in production: realtime interaction, tool calling, latency, turn-taking, failure handling, and eventually the backend systems needed to run these workflows reliably.

But the project should always have a practical reason for existing. I do not want to spend weeks building infrastructure before there is something I personally use.

## What comes later

Once the shortlist is useful, the project can grow into the rest of the job-search workflow:

- reviewing and approving applications
- opening and filling application forms
- recruiter and hiring-manager enrichment
- drafting targeted outreach
- tracking applications
- measuring which outreach actually works

Those are later milestones.

For now, the focus is the smallest useful loop:

**Talk → find jobs → rank jobs → hear the shortlist.**

## Current scope

The current sprint is only about proving that loop with real data.

Do not jump straight into auto-apply, LinkedIn automation, telephony, or a large distributed architecture.

We can add those things after the core workflow is working and we have used it ourselves.

## How I will measure success

The best test is simple:

> Would I actually apply to the jobs this system recommends?

If the answer is no, the next step is to improve the product rather than add more features.
