---
layout: essay
type: essay
title: "A for Effort"
# All dates must be YYYY-MM-DD format!
date: 2026-05-12
published: true
labels:
  - Design Patterns
---

<img width="200px" class="rounded float-start pe-4" src="../img/effortestim.png">

## 1. How did you make your effort estimates?

My estimates were based mostly on gut feeling and how complex a task looked on the surface before I started it. I'd read through the issue description, think about how many moving parts were involved, and guess how long it would take to get it working. I didn't have much historical data to draw from at the start of the project since this was my first time building something of this scale with Next.js. So early estimates were largely informed by how unfamiliar the feature felt, not by any real baseline.

Looking at my issues, my estimates ranged from 7 minutes for styling a page to over 2 hours for making an authenticated page. The styling task felt straightforward and contained, while the admin profile work touched authentication and database logic, so I budgeted more time for it. The issue was that "looks complex" didn't always map accurately to "actually takes longer," especially once bugs entered the picture.

## 2. Did estimating in advance provide any benefit?

Yes, even when the estimates were off, the act of estimating forced me to think through what a task actually involved before jumping into it. It was a planning exercise as much as a prediction.

For example, when I estimated 20 minutes for Implement RSVP, I had to consider what that feature actually required: connecting a form, writing to the database, handling state. That mental walkthrough helped me start the task with a clearer direction, even though it ended up taking a little more time than expected. The estimate being close in that case was due to practice and past experiences.

I also learned to overestimate the total time to complete the task a little bit so I didn't need to feel rushed and could provide adequate time for me to work out any issues.

## 3. Was tracking actual effort useful?

Yes. Seeing the split between coding time and non-coding time was probably the most useful part. For Update Profile for Admin View, I estimated 45 minutes but spent 23 minutes coding and 29 minutes on non-coding work — 52 minutes total. That told me the task wasn't just a coding problem; a significant portion of the time went to things like reading documentation, debugging, testing, and figuring out how the pieces fit together.

That insight informed how I thought about later tasks. When I saw that non-coding time was consistently close to or exceeding coding time, I started mentally accounting for that overhead in how I planned my work sessions. It also helped explain why my estimates were off — I was only really estimating the coding portion, not everything that surrounds it.

## 4. How did you track your actual effort?

I tracked effort through the project's GitHub issue tracker, logging estimated time, actual coding time, and actual non-coding time per issue. I'd note the time when I started and keep a rough sense of how long I spent actively coding versus everything else and log it down when I am finished.

In terms of accuracy, it was probably close, but not precise. Non-coding time in particular is hard to track cleanly because it includes things like context switching, reading documentation or having AI assistance. I likely underreported it in some cases. The coding time was more reliable since it's easier to know when you're actively writing code versus when you've drifted into debugging or research.

## 5. What would you change next time?

I would break my tasks into smaller portions after fully thinking through what parts I would need to implement at once. I'd use earlier completed issues as a reference point for later ones and track time in shorter increments during longer tasks.

## 6. AI Use

I used Claude (Anthropic) and ChatGPT (OpenAI) during the project, primarily for implementation help rather than for estimating or tracking effort directly.

**Tool:** Claude (Anthropic) / ChatGPT (OpenAI, GPT-4)

**Representative prompts:**

- *"How do I implement an authenticated page only users with certain roles can have access to?"*
- *"What's wrong with this ESLint error: [pasted error]?"*
- *"Give me an example of how to implement RSVP logic that stores and removes a user's action in the database."*

**Time breakdown (approximate, per task session):**

- Prompt engineering: ~2–5 minutes per issue
- Generation and reading output: ~3–7 minutes
- Verification and manual editing: ~5–15 minutes (higher for anything touching auth or database logic)

**What was accepted vs. edited:**

Most AI-generated code needed at least some adjustment. Responses often assumed a slightly different project structure than what I had, so field names, schema references, or import paths needed to be corrected. For simpler tasks like fixing ESLint errors or getting a styling snippet, the output was usually usable with minor tweaks. For more complex features like the admin profile update or RSVP logic, the AI gave a solid starting point but the final implementation required meaningful editing to fit the actual codebase. I didn't paste and submit. I read through everything, cut what didn't apply, and made sure I understood what the remaining code was doing before using it.