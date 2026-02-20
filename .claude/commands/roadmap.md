View and update the learning roadmap.

## Instructions

1. Read `CLAUDE.md` for learner context.
2. Read `roadmap.md` for the current state of the roadmap.
3. Scan artifacts in `notes/`, `designs/`, `reviews/`, `adrs/`, and `reflections/` to understand what has been completed.

## Process

### If `roadmap.md` is a skeleton/placeholder (first run):

Build a personalized, phase-based learning roadmap. Start from the learner's background (backend engineer, Kotlin, framework/infra team) and goals (Senior → Staff system design thinking).

#### Phase Structure:

**Phase 0: Core Foundations**
- Networking basics (TCP/IP, HTTP, DNS)
- Client-server model
- How databases work (at a high level)
- What happens when you type a URL in a browser
- API design basics (REST, request/response)
- *Why this phase*: Many engineers jump to distributed systems without solid fundamentals. This phase fills gaps without being condescending.

**Phase 1: Storage & Data Fundamentals**
- How relational databases work under the hood
- Indexing and query optimization
- SQL vs NoSQL tradeoffs
- Caching fundamentals
- Data modeling

**Phase 2: Distributed Systems Fundamentals**
- Why distribution is necessary
- CAP theorem and its practical implications
- Consistency models
- Replication strategies
- Partitioning/sharding

**Phase 3: Scalability Patterns**
- Load balancing
- Message queues and async processing
- CDNs and edge computing
- Rate limiting and backpressure
- Connection pooling

**Phase 4: System Design Practice**
- Design exercises of increasing complexity
- Architecture review practice
- ADR writing

**Phase 5: Advanced Topics**
- Consensus algorithms
- Distributed transactions
- Event sourcing and CQRS
- Stream processing
- Multi-region architectures

For each topic within a phase, track:
- Status: not started / in progress / completed
- Related artifacts (links to files in the repo)

Include mastery signals for each phase — how the learner knows they're ready to advance.

### If `roadmap.md` already has content:

1. Review completed artifacts and update topic statuses
2. Identify what's been completed since last update
3. Suggest the next 2-3 topics to tackle
4. Note any gaps that have become apparent
5. Adjust the roadmap if the learner's needs have evolved

## Output
Update `roadmap.md` in place. Present a summary of changes and recommended next steps to the learner.
