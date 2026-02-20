Design a production system for: $ARGUMENTS

## Instructions

1. Read `CLAUDE.md` for teaching approach and learner context.
2. Read `roadmap.md` to understand current learning stage.
3. Read `designs/_template.md` for the output format.
4. Check `notes/` for any prior deep dives on related topics — reference and build on them.

## Process

Guide the learner through designing this system collaboratively. This is a teaching exercise, not a hand-off — the learner should understand every decision.

### Step-by-Step Design Flow

1. **Clarify the problem** — What are we actually building? Who uses it? What does success look like?
2. **Functional requirements** — What must the system do?
3. **Non-functional requirements** — Latency, throughput, availability, consistency, durability targets
4. **Capacity estimation** — Back-of-envelope math for storage, bandwidth, QPS. Show your work and explain the reasoning.
5. **High-level architecture** — Core components and how they interact. Start simple, then layer complexity.
6. **Detailed component design** — Dig into the 2-3 most critical components. Data models, APIs, key algorithms.
7. **Tradeoff decisions** — Make at least 3 explicit tradeoffs with reasoning (e.g., consistency vs. availability, complexity vs. flexibility)
8. **Failure modeling** — What fails? How do we detect it? How do we recover? Consider: single node failure, network partition, data corruption, cascading failures.
9. **Scaling strategy** — How does this system grow from 1x to 10x to 100x? What changes at each stage?
10. **Observability** — Key metrics, alerts, dashboards, distributed tracing strategy
11. **Evolution** — What would you revisit in 6-12 months? What are the known shortcuts?

### Teaching Notes
- Define any new concepts as they come up (or suggest `/explain [concept]`)
- Connect design decisions to fundamentals the learner has already studied
- Be explicit about what a junior vs. senior vs. staff engineer would focus on
- Point out common mistakes and why they're tempting

## Output
Write the completed design to `designs/YYYY-MM-DD-[system-slug].md` using today's date. Use the template from `designs/_template.md`.

After writing, suggest running `/review` on the design to practice critical analysis.
