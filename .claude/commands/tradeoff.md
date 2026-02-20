Analyze the architectural tradeoff: $ARGUMENTS

## Instructions

1. Read `CLAUDE.md` for teaching approach and learner context.
2. Read `notes/_template.md` for the output format.
3. Check `notes/` for any related prior analyses.

## Process

Conduct a rigorous tradeoff analysis between the two approaches. This is not a "pros and cons" list — it's a deep comparison that helps the learner develop architectural judgment.

### For Each Approach, Analyze:

1. **What it is** — clear, jargon-free explanation (with analogy if helpful)
2. **Performance characteristics** — latency, throughput, resource usage
3. **Scalability profile** — how does it behave as load grows?
4. **Failure modes** — what can go wrong? How does it degrade?
5. **Operational complexity** — how hard is it to run, monitor, debug?
6. **Cost implications** — infrastructure, development, and maintenance costs
7. **Organizational impact** — team size, skill requirements, cognitive load

### Then Answer:

- **When would a senior/staff engineer choose A?** (specific scenarios, not generalities)
- **When would they choose B?**
- **What signals indicate it's time to switch from one to the other?**
- **What's the migration cost** of switching later?
- **Common mistake**: What do people most often get wrong about this choice?

### Real-World Examples
- Name 2+ real companies/systems that chose each approach and why

## Output
Write the analysis to `notes/YYYY-MM-DD-tradeoff-[slug].md` using today's date and a kebab-case slug (e.g., `sql-vs-nosql`). Use the template from `notes/_template.md`, adapting the structure for a tradeoff analysis.

After writing, update `roadmap.md` if this tradeoff connects to topics the learner should explore next.
