# oasync — ChatGPT → GitHub → tham-oracle Connector

Mailbox-v1 schema for routing ChatGPT messages through GitHub workflows into tham-oracle.

## Quick Start

ChatGPT commits JSON to `inbox/` → GitHub Connector workflow runs → output lands in tham-oracle `ψ/inbox/github/`

See `inbox/README.md` for message schema.

## Files

- `.github/workflows/github-connector.yml` — Process ChatGPT messages, run shell, commit output
- `inbox/` — Message drop zone
- `inbox/README.md` — Mailbox-v1 schema

## Usage

From tham-oracle:
```bash
bash scripts/oasync-push.sh "your message"
```

---
**Created**: 2026-05-17 | **Connector**: tham-oracle GitHub Connector v1
