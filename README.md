# Hi, I'm Ankit 👋

I build **safe-by-default MCP servers** — so AI agents can work with real systems, from infrastructure to your own documents, without being handed the keys.

## 🔐 The MCP server suite

🌐 **[dockndevai.github.io](https://dockndevai.github.io/)** — the whole suite on one page, with the security model and copy-paste installs.

A family of [Model Context Protocol](https://modelcontextprotocol.io) servers that share one governance model: **read-only by default**, layered access modes, resource allowlists, protected resources, delete gating, **typed confirmation** for high-impact ops, **secret redaction**, dry-run, and JSON audit logging. Mostly MIT-licensed and on npm as `@dockndevai/mcp-*` (plus the Apache-2.0 `ossian-mcp`).

| Server | What it does | Install | Stars |
|---|---|---|---|
| [**mcp-kubernetes**](https://github.com/dockndevai/mcp-kubernetes) | Pods, logs, deployments, scale/restart, apply, exec | `npx -y @dockndevai/mcp-kubernetes` | ![](https://img.shields.io/github/stars/dockndevai/mcp-kubernetes?style=social) |
| [**mcp-kafka**](https://github.com/dockndevai/mcp-kafka) | Topics, consumer groups + lag, create/alter/reset | `npx -y @dockndevai/mcp-kafka` | ![](https://img.shields.io/github/stars/dockndevai/mcp-kafka?style=social) |
| [**mcp-clickhouse**](https://github.com/dockndevai/mcp-clickhouse) | Schema, queries, SQL-classified read/write/destructive gating | `npx -y @dockndevai/mcp-clickhouse` | ![](https://img.shields.io/github/stars/dockndevai/mcp-clickhouse?style=social) |
| [**mcp-debezium**](https://github.com/dockndevai/mcp-debezium) | CDC connector status, config, lifecycle | `npx -y @dockndevai/mcp-debezium` | ![](https://img.shields.io/github/stars/dockndevai/mcp-debezium?style=social) |
| [**mcp-oci**](https://github.com/dockndevai/mcp-oci) | Oracle Cloud discovery + Terraform generation | `npx -y @dockndevai/mcp-oci` | ![](https://img.shields.io/github/stars/dockndevai/mcp-oci?style=social) |
| [**mcp-azure**](https://github.com/dockndevai/mcp-azure) | Azure Resource Manager inventory, tags, VM power, lifecycle | `npx -y @dockndevai/mcp-azure` | ![](https://img.shields.io/github/stars/dockndevai/mcp-azure?style=social) |
| [**mcp-azure-devops**](https://github.com/dockndevai/mcp-azure-devops) | Boards, repos, pipelines, projects | `npx -y @dockndevai/mcp-azure-devops` | ![](https://img.shields.io/github/stars/dockndevai/mcp-azure-devops?style=social) |
| [**mcp-keycloak**](https://github.com/dockndevai/mcp-keycloak) | Realms, users, clients, roles, groups | `npx -y @dockndevai/mcp-keycloak` | ![](https://img.shields.io/github/stars/dockndevai/mcp-keycloak?style=social) |
| [**mcp-percona-pg**](https://github.com/dockndevai/mcp-percona-pg) | Percona PostgreSQL + PgBouncer: pooling, tuning, backups/PITR, DR, upgrades | `npx -y @dockndevai/mcp-percona-pg` | ![](https://img.shields.io/github/stars/dockndevai/mcp-percona-pg?style=social) |
| [**mcp-grafana**](https://github.com/dockndevai/mcp-grafana) | Dashboards, datasource queries (PromQL/LogQL/SQL), alerts & annotations | `npx -y @dockndevai/mcp-grafana` | ![](https://img.shields.io/github/stars/dockndevai/mcp-grafana?style=social) |
| [**ossian-mcp**](https://github.com/dockndevai/ossian-mcp) | Ask your own documents with citations + durable agent memory (RAG) | `npx -y ossian-mcp` | ![](https://img.shields.io/github/stars/dockndevai/ossian-mcp?style=social) |
| [**mcp-macos**](https://github.com/dockndevai/mcp-macos) | Observe & operate a Mac — files, processes, apps, screenshots, shell, AppleScript, GUI (safe by default) | `npx -y @dockndevai/mcp-macos` | ![](https://img.shields.io/github/stars/dockndevai/mcp-macos?style=social) |
| [**mcp-outlook**](https://github.com/dockndevai/mcp-outlook) | Outlook mail (Microsoft Graph) — read, search, draft, send, reply, organize; browser sign-in | `npx -y @dockndevai/mcp-outlook` | ![](https://img.shields.io/github/stars/dockndevai/mcp-outlook?style=social) |
| [**mcp-teams**](https://github.com/dockndevai/mcp-teams) | Microsoft Teams (Microsoft Graph) — read teams, channels, chats & messages, post/reply/send; browser sign-in | `npx -y @dockndevai/mcp-teams` | ![](https://img.shields.io/github/stars/dockndevai/mcp-teams?style=social) |

Each works with Claude, Cursor, OpenAI Codex, VS Code, and Windsurf — per-client setup in every repo's `docs/CLIENTS.md`.

## 🧠 The platforms behind them

The agent tools sit on top of real systems I also build and run.

| Project | What it is |
|---|---|
| [**ossian**](https://github.com/dockndevai/ossian) | Open-book RAG over your own documents — Spring Boot + Spring AI, a React console, Keycloak OAuth2, Postgres/pgvector and Redis. Answers with citations, plus a maintenance side for ingestion, re-indexing and coverage gaps. `ossian-mcp` is its agent adapter. |
| [**spring-llm-gateway**](https://github.com/dockndevai/spring-llm-gateway) | An LLM gateway on Spring Cloud Gateway (WebFlux): virtual keys, token quotas, usage metering and failover for self-hosted OpenAI-compatible backends (vLLM, Ollama). |

## 🎙️ Otto — a voice for the Claude you already run

A realtime, voice-driven assistant with Claude as the brain: local Whisper STT, streaming TTS with barge-in, subagents, and a web dashboard.

- [**orrin-site**](https://github.com/dockndevai/orrin-site) — the site
- [**homebrew-otto**](https://github.com/dockndevai/homebrew-otto) — a `brew` tap to install it

## 🧪 Hands-on labs

Runnable reference environments — every claim measured, every failure documented. Each pairs with an MCP server above.

| Lab | What it covers |
|---|---|
| [**percona-pg-lab**](https://github.com/dockndevai/percona-pg-lab) | PostgreSQL + PgBouncer on Kubernetes with the Percona Operator — HA, DR, connection pooling, backups, observability. Pairs with `mcp-percona-pg`. |
| [**kafka-lifecycle-lab**](https://github.com/dockndevai/kafka-lifecycle-lab) | Operating Apache Kafka on Kubernetes with Strimzi — provision, upgrade, DR with MirrorMaker 2, and read-only agent triage. Pairs with `mcp-kafka`. |

⭐ **If any of these save you time, a star helps other engineers find them.**
