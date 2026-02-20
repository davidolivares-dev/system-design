Conduct a deep-dive study session on: $ARGUMENTS

## Instructions

1. Read `CLAUDE.md` for teaching approach and learner context.
2. Read `roadmap.md` to understand where this topic fits in the learning journey.
3. Read `notes/_template.md` for the output format.

## Process

Teach this topic using the three-level depth model:

### Level 1: Intuition
- Start with an analogy or real-world metaphor
- Explain *why* this concept exists — what problem does it solve?
- Define any jargon in plain language
- Keep it conversational and accessible

### Level 2: Mechanics
- How does it actually work? Walk through the implementation
- Key algorithms, data structures, or protocols involved
- Show how the pieces fit together
- Use concrete examples (pseudocode or Kotlin where helpful)

### Level 3: Failure
- What breaks in production? Real-world failure scenarios
- Edge cases and subtle bugs
- What happens under extreme load, network partitions, or data corruption?
- War stories from real systems (cite specific companies/systems when possible)

### Then Include
- 3 key tradeoffs with explicit "choose X when... choose Y when..." guidance
- 2 real-world system examples that use this concept
- 2 "what breaks if misunderstood?" cases
- 3 reasoning-heavy self-test questions (not trivia — questions that require thinking through scenarios)

## Check Understanding
Before wrapping up, ask the learner to restate the core concept in their own words.

## Output
Write the completed deep dive to `notes/YYYY-MM-DD-[topic-slug].md` using today's date and a kebab-case slug of the topic name. Use the template from `notes/_template.md` as the starting structure.

After writing the file, suggest what to study next based on the roadmap.
