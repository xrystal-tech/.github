# Xrystal

[![@xrystal/core](https://img.shields.io/npm/v/@xrystal/core?label=@xrystal%2Fcore&color=CB3837)](https://www.npmjs.com/package/@xrystal/core)
[![@xrystal/dto](https://img.shields.io/npm/v/@xrystal/dto?label=@xrystal%2Fdto&color=CB3837)](https://www.npmjs.com/package/@xrystal/dto)
[![policies](https://img.shields.io/badge/policies-EN%20%7C%20TR-4f46e5)](https://github.com/xrystal-tech/.github)

**Xrystal** is an engineering org for typed API platforms on **Bun**, **TypeScript**, and **Elysia**. The work we publish is open source: npm libraries, microservices on a shared runtime, and the GitOps-minded ops around shipping them. Docs and policies are **English and Turkish** by default.

We like small pieces that compose—loaders, DTOs, gateways—so every service returns the same JSON shape, traces requests the same way, and ships with the same **`xry`** workflow. An idea is not finished until it runs behind a clear contract and someone else can trust it in production.

## Libraries

[-xrystal-core](https://github.com/xrystal-tech/-xrystal-core) (`@xrystal/core`) is the runtime and **`xry`** CLI: Awilix DI, live `x/tmp.yml`, `ctr()` controllers, i18n and trace, optional Redis / MongoDB / Kafka loaders, plus HTTP, WebSocket, and Socket.IO on one pattern. Published on [npm](https://www.npmjs.com/package/@xrystal/core).

[dto](https://github.com/xrystal-tech/dto) (`@xrystal/dto`) is a framework-agnostic DTO layer for Express, Elysia, fetch, WebSocket, and Socket.IO—one JSON contract for API responses, structured logs, and queue messages. Published on [npm](https://www.npmjs.com/package/@xrystal/dto).

## API services

Reference microservices built on `@xrystal/core` and `@xrystal/dto`. Same middleware, gateway routing, env layout, and release gates.

| Service | Role |
| --- | --- |
| [api-gateway-svc](https://github.com/xrystal-tech/api-gateway-svc) | Edge HTTP routing, auth, WebSocket / MQTT passthrough |
| [api-core-svc](https://github.com/xrystal-tech/api-core-svc) | Core platform APIs and shared domain behavior |
| [api-iam-svc](https://github.com/xrystal-tech/api-iam-svc) | Identity, JWT, sessions, permission scopes |
| [api-log-svc](https://github.com/xrystal-tech/api-log-svc) | Central structured logging and log pipeline |
| [api-websocket-svc](https://github.com/xrystal-tech/api-websocket-svc) | Realtime channels aligned with gateway routes |
| [api-cron-svc](https://github.com/xrystal-tech/api-cron-svc) | Scheduled jobs and background triggers |
| [api-gpt-svc](https://github.com/xrystal-tech/api-gpt-svc) | LLM-backed features behind the same DTO contract |

## Organization defaults

[.github](https://github.com/xrystal-tech/.github) holds MIT-by-default licensing, privacy, [SECURITY](https://github.com/xrystal-tech/.github/blob/main/SECURITY.md), contributing, and code of conduct—**EN / TR**. A repository’s own `LICENSE` applies when it explicitly overrides the org default.

[github.com/xrystal-tech](https://github.com/xrystal-tech) · questions and policy changes → [open an issue](https://github.com/xrystal-tech/.github/issues)