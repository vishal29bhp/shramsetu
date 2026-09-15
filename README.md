# ShramSetu

**श्रम सेतु — "the labour bridge."** A trust-first marketplace connecting India's informal,
blue-collar and grey-collar workforce with verified employers, contractors and staffing agencies.

The platform closes four structural gaps in the informal labour market: **discovery** (geo + skill
matching instead of middlemen), **trust** (eKYC-backed identity and a portable work record),
**payment** (escrowed wages settled T+1 instead of delayed cash), and **mobility** (a verifiable
skill passport that travels between employers).

## Surfaces

| Surface | Stack |
|---------|-------|
| Worker app (Android, iOS) | React Native + TypeScript, offline-first |
| Employer / supervisor app | React Native + TypeScript |
| Employer & ops web console | React 18 + Vite + TypeScript |
| Backend | Python 3.12, FastAPI, PostgreSQL, Kafka, Kubernetes |

## Documentation

- **[System Design Specification](docs/SYSTEM_DESIGN.md)** — the full technical specification:
  requirements, high-level architecture, workflows, low-level module design, data models, and
  resilience/security/trade-off analysis, with 15 rendered Mermaid diagrams.

### Specification contents

| Section | Covers |
|---------|--------|
| 1 · System Overview & Requirements | Business context, 13 functional modules, scale/latency/availability targets |
| 2 · High-Level Design | Architecture style, component responsibilities, macro architecture, C4 context, deployment topology, repo layout |
| 3 · Workflow & Process Flow | End-to-end worker journey, employer requisition flow, offline sync workflow |
| 4 · Low-Level Design | Module internals with code, 5 sequence diagrams, state machines, API and event contracts |
| 5 · Data Models & Storage | Polyglot persistence rationale, ER model, physical schema, partitioning, caching, retention |
| 6 · Resilience, Security & Trade-offs | 15 failure modes, layered security architecture, 8 documented trade-offs, delivery roadmap |
