# System Design Learning System

An artifact-driven learning system for building real architectural thinking, powered by [Claude Code](https://docs.anthropic.com/en/docs/claude-code).

## Who This Is For

Engineers at any level who want to develop genuine system design skills for their career — not memorize interview patterns. Whether you're a junior engineer encountering distributed systems for the first time or a senior engineer sharpening your architectural judgment, this system adapts to your level.

## How It Works

Instead of reading passively, you learn by creating artifacts: design documents, tradeoff analyses, architecture reviews, and decision records. Each artifact lives in this repo, building a personal knowledge base over time.

Claude Code acts as a patient, rigorous mentor who:
- Starts from first principles and builds up
- Teaches at three levels: intuition, mechanics, and failure
- Makes tradeoffs explicit
- Never gives you happy-path-only answers
- Adapts to your current understanding

## Getting Started

1. Clone this repo
2. Install [Claude Code](https://docs.anthropic.com/en/docs/claude-code)
3. Run `claude` from the repo root
4. Type `/roadmap` to generate your personalized learning plan
5. Start learning with `/deep-dive [topic]`

## Commands

| Command | What It Does |
|---------|-------------|
| `/deep-dive [topic]` | Three-level topic study (intuition → mechanics → failure) |
| `/explain [concept]` | Quick, jargon-free explanation (conversational, no file) |
| `/design [system]` | Guided production system design |
| `/review [file]` | Staff-engineer critique of a design |
| `/tradeoff [A vs B]` | Architectural tradeoff analysis |
| `/adr [decision]` | Architectural Decision Record |
| `/reflect` | Assess learning progress, identify gaps |
| `/roadmap` | View and update your learning roadmap |

## Suggested Weekly Flow (2-3 hrs)

**Session 1: Learn**
- Pick a topic from your roadmap
- Run `/deep-dive [topic]` to study it in depth
- If you hit unfamiliar terms, use `/explain [concept]`

**Session 2: Apply**
- Run `/design [system]` to practice applying what you learned
- Run `/review` on your design to develop critical thinking
- Or run `/tradeoff [A vs B]` to sharpen decision-making

**Every few weeks:**
- Run `/reflect` to assess progress and find gaps
- Run `/roadmap` to update your plan

## Example Learning Session

Here's what a typical session looks like in practice. You open a terminal, run `claude`, and interact using slash commands:

```
> /roadmap
# Claude reads your roadmap, suggests "consistent hashing" as your next topic.

> /explain consistent hashing
# Not sure what that even is? Claude gives you a quick, jargon-free
# explanation with an analogy. No file created — just a fast answer.

> /deep-dive consistent hashing
# Ready to go deeper. Claude walks you through the concept at three levels:
# intuition (mental model), mechanics (how it works), and failure (what breaks).
# Writes a study note to notes/2026-02-20-consistent-hashing.md

> /design distributed cache
# Apply what you learned. Claude guides you through designing a system
# that uses consistent hashing, making tradeoffs explicit along the way.
# Writes a design doc to designs/2026-02-20-distributed-cache.md

> /review designs/2026-02-20-distributed-cache.md
# Claude reviews your design like a staff engineer — finds scalability risks,
# missing failure modes, and over-engineering. Constructive but direct.
# Writes a review to reviews/2026-02-20-review-distributed-cache.md

> /reflect
# After a few sessions, Claude reviews all your recent artifacts,
# assesses your understanding, identifies gaps, and suggests next steps.
# Writes a reflection to reflections/2026-02-20-reflection.md
```

Each command builds on the last, and every artifact stays in the repo as a reference you can revisit.

## Philosophy

- **Depth over breadth** — understand few things well rather than many things superficially
- **Career application, not interview prep** — design, evaluate, and communicate architecture
- **Failure-first thinking** — always ask "what breaks?"
- **Explicit tradeoffs** — there are no universally correct answers
- **Sustainable pace** — 2-3 hours per week, compounding over months
- **Beginner-friendly** — no assumed knowledge, everything explained from first principles

## Repo Structure

```
system-design/
├── CLAUDE.md          # Instructions for Claude Code
├── README.md          # This file
├── roadmap.md         # Your learning roadmap
├── designs/           # System design documents
├── adrs/              # Architectural Decision Records
├── notes/             # Study notes and tradeoff analyses
├── reviews/           # Architecture reviews
└── reflections/       # Periodic learning reflections
```

Each directory contains a `_template.md` that slash commands use as the starting structure for new artifacts.
