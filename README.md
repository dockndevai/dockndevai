# Hi, I'm Ankit 👋

I build **safe-by-default MCP servers** — so AI agents can operate real infrastructure without being handed the keys.

## 🔐 The MCP server suite

A family of [Model Context Protocol](https://modelcontextprotocol.io) servers that share one governance model: **read-only by default**, layered access modes, resource allowlists, protected resources, delete gating, **typed confirmation** for high-impact ops, **secret redaction**, dry-run, and JSON audit logging. All MIT-licensed and on npm as `@dockndevai/mcp-*`.

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

Each works with Claude, Cursor, OpenAI Codex, VS Code, and Windsurf — per-client setup in every repo's `docs/CLIENTS.md`.

⭐ **If any of these save you time, a star helps other engineers find them.**
