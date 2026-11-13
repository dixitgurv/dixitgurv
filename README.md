### Gaurav Dixit

Engineering lead and software architect in Ashburn, VA. Sixteen years of Java and Spring Boot services on AWS for various financial institutions, from the first design doc to the dashboards that keep them running.

Most of my day job is private, so this profile holds small, complete projects in the areas I work in now: **applied AI that has to be measured before it ships**, and **database performance**.

#### Projects

**[pg-perf-mcp-spring](https://github.com/dixitgurv/pg-perf-mcp-spring)**: An MCP server in Spring Boot 4 and Spring AI that lets an AI agent diagnose PostgreSQL performance like a DBA. Eight plan-analysis rules read EXPLAIN ANALYZE output and flag misestimates, disk sorts, unindexed foreign keys and wasted scans, each with the fix written out. Read-only in four layers, down to the Postgres session. Tested on PostgreSQL 17 with Testcontainers, and end to end by driving the packaged jar with the MCP Java client. On the demo database, its findings take a join from 30.8 ms to 0.15 ms. (Also in [Python](https://github.com/dixitgurv/pg-perf-mcp).)
`Java` `Spring Boot 4` `Spring AI` `MCP` `PostgreSQL` `Testcontainers`

**[springboot4-jackson3-demo](https://github.com/dixitgurv/springboot4-jackson3-demo)**: Every Jackson 2 → 3 behaviour change that can break a running Spring Boot service, each pinned by a test, with a migration checklist. Includes the one that turns yesterday's valid requests into 400s.
`Java` `Spring Boot 4` `Jackson 3` `JUnit`

**[lora-eval-gate](https://github.com/dixitgurv/lora-eval-gate)**: LoRA fine-tune of Qwen2.5-0.5B for text-to-SQL, plus the evaluation harness and promotion gate that decide whether it may replace the base model. Execution-based scoring on synthetic databases, an exact McNemar test on paired outcomes, and per-category regression checks. The gate runs in CI. Result: 40.8% → 80.0% execution accuracy on a 400-example held-out set, with an honest breakdown of where the gain comes from.
`Python` `PyTorch` `PEFT` `transformers` `SQLite`

#### What I work on

- **System design:** greenfield services, event-driven architecture on Kafka, API contracts and design reviews
- **AI engineering:** fine-tuning, evaluation harnesses and regression gates, MCP servers, LLM-based scoring in production
- **Database tuning:** Oracle AWR/ASH, execution plans, indexing and partitioning, PostgreSQL EXPLAIN
- **Platform:** AWS, Kubernetes, Jenkins CI/CD, Terraform, OpenTelemetry

dixitgurv@gmail.com
