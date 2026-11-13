### Gaurav Dixit

Engineering lead and software architect in Ashburn, VA. Sixteen years of Java and Spring Boot services on AWS for various financial institutions, from the first design doc to the dashboards that keep them running.

Most of my day job is private, so this profile holds small, complete projects in the areas I work in now: **applied AI that has to be measured before it ships**, and **database performance**.

#### Projects

**[lora-eval-gate](https://github.com/dixitgurv/lora-eval-gate)**: LoRA fine-tune of Qwen2.5-0.5B for text-to-SQL, plus the evaluation harness and promotion gate that decide whether it may replace the base model. Execution-based scoring on synthetic databases, an exact McNemar test on paired outcomes, and per-category regression checks. The gate runs in CI. Result: 40.8% → 80.0% execution accuracy on a 400-example held-out set, with an honest breakdown of where the gain comes from.
`Python` `PyTorch` `PEFT` `transformers` `SQLite`

**[pg-perf-mcp](https://github.com/dixitgurv/pg-perf-mcp)**: An MCP server that lets an AI agent diagnose PostgreSQL performance. It reads EXPLAIN ANALYZE plans and flags misestimates, disk sorts, unindexed join keys and wasted scans, and it also reports slow queries, unused indexes and table bloat. Read-only by design, enforced at the session level as well as by query checks. On the demo database, its findings take a join from 34 ms to 0.7 ms.
`Python` `MCP` `PostgreSQL` `psycopg`

**[springboot4-jackson3-demo](https://github.com/dixitgurv/springboot4-jackson3-demo)**: Every Jackson 2 → 3 behaviour change that can break a running Spring Boot service, each pinned by a test, with a migration checklist. Includes the one that turns yesterday's valid requests into 400s.
`Java` `Spring Boot 4` `Jackson 3` `JUnit`

#### What I work on

- **System design:** greenfield services, event-driven architecture on Kafka, API contracts and design reviews
- **AI engineering:** fine-tuning, evaluation harnesses and regression gates, MCP servers, LLM-based scoring in production
- **Database tuning:** Oracle AWR/ASH, execution plans, indexing and partitioning, PostgreSQL EXPLAIN
- **Platform:** AWS, Kubernetes, Jenkins CI/CD, Terraform, OpenTelemetry

dixitgurv@gmail.com
