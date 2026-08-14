# Security Baseline

## Authentication

Spring Security authentication is planned. Passwords will be hashed and never logged or stored as plaintext.

## Authorization, JWT, and RBAC

JWTs will carry limited identity/role claims. Services will enforce role and resource permissions, not merely trust the frontend. Patient, clinical, pharmacy, billing, emergency, and administrative access will remain separated.

## Secret Management

- `.env` and environment variables are planned for local development.
- `.env.example` contains placeholders only.
- Gemini, JWT, PostgreSQL, and AWS secrets must not enter Git, frontend bundles, logs, screenshots, or API examples.
- Later environments should inject protected secrets through GitHub/Kubernetes/AWS mechanisms.

## API Security

Planned controls include HTTPS, request validation, secure error messages, JWT validation, RBAC, rate limiting, CORS policy, dependency timeouts, and audit/correlation IDs.

## Healthcare Data Protection

Only synthetic/test healthcare data is permitted. Logs and metrics will minimize sensitive content. No real patient or confidential institutional information may be uploaded.

## AI Safety

- The frontend will never call Gemini directly.
- AI output is untrusted until validated and reviewed.
- Agents cannot autonomously diagnose, prescribe, or execute sensitive decisions.
- Prompt-injection defenses, minimum-necessary context, timeout/fallback behavior, and human approval are planned.

## Secure Development

The team will use Jira-linked feature branches, pull requests, code reviews, dependency hygiene, input validation, and meaningful security tests. High-risk findings require remediation or documented acceptance.

## DevSecOps Plan

- SonarQube for static quality/security analysis.
- Trivy for dependency, container, and configuration scanning.
- OWASP ZAP for dynamic web/API testing.
- Real reports will be stored under `results/`; no Day 1 result is claimed.

