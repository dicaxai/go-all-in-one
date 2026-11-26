# 🧰 go-all-in-one

[![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE.md)

A Go API starter that gets the fundamentals right from the start: two services, real authentication, OAuth 2 for third-party apps, and the tests and tooling to keep it that way.

- **Event-sourced user service.** DDD aggregate, versioned events with upcasters, projections in the same transaction, and a transactional outbox for email.
- **OAuth 2 auth service.** Email and Google sign-in, rotating refresh tokens with reuse detection, authorization code with PKCE, client credentials, ES256 access tokens (RFC 9068) verified through JWKS.
- **Three stores, one contract.** Memory, MySQL, or MongoDB, chosen at build time; every backend passes the same contract suites.
- **Ready for AI-assisted work.** `AGENTS.md` in every area, code standards, recipes for common changes, and import rules enforced by a test.

## Quick start

Docker is required.

```bash
git clone https://github.com/vardius/go-api-boilerplate.git
cd go-api-boilerplate
docker compose up --wait
