# Hi, I'm Ankit 👋

I build **safe-by-default, open-source engineering** across the stack — **AI agents, identity, and data platforms** — so systems can do real work without being handed the keys.

🌐 **[dockndevai.github.io](https://dockndevai.github.io/)** — everything on one page, with the security model, live stats, and copy-paste installs.
✍️ I write about how it's actually built on **[Medium](https://medium.com/@dockndev)** and **[Dev.to](https://dev.to/dockndevai)**.

Six areas, one principle — **least privilege, enforced, not documented:**

🤖 AI agent tooling (MCP) · 🔐 Identity & Keycloak · 📚 RAG & LLM platforms · 🧠 On-device AI · 🎙️ Voice · 🧪 Kubernetes labs

---

## 🤖 AI agent tooling — the MCP server suite

A family of [Model Context Protocol](https://modelcontextprotocol.io) servers that share one governance model: **read-only by default**, layered access modes, resource allowlists, protected resources, delete gating, **typed confirmation** for high-impact ops, **secret redaction**, dry-run, and JSON audit logging. Mostly MIT-licensed and on npm as `@dockndevai/mcp-*` (plus the Apache-2.0 `ossian-mcp`).

| Server | What it does | Install | Stars |
|---|---|---|---|
| [**mcp-kubernetes**](https://github.com/dockndevai/mcp-kubernetes) | Pods, logs, deployments, scale/restart, apply, exec | `npx -y @dockndevai/mcp-kubernetes` | ![](https://img.shields.io/github/stars/dockndevai/mcp-kubernetes?style=social) |
| [**mcp-openshift**](https://github.com/dockndevai/mcp-openshift) | OpenShift / Kubernetes — projects, pods, logs, routes, deployments; token or username/password | `npx -y @dockndevai/mcp-openshift` | ![](https://img.shields.io/github/stars/dockndevai/mcp-openshift?style=social) |
| [**mcp-kafka**](https://github.com/dockndevai/mcp-kafka) | Topics, consumer groups + lag, create/alter/reset | `npx -y @dockndevai/mcp-kafka` | ![](https://img.shields.io/github/stars/dockndevai/mcp-kafka?style=social) |
| [**mcp-clickhouse**](https://github.com/dockndevai/mcp-clickhouse) | Schema, queries, SQL-classified read/write/destructive gating | `npx -y @dockndevai/mcp-clickhouse` | ![](https://img.shields.io/github/stars/dockndevai/mcp-clickhouse?style=social) |
| [**mcp-debezium**](https://github.com/dockndevai/mcp-debezium) | CDC connector status, config, lifecycle | `npx -y @dockndevai/mcp-debezium` | ![](https://img.shields.io/github/stars/dockndevai/mcp-debezium?style=social) |
| [**mcp-oci**](https://github.com/dockndevai/mcp-oci) | Oracle Cloud discovery + Terraform generation | `npx -y @dockndevai/mcp-oci` | ![](https://img.shields.io/github/stars/dockndevai/mcp-oci?style=social) |
| [**mcp-azure**](https://github.com/dockndevai/mcp-azure) | Azure Resource Manager inventory, tags, VM power, lifecycle | `npx -y @dockndevai/mcp-azure` | ![](https://img.shields.io/github/stars/dockndevai/mcp-azure?style=social) |
| [**mcp-azure-devops**](https://github.com/dockndevai/mcp-azure-devops) | Boards, repos, pipelines, projects | `npx -y @dockndevai/mcp-azure-devops` | ![](https://img.shields.io/github/stars/dockndevai/mcp-azure-devops?style=social) |
| [**mcp-github-enterprise**](https://github.com/dockndevai/mcp-github-enterprise) | GitHub Enterprise — orgs, repos, teams, rulesets, security alerts & Actions, with a security-posture baseline | `npx -y @dockndevai/mcp-github-enterprise` | ![](https://img.shields.io/github/stars/dockndevai/mcp-github-enterprise?style=social) |
| [**mcp-keycloak**](https://github.com/dockndevai/mcp-keycloak) | Realms, users, clients, roles, groups | `npx -y @dockndevai/mcp-keycloak` | ![](https://img.shields.io/github/stars/dockndevai/mcp-keycloak?style=social) |
| [**mcp-percona-pg**](https://github.com/dockndevai/mcp-percona-pg) | Percona PostgreSQL + PgBouncer: pooling, tuning, backups/PITR, DR, upgrades | `npx -y @dockndevai/mcp-percona-pg` | ![](https://img.shields.io/github/stars/dockndevai/mcp-percona-pg?style=social) |
| [**mcp-grafana**](https://github.com/dockndevai/mcp-grafana) | Dashboards, datasource queries (PromQL/LogQL/SQL), alerts & annotations | `npx -y @dockndevai/mcp-grafana` | ![](https://img.shields.io/github/stars/dockndevai/mcp-grafana?style=social) |
| [**ossian-mcp**](https://github.com/dockndevai/ossian-mcp) | Ask your own documents with citations + durable agent memory (RAG) | `npx -y ossian-mcp` | ![](https://img.shields.io/github/stars/dockndevai/ossian-mcp?style=social) |
| [**mcp-outlook**](https://github.com/dockndevai/mcp-outlook) | Outlook mail + OneDrive files (Microsoft Graph) — read, search, draft, send; browser sign-in | `npx -y @dockndevai/mcp-outlook` | ![](https://img.shields.io/github/stars/dockndevai/mcp-outlook?style=social) |
| [**mcp-teams**](https://github.com/dockndevai/mcp-teams) | Microsoft Teams (Microsoft Graph) — teams, channels, chats & messages, post/reply/send; browser sign-in | `npx -y @dockndevai/mcp-teams` | ![](https://img.shields.io/github/stars/dockndevai/mcp-teams?style=social) |
| [**mcp-macos**](https://github.com/dockndevai/mcp-macos) | Observe & operate a Mac — files, processes, apps, screenshots, shell, AppleScript, GUI (safe by default) | `npx -y @dockndevai/mcp-macos` | ![](https://img.shields.io/github/stars/dockndevai/mcp-macos?style=social) |
| [**mcp-mac-control**](https://github.com/dockndevai/mcp-mac-control) | Full Mac control — drive it like a human: shell, AppleScript, files, and GUI; opt-in safe mode | `npx -y @dockndevai/mcp-mac-control` | ![](https://img.shields.io/github/stars/dockndevai/mcp-mac-control?style=social) |
| [**mcp-android**](https://github.com/dockndevai/mcp-android) | Control an Android device over ADB — screenshots, taps, typing, app launch, notifications | `npx -y @dockndevai/mcp-android` | ![](https://img.shields.io/github/stars/dockndevai/mcp-android?style=social) |
| [**mcp-ios**](https://github.com/dockndevai/mcp-ios) | Drive a physical iPhone/iPad over Appium + WebDriverAgent (XCUITest) | `npx -y @dockndevai/mcp-ios` | ![](https://img.shields.io/github/stars/dockndevai/mcp-ios?style=social) |
| [**mcp-cdp**](https://github.com/dockndevai/mcp-cdp) | Drive an Electron/Chrome app over the DevTools Protocol — DOM, console, network, gated JS eval. Cross-OS alternative to computer-use for testing apps | `npx -y @dockndevai/mcp-cdp` | ![](https://img.shields.io/github/stars/dockndevai/mcp-cdp?style=social) |
| [**mcp-laya**](https://github.com/dockndevai/mcp-laya) | Fast, local, typed decisions for agents (classify/score/yes-no) in 100+ languages — no hallucination | `pipx install mcp-laya` | ![](https://img.shields.io/github/stars/dockndevai/mcp-laya?style=social) |

Each works with Claude, Cursor, OpenAI Codex, VS Code, and Windsurf — per-client setup in every repo's `docs/CLIENTS.md`.

> 🛡️ **[laya-guard](https://github.com/dockndevai/laya-guard)** — an optional, fully-local AI risk guard for the servers above. High-risk commands (shell, `evaluate`, apply/delete/exec) are classified allow/confirm/block by a local decision model *before* they run — defense in depth that only ever tightens, never grants. Wired into every mutating server in the suite.

> 🧩 **[mcp-core](https://github.com/dockndevai/mcp-core)** — the shared governance library every server above is built on: access modes, the guard, resource allowlists, elicitation confirm, symlink-safe path handling, secret redaction and audit — one audited implementation instead of twenty that drift. On npm as `@dockndevai/mcp-core`.

## 🔐 Identity & Keycloak

Production Keycloak SPIs in Java — the two things teams hit first: consistent branding across realms, and real tenant isolation.

| Project | What it is |
|---|---|
| [**keycloak-configurable-theme**](https://github.com/dockndevai/keycloak-configurable-theme) | Keycloak 26.x SPI: one configurable theme for *all* realms — layout, colours, logo, favicon, console & email branding via JSON, admin console or REST. |
| [**keycloak-realm-database-router**](https://github.com/dockndevai/keycloak-realm-database-router) | Keycloak SPI: one database per realm — hard multi-tenant isolation at the data layer, with a Docker Compose stack and load tests. |
| [**mcp-keycloak**](https://github.com/dockndevai/mcp-keycloak) | The agent adapter — multi-realm Keycloak admin over MCP, same safe-by-default model as the suite. |

## 📚 RAG & LLM platforms

The agent tools sit on top of real platforms I also build and run.

| Project | What it is |
|---|---|
| [**ossian**](https://github.com/dockndevai/ossian) | Open-book RAG over your own documents — Spring Boot + Spring AI, a React console, Keycloak OAuth2, Postgres/pgvector and Redis. Answers with citations, plus a maintenance side for ingestion, re-indexing and coverage gaps. |
| [**ossian-kafka-connect**](https://github.com/dockndevai/ossian-kafka-connect) | A Kafka Connect sink for Ossian — turns Debezium CDC events into RAG documents with citations, so the knowledge base stays live. |
| [**spring-llm-gateway**](https://github.com/dockndevai/spring-llm-gateway) | An LLM gateway on Spring Cloud Gateway (WebFlux): virtual keys, token quotas, usage metering and failover for self-hosted OpenAI-compatible backends (vLLM, Ollama). |

## 🧠 On-device AI & 🎙️ voice

Small models that run where the data is — **Laya** is a tiny typed-decision model that runs locally (browser, Mac, Raspberry Pi) with nothing uploaded.

| Project | What it is |
|---|---|
| [**laya-models**](https://github.com/dockndevai/laya-models) | The Laya decision model, converted to ONNX so it runs in the browser — no server round-trip. |
| [**mac-attack**](https://github.com/dockndevai/mac-attack) | A macOS game & real screensaver: the camera turns people into cartoons and Laya directs harmless toy chaos — ~340 ms/decision on an M2 Pro. Body rectangles only, no face recognition, nothing uploaded. |
| [**pi-meeting-assistant**](https://github.com/dockndevai/pi-meeting-assistant) | A voice-controlled robot arm on a Raspberry Pi: local STT + Laya decisions in English, Hinglish and Hindi — no LLM in the loop. Plus a live meeting assistant. |
| [**otto-assist**](https://github.com/dockndevai/otto-assist) | A realtime, voice-driven assistant with Claude as the brain: local Whisper STT, streaming TTS with barge-in, subagents, and a web dashboard. ([Homebrew tap](https://github.com/dockndevai/homebrew-otto)) |

## 🧪 Hands-on Kubernetes labs

Runnable reference environments — every claim measured, every failure documented. Each pairs with an MCP server above.

| Lab | What it covers |
|---|---|
| [**percona-pg-lab**](https://github.com/dockndevai/percona-pg-lab) | PostgreSQL + PgBouncer on Kubernetes with the Percona Operator — HA, DR, pooling, backups, observability. Pairs with `mcp-percona-pg`. |
| [**kafka-lifecycle-lab**](https://github.com/dockndevai/kafka-lifecycle-lab) | Apache Kafka on Kubernetes with Strimzi — provision, upgrade, DR with MirrorMaker 2, read-only agent triage. Pairs with `mcp-kafka`. |
| [**clickhouse-lab**](https://github.com/dockndevai/clickhouse-lab) | ClickHouse on Kubernetes with the Altinity operator — ReplicatedMergeTree, upgrades, online PVC expansion, backups, cross-region DR. Pairs with `mcp-clickhouse`. |

## ✍️ Writing

Build logs & deep dives on **[Medium](https://medium.com/@dockndev)** and **[Dev.to](https://dev.to/dockndevai)** — the bugs, the trade-offs, and the governance decisions behind these systems.

---

⭐ **If any of these save you time, a star helps other engineers find them.**
