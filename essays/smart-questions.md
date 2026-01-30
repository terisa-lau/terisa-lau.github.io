---
layout: essay
type: essay
title: "Smart Questions?"
# All dates must be YYYY-MM-DD format!
date: 2026-01-29
published: true
labels:
  - Questions
  - Answers
  - StackOverflow
---

<div style="display: flex; justify-content: flex-start; margin: 20px 0;"> <img width="200px" src="../img/Screenshot 2026-01-29 185027.png" class="rounded" style="margin-right: 20px;"> </div>

## Smart Questions

In software engineering&mdash;or any field, really&mdash;knowing how to ask smart questions is the difference from having to write multiple lines of code to achieve the same output versus writing a single, well-crafted line. In Eric S. Raymond's "How to Ask Questions the Smart Way", he illustrates how asking smart questions usually leads to clearer, more accurate, and faster responses by minimizing ambiguity and focusing attention on the actual problem.

## Having Context

Asking smart questions are important because software engineering problems are diverse due to the wide range of programming languages and tools involved. Even seemingly minor details can be crucial in identifying the root cause of an issue. Additionally, most problems have multiple possible solutions and require systematic troubleshotting. Without sufficient context about the problem, the environment it is in, and the troubleshooting steps already taken, diagnosing and resolving an issue can become inefficient and unnecessarily time consuing.

## Discipline

An important aspect of asking smart questions is to do your research such as searching the web or reading documentation before seeking help. Using what is available and already known shows respect for others' time. Solutions for common issues are addressed in documentation or solved through prior discussions. Referencing these sources helps prevent repeating previous troubleshooting attempts while allowing more productive support.

## Examples

I found a question on Stack Overflow about running the game, Doom, on an Arduino. The user wants to use a different display than what the original project was made for.The original project set up was built for a small 128×64 I2C OLED display. They have a bigger 1.54-inch SPI TFT display with an ST7789 controller, at 240×240 resolution. They ask if there's an "easy way" to make Doom work on their display and they linked the project's GitHub repo for more info.

The question is missing important details, which makes it hard to answer well. For example:

- What Arduino board are they using?
- Which library for the display?
- How is everything wired up?
- Have they tried any changes? What errors did they get?

The phrase "easy solution" is too vague which leaves a lot of specifics out. Because of these gaps, it results in those assisting to have to ask additional questions and make assumptions which consumes more time. 
The question resulting in a single comment asking, “What have you tried?” with a link to a page on "How to create a Minimal, Reproducible Example."

Reference to the [question asked](https://stackoverflow.com/questions/79878957/different-display-for-doom-on-arduino).


The second question examined is a Stack Overflow post titled “Why doesn't NRVO work if there is a previous return statement?”. The author presents two short, self-contained C++ code examples that differ only in structure and asks why Named Return Value Optimization (NRVO) occurs in one case but not the other. The question clearly identifies the observed behavior, explains why the behavior is unexpected, and asks whether the limitation is imposed by the C++ standard or by current compiler implementations. The author further narrows the scope to C++17 and later and explicitly considers and dismisses potential causes, such as the use of const.
This question follows the guidelines outlined in How To Ask Questions the Smart Way. It includes minimal reproducible examples, demonstrates prior understanding of the concept involved, and asks a specific “why” question rather than requesting a workaround. By clearly articulating what is known, what has been attempted, and what remains unclear, the author enables responders to give precise, standards-based explanations. As a result, the question allows for high-quality technical discussion rather than guesswork and repetitive solutions, making it an example of a smart and effective technical question.
 
Reference to the [question asked](https://stackoverflow.com/questions/79878890/why-doesnt-nrvo-work-if-there-is-a-previous-return-statement).

## Conclusion

Asking smart questions leads to better answers and more productive discussions. When a questions are clear and show genuine interest and effort, others are more willing to help.
