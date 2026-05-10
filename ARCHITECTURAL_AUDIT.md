# Architectural Audit: n8n

**Date:** 2026-02-15
**Target:** `n8n` (Self-Hosted)
**Auditor:** Principal Systems Architect

## 1) Executive Summary
**Architecture:** Docker Compose Deployment.
**Verdict:** **Infrastructure.**
A self-hosted instance of n8n (Workflow Automation) using Docker Compose.

## 2) Recommendations
- **Persistence:** Ensure the Docker volumes for n8n data are backed up regularly.
- **Security:** If exposed to the internet, ensure it is behind a reverse proxy with Basic Auth or OAuth on top of n8n's built-in auth.
