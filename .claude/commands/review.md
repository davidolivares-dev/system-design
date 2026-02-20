Perform a staff-engineer architecture review of: $ARGUMENTS

## Instructions

1. Read `CLAUDE.md` for teaching approach and learner context.
2. If the argument is a file path, read that design document. If it's a design name, look for it in `designs/`.
3. Read `reviews/_template.md` for the output format.

## Process

Act as a Staff engineer reviewing a proposed architecture. Be direct, critical, and constructive. The goal is to teach the learner to think like an architectural reviewer.

### Review Dimensions

1. **Requirements check** — Does the design actually solve the stated problem? Are there missing requirements?
2. **Scalability risks** — What breaks at 10x? At 100x? Where are the bottlenecks?
3. **Failure modes** — What single points of failure exist? What happens during partial outages? Are failure scenarios addressed?
4. **Consistency and correctness** — Are there race conditions, data loss risks, or consistency violations?
5. **Over-engineering** — What's more complex than it needs to be? What can be simplified?
6. **Under-engineering** — What critical concerns are hand-waved or missing entirely?
7. **Operational complexity** — How hard is this to deploy, monitor, debug, and maintain?
8. **Observability gaps** — What would you struggle to debug in production?
9. **Security considerations** — Any obvious security gaps?
10. **Evolution readiness** — How well does this design accommodate future changes?

### For Each Issue Found
- Explain **why** it's a problem (not just that it is one)
- Suggest a concrete alternative or improvement
- Rate severity: critical / important / minor / nitpick

### Summary
- Overall assessment (1-2 sentences)
- Top 3 things to fix before this could go to production
- Top 3 things done well (always acknowledge strengths)
- Decisions that should be revisited in 6-12 months

## Teaching Notes
- Explain the *reasoning* behind each critique so the learner develops review instincts
- Point out patterns that distinguish senior from staff-level thinking
- If the learner made a common mistake, name the anti-pattern

## Output
Write the review to `reviews/YYYY-MM-DD-review-[design-slug].md` using today's date. Use the template from `reviews/_template.md`.
