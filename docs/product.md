# Learnix: product tour

Learnix is an AI study workspace for Brazilian ENEM students. The interface and the generated material are in Brazilian Portuguese. This page walks through what a student does and why each piece exists.

## The unit of work: a study

A **study** is one workspace for one topic. Everything the student does lives inside it: tutor conversations, notes, a mind map, flashcards and practice sets. Nothing is a loose chat that disappears.

## The tutor

- Builds material gradually (overview, then one concept at a time, then worked examples) instead of one long dump.
- Renders math with KaTeX, and cites web sources when search is enabled.
- Reads and writes the study's notes and mind map itself, so the answer ends up saved where it belongs. A small card under each reply shows which notes it changed.
- Can run several conversations per study, and a conversation can be branched.
- Shows what it is doing while it works: a one-line summary of its reasoning, each tool call as it runs, then the answer streaming in. The student can stop a turn at any point.
- Offers a reasoning level, from standard up to extra-high on higher plans.

## Notes

Plain Markdown files organised in folders, with a live preview and math. Every note keeps its **version history** and can be **branched**, so a student can rework a summary without losing the original. Highlights from the tutor's answers can be saved straight into a note.

## Practice

| Mode | How it works |
| --- | --- |
| **Training** | Feedback and explanation after every question. |
| **Mock exam** | Timed. Corrected at the end. |
| **Standalone test** | A test on any topic, outside a study. Each attempt adapts to the student's earlier mistakes. |

Questions follow the ENEM format (five options, one correct) and are generated per topic. For every answer the student also states a confidence level, so the result separates **mastery** from **guessing**. Wrong answers become the focus of the next study round, and the tutor can be asked about any question directly from its explanation.

## Flashcards, streak and progress

- **Flashcards** are generated from notes and reviewed with spaced repetition (a Leitner-style schedule). Reviewing costs no AI usage, so free-plan students can keep studying.
- A **study day** counts when the student finishes a practice set or reviews ten flashcards. Consecutive study days form the **streak**.
- The **monthly progress** card shows practice completed, how much of it scored 60% or more, flashcards reviewed, and the streak.
- An optional **leaderboard** is available for students who want to compete.

## Try it without an account

The landing page offers a **guest demo**: a ready-made study with a tutor conversation, notes, a mind map and a practice set. It costs nothing to run, and *Save my progress* converts it into a real account in place, so nothing the visitor did is lost.

## Plans

A free plan and paid subscription plans (paid through Stripe). Plans differ in monthly AI budget, maximum reasoning level and question-set size. Students see their usage as a percentage of the month, never as tokens or dollars.
