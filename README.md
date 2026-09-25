# Awesome System Design

A curated, opinionated list of resources to go deep in System Design: how systems are organised, scale and fail safely. Curated by [Felipe Guedes](https://fgxdev.com). Every entry has a one-line reason to read it; if I could not write the reason, it is not here.

Contributions welcome via pull request, with the same rule: one line on why.

## Foundations

- **Designing Data-Intensive Applications**, Martin Kleppmann. The book. Replication, partitioning, transactions and consistency explained from first principles.
- **Release It!**, Michael Nygard. Stability patterns (timeouts, circuit breakers, bulkheads) from real outages. Read before your first on-call.
- **Site Reliability Engineering** (Google, free online). SLOs, error budgets, toil. The vocabulary the whole industry uses.
- **The Twelve-Factor App**. Short, old, still the baseline for anything deployed more than once.

## Distributed systems

- **Jepsen analyses** (jepsen.io). What databases actually do under partitions, versus what their marketing says.
- **"Time, Clocks, and the Ordering of Events in a Distributed System"**, Lamport (1978). The paper behind every "happens-before".
- **"Paxos Made Simple"**, Lamport, and **"In Search of an Understandable Consensus Algorithm" (Raft)**, Ongaro and Ousterhout. Read Raft first, then Paxos.
- **Fallacies of Distributed Computing**. Eight sentences. Print them.
- **"Life beyond Distributed Transactions"**, Pat Helland. Why entities, idempotence and messages beat distributed transactions.

## Data and storage

- **PostgreSQL documentation**, chapters on MVCC, indexes and transactions. Better than most books.
- **"The Log: What every software engineer should know about real-time data's unifying abstraction"**, Jay Kreps. Why logs are the primitive under queues, replication and CDC.
- **Use The Index, Luke** (use-the-index-luke.com). SQL indexing explained for developers.
- **Transactional outbox and CDC**: the Debezium documentation is the practical reference.

## Messaging and events

- **Enterprise Integration Patterns**, Hohpe and Woolf. The vocabulary of queues, routers and translators; the website is enough.
- **"Exactly-once" is a spectrum**: read your broker's documentation on delivery guarantees, then design idempotent consumers anyway.

## Resilience and operations

- **Google SRE Workbook**, the practical companion to the SRE book.
- **Incident postmortem collections**: read public postmortems from cloud providers and large companies. Every one is a free lesson about a boundary someone trusted.
- **Chaos engineering principles** (principlesofchaos.org). Short manifesto; the practice is testing fallbacks before the incident does.

## Security as part of design

- **OWASP Application Security Verification Standard (ASVS)**. The checklist behind every serious application audit.
- **OWASP Top 10** and **OWASP API Security Top 10**. Where the findings actually are.
- **Threat modeling** (Adam Shostack, "Threat Modeling: Designing for Security"). Four questions: what are we building, what can go wrong, what do we do about it, did we do a good job.

## Architecture and decisions

- **Architecture Decision Records** (Michael Nygard's original post). One page per expensive decision.
- **"A Note on Distributed Computing"**, Waldo et al. (1994). Why local and remote calls are different and always will be.
- **Team Topologies**, Skelton and Pais. Conway's law applied on purpose.
- **Modular monoliths**: search for talks by Simon Brown. The right default for most products.

## Capacity and performance

- **Systems Performance**, Brendan Gregg. Methodology (USE, RED) before tools.
- **"Latency numbers every programmer should know"**. The table; update it every few years.
- **Little's Law**. One formula that sizes every queue and pool.

## Interviews are not the point, but

- **System Design Primer** (open source on GitHub). Broad coverage; use it as a map, not as the territory.
- The best preparation is a real incident. Volunteer for on-call.

## Em português

Lista curada de recursos para se aprofundar em System Design, com uma linha sobre por que ler cada um. Artigos em português sobre o tema em [fgxdev.com/pt/articles](https://fgxdev.com/pt/articles/tag/system-design/).

## License

Apache-2.0 for the list and its commentary. Copyright (c) 2026 Felipe Guedes (fgxdev.com). Each linked resource keeps its own license.
