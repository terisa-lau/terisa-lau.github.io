---
layout: essay
type: essay
title: "Getting Code to Work VS Getting Code to Last"
# All dates must be YYYY-MM-DD format!
date: 2026-05-01
published: true
labels:
  - Design Patterns
---

<img width="200px" class="rounded float-start pe-4" src="../img/designPattern.png">
## Design pattern? Who is she?

When we first started building the class website, the main goal was just getting things to function. A button that submitted correctly or a page that loaded without crashing felt like a win. But as the project grew, the way the code was structured, how different pieces talked to each other, and how painful it was to update one feature without breaking another all started to matter a lot more than I expected.

Design patterns are well-established solutions to problems that come up repeatedly in software development. They are frameworks for organizing a project so it stays readable, maintainable, and scalable as it grows. In web development especially, this matters because users expect consistency, and developers need a reliable way to deliver that without rebuilding the same logic from scratch every time.

## Accidental Compliance 

A lot of the decisions we made during the project ended up aligning with real design patterns, even when we weren't explicitly naming them. The clearest example was how we separated concerns within the app. The code managing data — things like user posts or stored content — was kept separate from the code rendering the UI, with a middle layer handling user interactions like form submissions and button clicks. That's the Model-View-Controller (MVC) pattern. Breaking things into those three layers made it way easier to make changes without triggering a chain reaction across the whole codebase.

Reusability came up naturally too. Instead of rewriting navigation bars or page layouts every time, we built components once and used them everywhere. It kept the site consistent. If something needed to change, you changed it in one place and it updated everywhere. That's the core idea behind modular design.

Some of the more complex features really drove home why structured design matters. Letting users edit their own posts required the system to pull existing data, display it in an editable format, and save updates cleanly without disrupting anything else. Implementing admin controls added another layer as the system needed to clearly distinguish between what different user roles could and couldn't do. Without some kind of pattern guiding those interactions, things would've gotten messy fast.

By the end of the project, my mindset had shifted. I stopped thinking about code purely in terms of whether it worked and started thinking about whether it was built well. Design patterns gave the project structure that made it easier to grow, easier to debug, and easier to understand when coming back to it after time away. They turned out to be a genuinely useful way to think about building things that last.
