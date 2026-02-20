Write an Architectural Decision Record for: $ARGUMENTS

## Instructions

1. Read `CLAUDE.md` for teaching approach and learner context.
2. Read `adrs/_template.md` for the output format.
3. Check existing ADRs in `adrs/` to determine the next sequence number.

## Process

Guide the learner through writing a concise, clear ADR. This is a critical staff-level skill — the ability to document decisions so future engineers understand *why* something was done.

### ADR Structure

1. **Title** — Short, descriptive (e.g., "Use PostgreSQL for user data")
2. **Status** — Proposed / Accepted / Deprecated / Superseded
3. **Context** — What situation are we in? What forces are at play? What constraints exist?
4. **Options Considered** — At least 2-3 realistic alternatives. For each:
   - Brief description
   - Key advantages
   - Key disadvantages
5. **Tradeoff Analysis** — Explicit comparison. What are we optimizing for? What are we sacrificing?
6. **Decision** — What we chose and *why*. One clear paragraph.
7. **Consequences** — What follows from this decision?
   - Positive consequences
   - Negative consequences (be honest)
   - Risks to monitor
8. **Metrics** — How will we know if this decision is working?
9. **Reconsideration Triggers** — What would cause us to revisit this decision?

### Teaching Notes
- ADRs should be executive-readable — clear, concise, no unnecessary jargon
- The *why* matters more than the *what*
- Good ADRs make future engineers grateful, not confused
- Practice thinking about decisions the learner encounters in their actual work

## Output

Determine the next ADR number by counting existing files in `adrs/` (excluding `_template.md`). Use format `NNNN-[decision-slug].md` (e.g., `0001-use-postgresql.md`).

Write the ADR to `adrs/NNNN-[decision-slug].md`.
