# THE ART OF BACKEND — The Complete Engineer's Bible

> *"A senior engineer isn't someone who knows everything — they're someone who knows what to reach for, when to reach for it, and why everything else exists."*

This is not a tutorial. This is your **complete map of the backend territory** — every concept, technology, pattern, and tool you will ever need as a backend engineer. From the first HTTP request to distributed systems at planetary scale.

**This document is a living index.** Each item is a teachable unit. Use it to navigate your learning, understand where you are, and know what comes next.

---

## How to Use This Bible

```
Say: "teach me [topic number or name]"
Say: "go deeper on [concept]"
Say: "compare [X] vs [Y]"
Say: "give me a real example of [topic]"
Say: "what should I learn next?"
Say: "ready to test" → switches to quiz mode
```

> Topics marked `[CORE]` are non-negotiable fundamentals.
> Topics marked `[ADVANCED]` assume Phase 1-5 are solid.
> Topics marked `[SPECIALIST]` are deep dives for specific career paths.

---

## TABLE OF CONTENTS

- [Phase 0 — Mental Models](#phase-0--mental-models--first-principles)
- [Phase 1 — Internet & Networking](#phase-1--internet--networking)
- [Phase 2 — Core Backend Concepts](#phase-2--core-backend-concepts)
- [Phase 3 — Languages & Runtimes](#phase-3--languages--runtimes)
- [Phase 4 — Web Frameworks](#phase-4--web-frameworks)
- [Phase 5 — Databases](#phase-5--databases)
- [Phase 6 — APIs & Communication](#phase-6--apis--communication-protocols)
- [Phase 7 — Caching](#phase-7--caching)
- [Phase 8 — Authentication & Security](#phase-8--authentication--security)
- [Phase 9 — Performance & Reliability](#phase-9--performance--reliability)
- [Phase 10 — Infrastructure & DevOps](#phase-10--infrastructure--devops)
- [Phase 11 — Cloud Platforms & Serverless](#phase-11--cloud-platforms--serverless)
- [Phase 12 — Messaging & Event-Driven Systems](#phase-12--messaging--event-driven-systems)
- [Phase 13 — Search & Analytics](#phase-13--search--analytics)
- [Phase 14 — Distributed Systems & Microservices](#phase-14--distributed-systems--microservices)
- [Phase 15 — Advanced Architecture Patterns](#phase-15--advanced-architecture-patterns)
- [Phase 16 — Data Engineering & Pipelines](#phase-16--data-engineering--pipelines)
- [Phase 17 — AI/ML Backend Integration](#phase-17--aiml-backend-integration)
- [Phase 18 — Observability & SRE](#phase-18--observability--sre)
- [Phase 19 — Testing & Quality](#phase-19--testing--quality)
- [Phase 20 — Career & System Design Interviews](#phase-20--career--system-design-interviews)

---

## PHASE 0 — Mental Models & First Principles

> Before you write a line of backend code, you need to understand how computers and networks actually work. Skip this and you will spend years cargo-culting solutions without understanding them.

| # | Topic | Tag |
|---|-------|-----|
| 0.1 | [How to think like a backend engineer — reasoning about systems](phases/phase-00-mental-models/0.01-think-like-a-backend-engineer.md) | `[CORE]` ✅ |
| 0.2 | [What "the backend" actually is — and what it isn't](phases/phase-00-mental-models/0.02-what-is-the-backend.md) | `[CORE]` ✅ |
| 0.3 | [How the internet physically works — cables, packets, hops](phases/phase-00-mental-models/0.03-how-the-internet-works.md) | `[CORE]` ✅ |
| 0.4 | [The OSI Model — 7 layers that explain every network tool](phases/phase-00-mental-models/0.04-osi-model.md) | `[CORE]` ✅ |
| 0.5 | [Latency, bandwidth, throughput — the three numbers governing every decision](phases/phase-00-mental-models/0.05-latency-bandwidth-throughput.md) | `[CORE]` ✅ |
| 0.6 | [The memory hierarchy — registers, L1/L2/L3 cache, RAM, disk, network](phases/phase-00-mental-models/0.06-memory-hierarchy.md) | `[CORE]` ✅ |
| 0.7 | [Binary, hexadecimal, and encoding — why your string is broken](phases/phase-00-mental-models/0.07-binary-hex-encoding.md) | `[CORE]` ✅ |
| 0.8 | [Character encoding deep dive — ASCII, UTF-8, Unicode, Base64](phases/phase-00-mental-models/0.08-character-encoding.md) | `[CORE]` ✅ |
| 0.9 | [Time zones, UTC, Unix timestamps — why dates destroy production systems](phases/phase-00-mental-models/0.09-timezones-utc-timestamps.md) | `[CORE]` ✅ |
| 0.10 | [Idempotency — the concept behind retry-safe systems](phases/phase-00-mental-models/0.10-idempotency.md) | `[CORE]` ✅ |
| 0.11 | [Determinism vs. non-determinism in distributed systems](phases/phase-00-mental-models/0.11-determinism.md) | `[ADVANCED]` ✅ |
| 0.12 | [The fallacies of distributed computing — 8 assumptions that will burn you](phases/phase-00-mental-models/0.12-fallacies-of-distributed-computing.md) | `[ADVANCED]` ✅ |
| 0.13 | [CAP theorem — consistency, availability, partition tolerance](phases/phase-00-mental-models/0.13-cap-theorem.md) | `[ADVANCED]` ✅ |
| 0.14 | [How a CPU executes code — processes, threads, context switching](phases/phase-00-mental-models/0.14-cpu-processes-threads.md) | `[CORE]` ✅ |
| 0.15 | [Synchronous vs. asynchronous — the most important mental model in backend](phases/phase-00-mental-models/0.15-sync-vs-async.md) | `[CORE]` ✅ |
| 0.16 | [Concurrency vs. parallelism — they are not the same thing](phases/phase-00-mental-models/0.16-concurrency-vs-parallelism.md) | `[CORE]` ✅ |
| 0.17 | [The cost of abstraction — why "it just works" is dangerous thinking](phases/phase-00-mental-models/0.17-cost-of-abstraction.md) | `[CORE]` ✅ |

---

## PHASE 1 — Internet & Networking

> Every backend system lives on a network. If you don't understand how data travels from point A to B, you cannot debug, optimize, or secure anything.

| # | Topic | Tag |
|---|-------|-----|
| 1.1 | [IP addresses — IPv4, IPv6, subnets, CIDR notation](phases/phase-01-internet-networking/1.01-ip-addresses.md) | `[CORE]` ✅ |
| 1.2 | [TCP — reliability, handshakes, flow control, why it's slow](phases/phase-01-internet-networking/1.02-tcp.md) | `[CORE]` ✅ |
| 1.3 | [UDP — speed over reliability, where and why it's used](phases/phase-01-internet-networking/1.03-udp.md) | `[CORE]` ✅ |
| 1.4 | [DNS — resolution pipeline, records (A, AAAA, CNAME, MX, TXT, SRV), TTL](phases/phase-01-internet-networking/1.04-dns.md) | `[CORE]` ✅ |
| 1.5 | [DNS internals — recursive resolvers, root servers, authoritative servers](phases/phase-01-internet-networking/1.05-dns-internals.md) | `[CORE]` ✅ |
| 1.6 | [HTTP/1.0 — the original, stateless, one request per connection](phases/phase-01-internet-networking/1.06-http1.md) | `[CORE]` ✅ |
| 1.7 | [HTTP/1.1 — persistent connections, pipelining, chunked transfer](phases/phase-01-internet-networking/1.07-http11.md) | `[CORE]` ✅ |
| 1.8 | [HTTP/2 — multiplexing, header compression (HPACK), server push, streams](phases/phase-01-internet-networking/1.08-http2.md) | `[CORE]` ✅ |
| 1.9 | [HTTP/3 & QUIC — UDP-based, 0-RTT, why it was built](phases/phase-01-internet-networking/1.09-http3-quic.md) | `[ADVANCED]` ✅ |
| 1.10 | [HTTPS — TLS handshake step by step, certificates, CAs, HSTS](phases/phase-01-internet-networking/1.10-https-tls.md) | `[CORE]` ✅ |
| 1.11 | [TLS 1.2 vs TLS 1.3 — differences, why you must upgrade](phases/phase-01-internet-networking/1.11-tls-versions.md) | `[ADVANCED]` ✅ |
| 1.12 | [HTTP headers deep dive — request, response, caching headers](phases/phase-01-internet-networking/1.12-http-headers.md) | `[CORE]` ✅ |
| 1.13 | [HTTP status codes — every range explained with production context](phases/phase-01-internet-networking/1.13-http-status-codes.md) | `[CORE]` ✅ |
| 1.14 | [Cookies — structure, attributes (SameSite, HttpOnly, Secure), scope](phases/phase-01-internet-networking/1.14-cookies.md) | `[CORE]` ✅ |
| 1.15 | [CORS — why it exists, preflight requests, how to configure it correctly](phases/phase-01-internet-networking/1.15-cors.md) | `[CORE]` ✅ |
| 1.16 | [CDNs — how content delivery networks work, edge caching, PoPs](phases/phase-01-internet-networking/1.16-cdns.md) | `[CORE]` ✅ |
| 1.17 | [Proxies vs. reverse proxies — the difference and when each is used](phases/phase-01-internet-networking/1.17-proxies.md) | `[CORE]` ✅ |
| 1.18 | [Load balancers — L4 vs L7, algorithms (round-robin, least-conn, IP hash)](phases/phase-01-internet-networking/1.18-load-balancers.md) | `[CORE]` ✅ |
| 1.19 | [NAT — network address translation, port mapping](phases/phase-01-internet-networking/1.19-nat.md) | `[ADVANCED]` ✅ |
| 1.20 | [Firewalls — stateful vs stateless, rules, security groups](phases/phase-01-internet-networking/1.20-firewalls.md) | `[ADVANCED]` ✅ |
| 1.21 | [VPNs & tunneling — how they work, site-to-site, client VPN](phases/phase-01-internet-networking/1.21-vpns.md) | `[ADVANCED]` ✅ |
| 1.22 | [Service mesh — what it is, Istio, Envoy, when you need one](phases/phase-01-internet-networking/1.22-service-mesh.md) | `[SPECIALIST]` ✅ |

---

## PHASE 2 — Core Backend Concepts

> These are the ideas that every backend engineer uses every day, regardless of language or framework.

| # | Topic | Tag |
|---|-------|-----|
| 2.1 | [The request/response lifecycle — what happens from browser to database and back](phases/phase-02-core-backend-concepts/2.01-request-response-lifecycle.md) | `[CORE]` ✅ |
| 2.2 | [Client-server architecture — what the server is responsible for](phases/phase-02-core-backend-concepts/2.02-client-server-architecture.md) | `[CORE]` ✅ |
| 2.3 | [Stateless vs. stateful servers — why this matters for scaling](phases/phase-02-core-backend-concepts/2.03-stateless-vs-stateful.md) | `[CORE]` ✅ |
| 2.4 | [Environment variables — configuration vs. code, 12-factor app](phases/phase-02-core-backend-concepts/2.04-environment-variables.md) | `[CORE]` ✅ |
| 2.5 | [Secrets management — never in code, never in git, always encrypted](phases/phase-02-core-backend-concepts/2.05-secrets-management.md) | `[CORE]` ✅ |
| 2.6 | [Input validation — trust nothing from users, validate at every boundary](phases/phase-02-core-backend-concepts/2.06-input-validation.md) | `[CORE]` ✅ |
| 2.7 | [Error handling strategies — error codes, exceptions, error objects, propagation](phases/phase-02-core-backend-concepts/2.07-error-handling.md) | `[CORE]` ✅ |
| 2.8 | [Logging basics — what to log, what not to log, structured logging](phases/phase-02-core-backend-concepts/2.08-logging.md) | `[CORE]` ✅ |
| 2.9 | [Request IDs and distributed tracing basics](phases/phase-02-core-backend-concepts/2.09-request-ids-tracing.md) | `[CORE]` ✅ |
| 2.10 | [Graceful shutdown — why your server must drain connections before dying](phases/phase-02-core-backend-concepts/2.10-graceful-shutdown.md) | `[CORE]` ✅ |
| 2.11 | [Health checks — liveness vs readiness probes](phases/phase-02-core-backend-concepts/2.11-health-checks.md) | `[CORE]` ✅ |
| 2.12 | [Backpressure — when your system receives more than it can handle](phases/phase-02-core-backend-concepts/2.12-backpressure.md) | `[ADVANCED]` ✅ |
| 2.13 | [Circuit breakers — stopping cascade failures](phases/phase-02-core-backend-concepts/2.13-circuit-breakers.md) | `[ADVANCED]` ✅ |
| 2.14 | [Retry logic — exponential backoff, jitter, when NOT to retry](phases/phase-02-core-backend-concepts/2.14-retry-logic.md) | `[ADVANCED]` ✅ |
| 2.15 | [Timeouts — connection timeout vs. read timeout, why defaults will kill you](phases/phase-02-core-backend-concepts/2.15-timeouts.md) | `[CORE]` ✅ |
| 2.16 | [Feature flags — deploying code before it's live](phases/phase-02-core-backend-concepts/2.16-feature-flags.md) | `[ADVANCED]` ✅ |
| 2.17 | [Rate limiting strategies — token bucket, sliding window, fixed window](phases/phase-02-core-backend-concepts/2.17-rate-limiting.md) | `[CORE]` ✅ |
| 2.18 | [Pagination — offset, cursor, keyset — performance differences](phases/phase-02-core-backend-concepts/2.18-pagination.md) | `[CORE]` ✅ |
| 2.19 | [API versioning — URL path, headers, query params — trade-offs](phases/phase-02-core-backend-concepts/2.19-api-versioning.md) | `[CORE]` ✅ |
| 2.20 | [Webhooks — push vs. pull, delivery guarantees, signature verification](phases/phase-02-core-backend-concepts/2.20-webhooks.md) | `[CORE]` ✅ |

---

## PHASE 3 — Languages & Runtimes

> You need to know one backend language deeply. You need to understand all the others exist and why.

| # | Topic | Tag |
|---|-------|-----|
| 3.1 | [**Python** — interpreted, GIL, asyncio, why it dominates data & APIs](phases/phase-03-languages-runtimes/3.01-python.md) | `[CORE]` ✅ |
| 3.2 | [Python internals — CPython, GIL deep dive, memory management](phases/phase-03-languages-runtimes/3.02-python-internals.md) | `[ADVANCED]` ✅ |
| 3.3 | [Python async/await — event loop, coroutines, tasks, asyncio internals](phases/phase-03-languages-runtimes/3.03-python-async.md) | `[CORE]` ✅ |
| 3.4 | [**Node.js** — V8, event loop, libuv, non-blocking I/O model](phases/phase-03-languages-runtimes/3.04-nodejs.md) | `[CORE]` ✅ |
| 3.5 | [Node.js internals — call stack, callback queue, microtask queue, event loop phases](phases/phase-03-languages-runtimes/3.05-nodejs-internals.md) | `[ADVANCED]` ✅ |
| 3.6 | [**Go (Golang)** — goroutines, channels, why it was built for servers](phases/phase-03-languages-runtimes/3.06-golang.md) | `[CORE]` ✅ |
| 3.7 | [Go internals — goroutine scheduler (M:N), garbage collector, escape analysis](phases/phase-03-languages-runtimes/3.07-golang-internals.md) | `[ADVANCED]` ✅ |
| 3.8 | [**Java** — JVM, JIT compilation, garbage collection, Spring ecosystem](phases/phase-03-languages-runtimes/3.08-java.md) | `[CORE]` ✅ |
| 3.9 | [**Rust** — ownership, borrowing, zero-cost abstractions, when to use it](phases/phase-03-languages-runtimes/3.09-rust.md) | `[ADVANCED]` ✅ |
| 3.10 | [**Ruby** — the language Rails made famous, concurrency model](phases/phase-03-languages-runtimes/3.10-ruby.md) | `[CORE]` ✅ |
| 3.11 | [**PHP** — the language that powers 70% of the web, modern PHP 8.x](phases/phase-03-languages-runtimes/3.11-php.md) | `[CORE]` ✅ |
| 3.12 | [**Elixir/Erlang** — BEAM VM, actor model, fault tolerance, why WhatsApp used it](phases/phase-03-languages-runtimes/3.12-elixir-erlang.md) | `[SPECIALIST]` ✅ |
| 3.13 | [**C#/.NET** — CLR, ASP.NET Core, enterprise use cases](phases/phase-03-languages-runtimes/3.13-csharp-dotnet.md) | `[CORE]` ✅ |
| 3.14 | [**Kotlin** — JVM language, Spring/Ktor backend use](phases/phase-03-languages-runtimes/3.14-kotlin.md) | `[ADVANCED]` ✅ |
| 3.15 | [Language selection framework — how to choose the right language for a system](phases/phase-03-languages-runtimes/3.15-language-selection.md) | `[CORE]` ✅ |
| 3.16 | [Runtimes explained — what a runtime is and why it matters](phases/phase-03-languages-runtimes/3.16-runtimes.md) | `[CORE]` ✅ |
| 3.17 | [Compiled vs. interpreted vs. JIT — real performance implications](phases/phase-03-languages-runtimes/3.17-compiled-interpreted-jit.md) | `[ADVANCED]` ✅ |
| 3.18 | [Memory management — manual (C/Rust), GC (Java/Go/Python), ownership (Rust)](phases/phase-03-languages-runtimes/3.18-memory-management.md) | `[ADVANCED]` ✅ |
| 3.19 | [Type systems — static vs. dynamic, strong vs. weak, structural vs. nominal](phases/phase-03-languages-runtimes/3.19-type-systems.md) | `[ADVANCED]` ✅ |

---

## PHASE 4 — Web Frameworks

> Frameworks are opinions about how to structure code. Know what opinions a framework has and why.

### Python Frameworks
| # | Topic | Tag |
|---|-------|-----|
| 4.1 | [**FastAPI** — async-first, OpenAPI auto-generation, dependency injection](phases/phase-04-web-frameworks/4.01-fastapi.md) | `[CORE]` ✅ |
| 4.2 | [**Django** — batteries-included, ORM, admin, when it's overkill](phases/phase-04-web-frameworks/4.02-django.md) | `[CORE]` ✅ |
| 4.3 | [**Flask** — minimalist, microframework, composable](phases/phase-04-web-frameworks/4.03-flask.md) | `[CORE]` ✅ |
| 4.4 | [**Starlette** — the ASGI foundation under FastAPI](phases/phase-04-web-frameworks/4.04-starlette.md) | `[ADVANCED]` ✅ |
| 4.5 | [**Litestar (Starlite)** — FastAPI alternative, more opinionated](phases/phase-04-web-frameworks/4.05-litestar.md) | `[ADVANCED]` ✅ |
| 4.6 | [**Tornado** — async Python before asyncio existed](phases/phase-04-web-frameworks/4.06-tornado.md) | `[SPECIALIST]` ✅ |

### Node.js Frameworks
| # | Topic | Tag |
|---|-------|-----|
| 4.7 | [**Express.js** — minimal, middleware-centric, the original Node framework](phases/phase-04-web-frameworks/4.07-expressjs.md) | `[CORE]` ✅ |
| 4.8 | [**Fastify** — faster than Express, JSON schema validation built-in](phases/phase-04-web-frameworks/4.08-fastify.md) | `[CORE]` ✅ |
| 4.9 | [**NestJS** — opinionated, Angular-inspired, TypeScript-first](phases/phase-04-web-frameworks/4.09-nestjs.md) | `[CORE]` ✅ |
| 4.10 | [**Hono** — ultra-fast, runs everywhere (Edge, Deno, Bun, Node)](phases/phase-04-web-frameworks/4.10-hono.md) | `[ADVANCED]` ✅ |
| 4.11 | [**Elysia** — Bun-native, type-safe, high performance](phases/phase-04-web-frameworks/4.11-elysia.md) | `[ADVANCED]` ✅ |

### Go Frameworks
| # | Topic | Tag |
|---|-------|-----|
| 4.12 | [**net/http** — Go's stdlib, often enough by itself](phases/phase-04-web-frameworks/4.12-go-net-http.md) | `[CORE]` ✅ |
| 4.13 | [**Gin** — fast HTTP framework, most popular in Go ecosystem](phases/phase-04-web-frameworks/4.13-gin.md) | `[CORE]` ✅ |
| 4.14 | [**Echo** — lightweight alternative to Gin](phases/phase-04-web-frameworks/4.14-echo.md) | `[CORE]` ✅ |
| 4.15 | [**Fiber** — Express-inspired, built on fasthttp](phases/phase-04-web-frameworks/4.14-echo.md) | `[ADVANCED]` ✅ |
| 4.16 | [**Chi** — lightweight, idiomatic, no magic](phases/phase-04-web-frameworks/4.14-echo.md) | `[ADVANCED]` ✅ |

### Java/Kotlin Frameworks
| # | Topic | Tag |
|---|-------|-----|
| 4.17 | [**Spring Boot** — the enterprise standard, dependency injection, auto-config](phases/phase-04-web-frameworks/4.17-spring-boot.md) | `[CORE]` ✅ |
| 4.18 | [**Quarkus** — GraalVM native, cloud-native Java](phases/phase-04-web-frameworks/4.18-quarkus.md) | `[ADVANCED]` ✅ |
| 4.19 | [**Micronaut** — ahead-of-time compiled, fast startup](phases/phase-04-web-frameworks/4.18-quarkus.md) | `[ADVANCED]` ✅ |
| 4.20 | [**Ktor** — Kotlin-native, coroutine-first](phases/phase-04-web-frameworks/4.18-quarkus.md) | `[ADVANCED]` ✅ |

### Other Frameworks
| # | Topic | Tag |
|---|-------|-----|
| 4.21 | [**Ruby on Rails** — the framework that defined MVC for the web](phases/phase-04-web-frameworks/4.21-rails.md) | `[CORE]` ✅ |
| 4.22 | [**Laravel** (PHP) — the dominant PHP framework](phases/phase-04-web-frameworks/4.22-laravel.md) | `[CORE]` ✅ |
| 4.23 | [**ASP.NET Core** (C#) — high-performance, cross-platform .NET](phases/phase-04-web-frameworks/4.22-laravel.md) | `[CORE]` ✅ |
| 4.24 | [**Axum** (Rust) — Tokio-based, ergonomic async Rust web framework](phases/phase-04-web-frameworks/4.22-laravel.md) | `[SPECIALIST]` ✅ |
| 4.25 | [Framework internals — middleware chains, routing trees, request lifecycle](phases/phase-04-web-frameworks/4.25-framework-internals.md) | `[ADVANCED]` ✅ |
| 4.26 | [WSGI vs. ASGI — Python server interfaces explained](phases/phase-04-web-frameworks/4.26-wsgi-asgi.md) | `[CORE]` ✅ |

---

## PHASE 5 — Databases

> Your database is the hardest part of your system to change. The decisions you make here last years.

### Relational Databases (SQL)
| # | Topic | Tag |
|---|-------|-----|
| 5.1 | Relational model — tables, rows, columns, relationships | `[CORE]` |
| 5.2 | SQL fundamentals — SELECT, INSERT, UPDATE, DELETE | `[CORE]` |
| 5.3 | SQL joins — INNER, LEFT, RIGHT, FULL, CROSS, SELF — with diagrams | `[CORE]` |
| 5.4 | Aggregations — GROUP BY, HAVING, window functions | `[CORE]` |
| 5.5 | Subqueries, CTEs (WITH), and when to use each | `[CORE]` |
| 5.6 | ACID properties — atomicity, consistency, isolation, durability | `[CORE]` |
| 5.7 | Transactions — BEGIN, COMMIT, ROLLBACK, savepoints | `[CORE]` |
| 5.8 | Isolation levels — read uncommitted to serializable, and their trade-offs | `[ADVANCED]` |
| 5.9 | Indexes — B-tree, hash, GIN, GiST, partial indexes | `[CORE]` |
| 5.10 | How indexes work internally — B-tree structure, pages, seeks | `[ADVANCED]` |
| 5.11 | EXPLAIN / EXPLAIN ANALYZE — reading query plans | `[CORE]` |
| 5.12 | Database normalization — 1NF, 2NF, 3NF, BCNF with real examples | `[CORE]` |
| 5.13 | Denormalization — when and why you break normalization rules intentionally | `[ADVANCED]` |
| 5.14 | Database design — primary keys, foreign keys, constraints, cascades | `[CORE]` |
| 5.15 | Sequences & auto-increment vs. UUIDs vs. ULIDs — the trade-offs | `[CORE]` |
| 5.16 | Schema migrations — versioned, reversible, zero-downtime strategies | `[CORE]` |
| 5.17 | Locking — row locks, table locks, deadlocks, advisory locks | `[ADVANCED]` |
| 5.18 | MVCC — multi-version concurrency control, how PostgreSQL avoids locks | `[ADVANCED]` |
| 5.19 | Stored procedures & triggers — when they help and when they're a trap | `[ADVANCED]` |
| 5.20 | Views & materialized views — computed vs. cached queries | `[ADVANCED]` |
| 5.21 | Connection pooling — PgBouncer, HikariCP, why raw connections are expensive | `[CORE]` |
| 5.22 | Replication — primary-replica, streaming replication, logical replication | `[ADVANCED]` |
| 5.23 | Read replicas — offloading read traffic, replication lag implications | `[ADVANCED]` |
| 5.24 | Partitioning — range, list, hash — when to partition and why | `[ADVANCED]` |
| 5.25 | Full-text search in PostgreSQL — tsvector, tsquery, ranking | `[ADVANCED]` |

### SQL Databases — Specific Systems
| # | Topic | Tag |
|---|-------|-----|
| 5.26 | **PostgreSQL** — the gold standard, JSONB, extensions, pg ecosystem | `[CORE]` |
| 5.27 | **MySQL / MariaDB** — InnoDB engine, differences from Postgres | `[CORE]` |
| 5.28 | **SQLite** — embedded, file-based, perfect for dev/edge/serverless | `[CORE]` |
| 5.29 | **CockroachDB** — distributed SQL, geo-partitioning, Postgres-compatible | `[SPECIALIST]` |
| 5.30 | **PlanetScale** — MySQL-compatible, branching model, no foreign keys trade-off | `[ADVANCED]` |
| 5.31 | **Neon** — serverless Postgres, branching, separation of storage and compute | `[ADVANCED]` |
| 5.32 | **TiDB** — distributed HTAP, MySQL-compatible | `[SPECIALIST]` |

### NoSQL Databases
| # | Topic | Tag |
|---|-------|-----|
| 5.33 | NoSQL philosophy — BASE properties, eventual consistency | `[CORE]` |
| 5.34 | **MongoDB** — document model, BSON, aggregation pipeline, indexes | `[CORE]` |
| 5.35 | **Redis** — data structures as a database, persistence options | `[CORE]` |
| 5.36 | Redis deep dive — strings, hashes, lists, sets, sorted sets, streams | `[CORE]` |
| 5.37 | Redis Cluster — sharding, slots, replication, failover | `[ADVANCED]` |
| 5.38 | **DynamoDB** — AWS's managed NoSQL, single-table design, GSIs | `[ADVANCED]` |
| 5.39 | **Cassandra** — wide-column, write-optimized, partition keys, consistency levels | `[ADVANCED]` |
| 5.40 | **Firestore / Firebase** — real-time sync, document model, offline support | `[CORE]` |
| 5.41 | **HBase** — Hadoop-native wide-column store | `[SPECIALIST]` |
| 5.42 | **Couchbase** — document + key-value + full-text, mobile sync | `[SPECIALIST]` |
| 5.43 | **Neo4j** — graph database, Cypher query language, relationship-first thinking | `[SPECIALIST]` |
| 5.44 | **InfluxDB** — time-series database, retention policies, Flux query language | `[SPECIALIST]` |
| 5.45 | **TimescaleDB** — time-series on top of PostgreSQL | `[SPECIALIST]` |

### ORMs & Query Builders
| # | Topic | Tag |
|---|-------|-----|
| 5.46 | ORM fundamentals — what they do, what they hide from you | `[CORE]` |
| 5.47 | **SQLAlchemy** (Python) — Core vs. ORM, session management | `[CORE]` |
| 5.48 | **Django ORM** — models, migrations, QuerySets, N+1 problem | `[CORE]` |
| 5.49 | **Prisma** (Node.js) — type-safe, code-first schema | `[CORE]` |
| 5.50 | **TypeORM** (Node.js) — decorator-based, Active Record vs. Data Mapper | `[CORE]` |
| 5.51 | **Drizzle ORM** (Node.js) — SQL-first, lightweight, TypeScript-native | `[ADVANCED]` |
| 5.52 | **GORM** (Go) — the standard Go ORM | `[CORE]` |
| 5.53 | **Hibernate** (Java) — JPA standard, lazy loading pitfalls | `[CORE]` |
| 5.54 | The N+1 query problem — what it is, how to detect it, how to fix it | `[CORE]` |
| 5.55 | Raw queries vs. ORM — when to break out of the abstraction | `[CORE]` |

---

## PHASE 6 — APIs & Communication Protocols

> The contract between your backend and everything else. Get this wrong and you'll be paying the technical debt forever.

### REST
| # | Topic | Tag |
|---|-------|-----|
| 6.1 | REST fundamentals — Roy Fielding's actual constraints (not what people think) | `[CORE]` |
| 6.2 | RESTful resource design — nouns, not verbs, nesting, relationships | `[CORE]` |
| 6.3 | HTTP methods semantics — GET, POST, PUT, PATCH, DELETE done right | `[CORE]` |
| 6.4 | REST API design best practices — naming, filtering, sorting, pagination | `[CORE]` |
| 6.5 | HATEOAS — hypermedia as the engine of application state | `[ADVANCED]` |
| 6.6 | OpenAPI / Swagger — API contracts, code generation, documentation | `[CORE]` |

### GraphQL
| # | Topic | Tag |
|---|-------|-----|
| 6.7 | GraphQL fundamentals — queries, mutations, subscriptions | `[CORE]` |
| 6.8 | GraphQL schema design — types, resolvers, schema-first vs. code-first | `[CORE]` |
| 6.9 | The N+1 problem in GraphQL — DataLoader pattern | `[ADVANCED]` |
| 6.10 | GraphQL vs. REST — when each wins, when each is the wrong choice | `[CORE]` |
| 6.11 | **Apollo Server / Apollo Federation** — microservices with GraphQL | `[ADVANCED]` |
| 6.12 | **Strawberry / Ariadne** (Python GraphQL) | `[ADVANCED]` |
| 6.13 | GraphQL persisted queries, query depth limiting, complexity analysis | `[ADVANCED]` |

### gRPC & Protocol Buffers
| # | Topic | Tag |
|---|-------|-----|
| 6.14 | Protocol Buffers — binary serialization, .proto files, field numbers | `[CORE]` |
| 6.15 | gRPC — HTTP/2-based RPC, four service types (unary, streaming) | `[CORE]` |
| 6.16 | gRPC vs. REST — latency, payload size, browser limitations | `[CORE]` |
| 6.17 | gRPC-web — using gRPC from browsers | `[ADVANCED]` |
| 6.18 | gRPC interceptors — the middleware equivalent | `[ADVANCED]` |
| 6.19 | **Buf** — modern toolchain for Protocol Buffers | `[ADVANCED]` |

### Real-Time Communication
| # | Topic | Tag |
|---|-------|-----|
| 6.20 | WebSockets — full-duplex, the handshake, frames, ping/pong | `[CORE]` |
| 6.21 | Server-Sent Events (SSE) — one-directional, HTTP-native streaming | `[CORE]` |
| 6.22 | Long polling vs. short polling vs. SSE vs. WebSockets — comparison | `[CORE]` |
| 6.23 | Socket.IO — abstraction over WebSockets, rooms, namespaces | `[ADVANCED]` |
| 6.24 | **WebRTC** — peer-to-peer media, STUN/TURN servers | `[SPECIALIST]` |

### Other Protocols & Patterns
| # | Topic | Tag |
|---|-------|-----|
| 6.25 | MQTT — IoT messaging protocol, publish/subscribe, QoS levels | `[SPECIALIST]` |
| 6.26 | AMQP — Advanced Message Queuing Protocol, used by RabbitMQ | `[ADVANCED]` |
| 6.27 | **tRPC** — end-to-end type safety without schemas (TypeScript) | `[ADVANCED]` |
| 6.28 | JSON-RPC — lightweight RPC using JSON | `[ADVANCED]` |
| 6.29 | Thrift — Facebook's binary serialization protocol | `[SPECIALIST]` |
| 6.30 | MessagePack — binary JSON alternative | `[SPECIALIST]` |

---

## PHASE 7 — Caching

> Caching is one of the two hard problems in computer science (along with naming things and off-by-one errors). It's also one of the highest-leverage performance tools you have.

| # | Topic | Tag |
|---|-------|-----|
| 7.1 | Caching fundamentals — why it works, locality of reference | `[CORE]` |
| 7.2 | Cache eviction policies — LRU, LFU, FIFO, TTL | `[CORE]` |
| 7.3 | Cache invalidation — the hardest problem, strategies | `[CORE]` |
| 7.4 | In-process / in-memory caching — the fastest cache | `[CORE]` |
| 7.5 | **Redis as a cache** — TTL, eviction policies, cache-aside pattern | `[CORE]` |
| 7.6 | **Memcached** — when to choose it over Redis | `[CORE]` |
| 7.7 | Cache-aside (lazy loading) pattern | `[CORE]` |
| 7.8 | Write-through cache pattern | `[ADVANCED]` |
| 7.9 | Write-behind (write-back) cache pattern | `[ADVANCED]` |
| 7.10 | Read-through cache pattern | `[ADVANCED]` |
| 7.11 | Cache stampede — the thundering herd problem and how to prevent it | `[ADVANCED]` |
| 7.12 | Cache warming — strategies for pre-populating caches | `[ADVANCED]` |
| 7.13 | Distributed cache consistency — the CAP trade-offs | `[ADVANCED]` |
| 7.14 | HTTP caching — Cache-Control, ETag, Last-Modified, Vary | `[CORE]` |
| 7.15 | CDN caching — edge nodes, cache-control for static vs. dynamic content | `[CORE]` |
| 7.16 | **Varnish** — dedicated HTTP caching proxy | `[SPECIALIST]` |
| 7.17 | Database query result caching — when it helps vs. when it masks problems | `[ADVANCED]` |
| 7.18 | Content-addressable storage — hash-based caching | `[SPECIALIST]` |
| 7.19 | Bloom filters — probabilistic data structure for cache miss reduction | `[SPECIALIST]` |

---

## PHASE 8 — Authentication & Security

> Security is not a feature you add later. It's a property of the system you design from the beginning.

### Authentication
| # | Topic | Tag |
|---|-------|-----|
| 8.1 | Authentication vs. Authorization — they are not the same thing | `[CORE]` |
| 8.2 | Password hashing — bcrypt, Argon2, scrypt — why MD5 will get you fired | `[CORE]` |
| 8.3 | Sessions — server-side session storage, cookies, session IDs | `[CORE]` |
| 8.4 | JWT (JSON Web Tokens) — structure, signing, verification, expiry | `[CORE]` |
| 8.5 | JWT pitfalls — the alg:none exploit, RS256 vs. HS256, short expiry requirement | `[CORE]` |
| 8.6 | OAuth 2.0 — flows (Authorization Code, Client Credentials, Device Flow) | `[CORE]` |
| 8.7 | OAuth 2.0 + PKCE — for mobile and SPAs | `[ADVANCED]` |
| 8.8 | OpenID Connect (OIDC) — identity layer on top of OAuth 2.0 | `[CORE]` |
| 8.9 | SAML — enterprise SSO, the XML nightmare | `[ADVANCED]` |
| 8.10 | API Keys — generation, storage, rotation, scoping | `[CORE]` |
| 8.11 | HMAC — signing requests with shared secrets (Stripe webhook pattern) | `[CORE]` |
| 8.12 | Multi-factor authentication (MFA/2FA) — TOTP, SMS, WebAuthn | `[ADVANCED]` |
| 8.13 | Passkeys & WebAuthn — the password-less future | `[ADVANCED]` |
| 8.14 | Token refresh flows — access token + refresh token pattern | `[CORE]` |
| 8.15 | **Auth0 / Clerk / Supabase Auth / Firebase Auth** — managed auth platforms | `[CORE]` |
| 8.16 | **Keycloak** — open-source identity provider | `[ADVANCED]` |

### Authorization
| # | Topic | Tag |
|---|-------|-----|
| 8.17 | RBAC — role-based access control, modeling roles and permissions | `[CORE]` |
| 8.18 | ABAC — attribute-based access control, policy-as-code | `[ADVANCED]` |
| 8.19 | ReBAC — relationship-based access control (Google Zanzibar model) | `[SPECIALIST]` |
| 8.20 | **OPA (Open Policy Agent)** — policy engine, Rego language | `[ADVANCED]` |
| 8.21 | Row-level security in PostgreSQL | `[ADVANCED]` |

### Security Fundamentals
| # | Topic | Tag |
|---|-------|-----|
| 8.22 | OWASP Top 10 — the list every backend engineer must memorize | `[CORE]` |
| 8.23 | SQL injection — how it works, how to prevent it, parameterized queries | `[CORE]` |
| 8.24 | XSS (Cross-Site Scripting) — stored, reflected, DOM-based | `[CORE]` |
| 8.25 | CSRF (Cross-Site Request Forgery) — tokens, SameSite cookies | `[CORE]` |
| 8.26 | SSRF (Server-Side Request Forgery) — attacking from the inside | `[ADVANCED]` |
| 8.27 | Command injection — OS command injection, shell escaping | `[CORE]` |
| 8.28 | Path traversal attacks | `[CORE]` |
| 8.29 | Insecure deserialization | `[ADVANCED]` |
| 8.30 | Security headers — CSP, HSTS, X-Frame-Options, referrer-policy | `[CORE]` |
| 8.31 | Rate limiting & brute force protection | `[CORE]` |
| 8.32 | DDoS attacks — types, mitigation strategies, Cloudflare/WAF | `[ADVANCED]` |
| 8.33 | Secrets in production — Vault, AWS Secrets Manager, sealed secrets | `[CORE]` |
| 8.34 | Dependency security — supply chain attacks, SBOMs, Dependabot | `[ADVANCED]` |
| 8.35 | Penetration testing basics — what to test, responsible disclosure | `[SPECIALIST]` |
| 8.36 | Zero-trust security model | `[SPECIALIST]` |

---

## PHASE 9 — Performance & Reliability

> Performance is a feature. Reliability is a promise. Both are engineered, not hoped for.

| # | Topic | Tag |
|---|-------|-----|
| 9.1 | Performance fundamentals — measuring before optimizing | `[CORE]` |
| 9.2 | Latency percentiles — p50, p95, p99, p999 — why averages lie | `[CORE]` |
| 9.3 | Little's Law — the relationship between throughput, latency, concurrency | `[ADVANCED]` |
| 9.4 | Profiling Python — cProfile, py-spy, memory_profiler | `[CORE]` |
| 9.5 | Profiling Node.js — clinic.js, --prof, heap snapshots | `[CORE]` |
| 9.6 | Profiling Go — pprof, trace, benchmarks | `[CORE]` |
| 9.7 | Database performance — slow query logs, pg_stat_statements | `[CORE]` |
| 9.8 | N+1 queries — detection, DataLoader pattern, eager loading | `[CORE]` |
| 9.9 | Connection pooling deep dive — PgBouncer, HikariCP, pool sizing formula | `[ADVANCED]` |
| 9.10 | Async I/O and why it matters — blocking vs. non-blocking under load | `[CORE]` |
| 9.11 | Thread pools — sizing, saturation, starvation | `[ADVANCED]` |
| 9.12 | Horizontal vs. vertical scaling — when each is appropriate | `[CORE]` |
| 9.13 | Load testing — k6, Locust, Gatling, JMeter — designing realistic tests | `[CORE]` |
| 9.14 | Chaos engineering — intentional failure, Netflix Chaos Monkey | `[ADVANCED]` |
| 9.15 | SLOs, SLAs, SLIs — defining and measuring reliability | `[ADVANCED]` |
| 9.16 | Error budgets — how reliability is traded against velocity | `[ADVANCED]` |
| 9.17 | Bulkhead pattern — isolating failures to prevent cascade | `[ADVANCED]` |
| 9.18 | Timeout + retry + fallback — the reliability triad | `[CORE]` |
| 9.19 | Blue/green deployment — zero-downtime releases | `[ADVANCED]` |
| 9.20 | Canary deployments — releasing to 1% of traffic first | `[ADVANCED]` |
| 9.21 | Database connection exhaustion — the silent killer | `[ADVANCED]` |
| 9.22 | Memory leaks — detection, heap dumps, common patterns | `[ADVANCED]` |
| 9.23 | CPU profiling in production — flame graphs | `[SPECIALIST]` |
| 9.24 | Goroutine/thread leaks | `[ADVANCED]` |

---

## PHASE 10 — Infrastructure & DevOps

> The code runs somewhere. Where it runs, how it runs, and how it gets there is not someone else's job.

### Containers
| # | Topic | Tag |
|---|-------|-----|
| 10.1 | **Docker** — images, containers, layers, the Dockerfile | `[CORE]` |
| 10.2 | Docker internals — namespaces, cgroups, union filesystems | `[ADVANCED]` |
| 10.3 | Writing production Dockerfiles — multi-stage builds, minimizing layers | `[CORE]` |
| 10.4 | Docker Compose — local multi-service development | `[CORE]` |
| 10.5 | Container registries — Docker Hub, ECR, GCR, GHCR | `[CORE]` |
| 10.6 | **Kubernetes (K8s)** — the container orchestration standard | `[ADVANCED]` |
| 10.7 | Kubernetes architecture — control plane, worker nodes, etcd | `[ADVANCED]` |
| 10.8 | Kubernetes objects — Pods, Deployments, Services, ConfigMaps, Secrets | `[ADVANCED]` |
| 10.9 | Kubernetes networking — Services, Ingress, NetworkPolicies | `[ADVANCED]` |
| 10.10 | Helm — the Kubernetes package manager | `[ADVANCED]` |
| 10.11 | **Podman** — Docker alternative, daemonless containers | `[SPECIALIST]` |

### CI/CD
| # | Topic | Tag |
|---|-------|-----|
| 10.12 | CI/CD fundamentals — the pipeline: lint, test, build, deploy | `[CORE]` |
| 10.13 | **GitHub Actions** — workflows, jobs, steps, marketplace actions | `[CORE]` |
| 10.14 | **GitLab CI** — .gitlab-ci.yml, runners, artifacts | `[CORE]` |
| 10.15 | **Jenkins** — the original CI, declarative pipelines, plugins | `[ADVANCED]` |
| 10.16 | **CircleCI / Buildkite / Travis CI** | `[ADVANCED]` |
| 10.17 | Deployment strategies — recreate, rolling, blue-green, canary | `[CORE]` |
| 10.18 | Infrastructure as Code (IaC) — why you must never click in a console | `[CORE]` |

### Infrastructure as Code
| # | Topic | Tag |
|---|-------|-----|
| 10.19 | **Terraform** — declarative IaC, providers, state management | `[CORE]` |
| 10.20 | **Pulumi** — IaC with real programming languages | `[ADVANCED]` |
| 10.21 | **Ansible** — configuration management, idempotent playbooks | `[ADVANCED]` |
| 10.22 | **Chef / Puppet** — configuration management at enterprise scale | `[SPECIALIST]` |

### Web Servers & Reverse Proxies
| # | Topic | Tag |
|---|-------|-----|
| 10.23 | **Nginx** — the most deployed web server, config deep dive | `[CORE]` |
| 10.24 | **Caddy** — automatic HTTPS, modern Nginx alternative | `[ADVANCED]` |
| 10.25 | **Traefik** — cloud-native reverse proxy, Docker/K8s-native | `[ADVANCED]` |
| 10.26 | **HAProxy** — the high-performance load balancer | `[ADVANCED]` |
| 10.27 | Process managers — Supervisor, systemd, PM2 | `[CORE]` |

---

## PHASE 11 — Cloud Platforms & Serverless

> The cloud is not magic. It is other people's computers with very good billing infrastructure.

### AWS (Amazon Web Services)
| # | Topic | Tag |
|---|-------|-----|
| 11.1 | AWS fundamentals — regions, AZs, the global infrastructure | `[CORE]` |
| 11.2 | **EC2** — virtual machines, instance types, spot vs. on-demand | `[CORE]` |
| 11.3 | **S3** — object storage, the backbone of the internet | `[CORE]` |
| 11.4 | **RDS** — managed relational databases (Postgres, MySQL, Aurora) | `[CORE]` |
| 11.5 | **Aurora** — AWS's high-performance MySQL/Postgres-compatible DB | `[ADVANCED]` |
| 11.6 | **DynamoDB** — managed NoSQL, single-table design patterns | `[ADVANCED]` |
| 11.7 | **ElastiCache** — managed Redis/Memcached | `[CORE]` |
| 11.8 | **Lambda** — serverless functions, cold starts, execution limits | `[CORE]` |
| 11.9 | **API Gateway** — managed HTTP/WebSocket APIs in front of Lambda | `[CORE]` |
| 11.10 | **SQS** — simple queue service, visibility timeout, DLQ | `[CORE]` |
| 11.11 | **SNS** — pub/sub, fan-out to SQS, email, SMS | `[CORE]` |
| 11.12 | **ECS / EKS** — containers on AWS (Fargate vs. EC2-backed) | `[ADVANCED]` |
| 11.13 | **CloudFront** — AWS CDN | `[CORE]` |
| 11.14 | **VPC** — virtual private cloud, subnets, routing, security groups | `[ADVANCED]` |
| 11.15 | **IAM** — identity and access management, least-privilege principle | `[CORE]` |
| 11.16 | **Secrets Manager / SSM Parameter Store** | `[CORE]` |
| 11.17 | **CloudWatch** — metrics, logs, alarms, dashboards | `[CORE]` |
| 11.18 | **Route 53** — DNS management, health checks, routing policies | `[ADVANCED]` |
| 11.19 | **Kinesis** — real-time data streaming | `[SPECIALIST]` |
| 11.20 | **Step Functions** — serverless workflow orchestration | `[ADVANCED]` |

### GCP (Google Cloud Platform)
| # | Topic | Tag |
|---|-------|-----|
| 11.21 | **Cloud Run** — serverless containers (the best of both worlds) | `[CORE]` |
| 11.22 | **GKE** — managed Kubernetes | `[ADVANCED]` |
| 11.23 | **Cloud SQL** — managed Postgres/MySQL | `[CORE]` |
| 11.24 | **Firestore** — managed document DB | `[CORE]` |
| 11.25 | **BigQuery** — serverless analytics at scale | `[SPECIALIST]` |
| 11.26 | **Pub/Sub** — managed message queue | `[CORE]` |
| 11.27 | **Cloud Storage (GCS)** — object storage | `[CORE]` |

### Azure
| # | Topic | Tag |
|---|-------|-----|
| 11.28 | **Azure Functions** — serverless compute | `[CORE]` |
| 11.29 | **Azure Cosmos DB** — globally distributed NoSQL | `[ADVANCED]` |
| 11.30 | **Azure Service Bus** — enterprise messaging | `[ADVANCED]` |
| 11.31 | **AKS** — managed Kubernetes | `[ADVANCED]` |

### Serverless & Edge
| # | Topic | Tag |
|---|-------|-----|
| 11.32 | Serverless fundamentals — functions, cold starts, stateless constraints | `[CORE]` |
| 11.33 | Cold start problem — causes, mitigation, provisioned concurrency | `[ADVANCED]` |
| 11.34 | **Vercel / Netlify** — frontend-focused, edge functions | `[CORE]` |
| 11.35 | **Cloudflare Workers** — edge compute at 300+ PoPs, V8 isolates | `[ADVANCED]` |
| 11.36 | **Cloudflare D1 / KV / R2 / Durable Objects** — edge data primitives | `[ADVANCED]` |
| 11.37 | **Fly.io** — deploy containers globally, close to users | `[ADVANCED]` |
| 11.38 | **Railway / Render** — simpler deployment platforms | `[CORE]` |
| 11.39 | Edge computing vs. serverless vs. containers — the trade-off matrix | `[ADVANCED]` |
| 11.40 | Cost modeling cloud architectures — avoiding bill shock | `[ADVANCED]` |

---

## PHASE 12 — Messaging & Event-Driven Systems

> The moment you have two services that need to talk, you have a distributed systems problem. Messaging is how you solve it.

| # | Topic | Tag |
|---|-------|-----|
| 12.1 | Why messaging? — decoupling, resilience, async processing | `[CORE]` |
| 12.2 | Message queues vs. event streams — the fundamental difference | `[CORE]` |
| 12.3 | At-most-once vs. at-least-once vs. exactly-once delivery | `[CORE]` |
| 12.4 | Dead letter queues (DLQ) — handling poison messages | `[CORE]` |
| 12.5 | **RabbitMQ** — exchanges, queues, bindings, routing keys | `[CORE]` |
| 12.6 | RabbitMQ exchange types — direct, topic, fanout, headers | `[ADVANCED]` |
| 12.7 | **Apache Kafka** — partitions, topics, offsets, consumer groups | `[ADVANCED]` |
| 12.8 | Kafka internals — log-based storage, retention, compaction | `[ADVANCED]` |
| 12.9 | Kafka consumers — rebalancing, partition assignment, lag monitoring | `[ADVANCED]` |
| 12.10 | **Kafka Connect** — data pipelines, source/sink connectors | `[SPECIALIST]` |
| 12.11 | **Kafka Streams** — stream processing without a separate system | `[SPECIALIST]` |
| 12.12 | **Apache Pulsar** — Kafka alternative, multi-tenancy, tiered storage | `[SPECIALIST]` |
| 12.13 | **NATS** — lightweight, cloud-native messaging | `[ADVANCED]` |
| 12.14 | **AWS SQS + SNS** — managed queue + pub/sub | `[CORE]` |
| 12.15 | **Google Pub/Sub** — managed streaming | `[CORE]` |
| 12.16 | **Azure Service Bus / Event Hub** | `[ADVANCED]` |
| 12.17 | Event-driven architecture (EDA) — events, commands, queries | `[ADVANCED]` |
| 12.18 | CQRS — Command Query Responsibility Segregation | `[ADVANCED]` |
| 12.19 | Event sourcing — storing state as a sequence of events | `[ADVANCED]` |
| 12.20 | Outbox pattern — reliable event publishing with transactions | `[ADVANCED]` |
| 12.21 | Saga pattern — distributed transactions without 2PC | `[ADVANCED]` |
| 12.22 | Choreography vs. orchestration in sagas | `[ADVANCED]` |
| 12.23 | Background jobs & task queues — Celery, BullMQ, Sidekiq, Faktory | `[CORE]` |
| 12.24 | **Celery** (Python) — distributed task queue, workers, beat scheduler | `[CORE]` |
| 12.25 | **BullMQ** (Node.js) — Redis-backed job queue | `[CORE]` |
| 12.26 | **Sidekiq** (Ruby) — background processing | `[CORE]` |
| 12.27 | **Temporal** — durable workflow execution engine | `[SPECIALIST]` |
| 12.28 | **Inngest** — serverless queues and workflows | `[ADVANCED]` |

---

## PHASE 13 — Search & Analytics

> When your database queries become full-text searches, you need dedicated tools. When your data becomes too big for OLTP, you need OLAP.

| # | Topic | Tag |
|---|-------|-----|
| 13.1 | Full-text search fundamentals — tokenization, stemming, inverted index | `[CORE]` |
| 13.2 | **Elasticsearch** — distributed, RESTful search and analytics | `[CORE]` |
| 13.3 | Elasticsearch internals — shards, replicas, segments, lucene | `[ADVANCED]` |
| 13.4 | Elasticsearch query DSL — bool, match, term, range, aggregations | `[ADVANCED]` |
| 13.5 | **OpenSearch** — AWS's open-source Elasticsearch fork | `[ADVANCED]` |
| 13.6 | **Apache Solr** — the original enterprise search | `[SPECIALIST]` |
| 13.7 | **Typesense** — open-source, typo-tolerant search | `[ADVANCED]` |
| 13.8 | **Meilisearch** — open-source, developer-friendly search | `[ADVANCED]` |
| 13.9 | **Algolia** — managed search-as-a-service | `[CORE]` |
| 13.10 | Vector databases — semantic search, embeddings, ANN algorithms | `[ADVANCED]` |
| 13.11 | **pgvector** — vector search in PostgreSQL | `[ADVANCED]` |
| 13.12 | **Pinecone / Weaviate / Qdrant / Milvus** — dedicated vector databases | `[ADVANCED]` |
| 13.13 | OLTP vs. OLAP — transactional vs. analytical workloads | `[CORE]` |
| 13.14 | **ClickHouse** — columnar OLAP at high speed | `[SPECIALIST]` |
| 13.15 | **Apache Druid** — real-time analytics for event data | `[SPECIALIST]` |
| 13.16 | **BigQuery** — serverless analytics warehouse | `[SPECIALIST]` |
| 13.17 | **Snowflake** — cloud data warehouse | `[SPECIALIST]` |
| 13.18 | **Redshift** — AWS data warehouse | `[SPECIALIST]` |
| 13.19 | Data warehouses vs. data lakes vs. data lakehouses | `[SPECIALIST]` |
| 13.20 | **Apache Iceberg / Delta Lake / Hudi** — open table formats | `[SPECIALIST]` |

---

## PHASE 14 — Distributed Systems & Microservices

> Distributed systems are hard. Anyone who tells you otherwise is selling something. Learn why they're hard before you decide to build one.

### Distributed Systems Theory
| # | Topic | Tag |
|---|-------|-----|
| 14.1 | Why distributed systems are hard — 8 fallacies, partial failures | `[CORE]` |
| 14.2 | CAP theorem — consistency, availability, partition tolerance | `[CORE]` |
| 14.3 | PACELC theorem — extending CAP with latency | `[ADVANCED]` |
| 14.4 | Consistency models — eventual, strong, causal, read-your-writes | `[ADVANCED]` |
| 14.5 | Consensus algorithms — Paxos, Raft — how distributed agreement works | `[SPECIALIST]` |
| 14.6 | Vector clocks and logical time | `[SPECIALIST]` |
| 14.7 | Two-phase commit (2PC) — why it's fragile | `[ADVANCED]` |
| 14.8 | Distributed transactions — sagas, TCC, best-effort | `[ADVANCED]` |

### Microservices
| # | Topic | Tag |
|---|-------|-----|
| 14.9 | Monolith vs. microservices — the actual trade-offs | `[CORE]` |
| 14.10 | The modular monolith — the underrated option | `[ADVANCED]` |
| 14.11 | Service decomposition strategies — domain-driven design, bounded contexts | `[ADVANCED]` |
| 14.12 | Inter-service communication — synchronous (REST/gRPC) vs. async (events) | `[CORE]` |
| 14.13 | Service discovery — client-side vs. server-side, Consul, etcd | `[ADVANCED]` |
| 14.14 | API Gateway pattern — single entry point, routing, auth | `[ADVANCED]` |
| 14.15 | BFF (Backend For Frontend) pattern | `[ADVANCED]` |
| 14.16 | Circuit breakers in microservices — Hystrix, Resilience4j | `[ADVANCED]` |
| 14.17 | Distributed tracing — OpenTelemetry, Jaeger, Zipkin, correlation IDs | `[ADVANCED]` |
| 14.18 | The sidecar pattern — Envoy, Istio | `[SPECIALIST]` |
| 14.19 | Service mesh — Istio, Linkerd, Consul Connect | `[SPECIALIST]` |
| 14.20 | Conway's Law — your architecture will mirror your org structure | `[CORE]` |
| 14.21 | When NOT to use microservices | `[CORE]` |

### Data Patterns in Distributed Systems
| # | Topic | Tag |
|---|-------|-----|
| 14.22 | Database-per-service pattern | `[ADVANCED]` |
| 14.23 | Shared database anti-pattern | `[ADVANCED]` |
| 14.24 | Event-driven data synchronization across services | `[ADVANCED]` |
| 14.25 | Distributed caching patterns | `[ADVANCED]` |
| 14.26 | Global ID generation — Snowflake IDs, ULID, Twitter's Snowflake | `[ADVANCED]` |

---

## PHASE 15 — Advanced Architecture Patterns

> Patterns are solutions to recurring problems. Learn the name, learn when the problem occurs, and never build the wrong thing twice.

| # | Topic | Tag |
|---|-------|-----|
| 15.1 | Domain-Driven Design (DDD) — ubiquitous language, bounded contexts | `[ADVANCED]` |
| 15.2 | Hexagonal architecture (Ports & Adapters) | `[ADVANCED]` |
| 15.3 | Clean architecture — independence from frameworks, databases, UI | `[ADVANCED]` |
| 15.4 | Repository pattern — abstracting data access | `[ADVANCED]` |
| 15.5 | Unit of Work pattern | `[ADVANCED]` |
| 15.6 | CQRS — separating read and write models | `[ADVANCED]` |
| 15.7 | Event sourcing — the complete guide | `[ADVANCED]` |
| 15.8 | Strangler fig pattern — migrating monoliths | `[ADVANCED]` |
| 15.9 | Sidecar pattern — co-located helper processes | `[SPECIALIST]` |
| 15.10 | Anti-corruption layer — protecting your domain from external models | `[ADVANCED]` |
| 15.11 | Shared kernel — what two bounded contexts can share | `[ADVANCED]` |
| 15.12 | Twelve-factor app methodology — the cloud-native standards | `[CORE]` |
| 15.13 | Multi-tenancy architectures — silo, pool, hybrid | `[ADVANCED]` |
| 15.14 | Geo-distribution — data residency, latency routing, replication | `[SPECIALIST]` |
| 15.15 | Database sharding — horizontal partitioning strategies | `[ADVANCED]` |
| 15.16 | Consistent hashing — the algorithm behind distributed caches | `[ADVANCED]` |
| 15.17 | Idempotent APIs and at-least-once delivery | `[ADVANCED]` |
| 15.18 | The Outbox pattern — guaranteed event publishing | `[ADVANCED]` |
| 15.19 | Change Data Capture (CDC) — Debezium, replication slots | `[SPECIALIST]` |
| 15.20 | Read-through architecture with write-behind | `[SPECIALIST]` |

---

## PHASE 16 — Data Engineering & Pipelines

> Backends don't just serve data — they process it, transform it, and move it. This is the plumbing of the data world.

| # | Topic | Tag |
|---|-------|-----|
| 16.1 | ETL vs. ELT — extract-transform-load vs. extract-load-transform | `[ADVANCED]` |
| 16.2 | Batch processing vs. stream processing | `[ADVANCED]` |
| 16.3 | **Apache Spark** — distributed batch processing | `[SPECIALIST]` |
| 16.4 | **Apache Flink** — stateful stream processing | `[SPECIALIST]` |
| 16.5 | **Apache Beam** — unified batch + streaming model | `[SPECIALIST]` |
| 16.6 | **dbt** — data build tool, SQL-based transformations | `[SPECIALIST]` |
| 16.7 | **Airbyte** — open-source data integration | `[SPECIALIST]` |
| 16.8 | **Fivetran** — managed data pipelines | `[SPECIALIST]` |
| 16.9 | Data lakes — storing raw data at scale | `[SPECIALIST]` |
| 16.10 | **Apache Hadoop** — the original distributed data processing | `[SPECIALIST]` |
| 16.11 | **Apache Hive** — SQL on Hadoop | `[SPECIALIST]` |
| 16.12 | **Prefect / Apache Airflow / Dagster** — workflow orchestration | `[SPECIALIST]` |
| 16.13 | Schema evolution — handling changing data structures over time | `[ADVANCED]` |
| 16.14 | **Apache Avro** — schema-based serialization, schema registry | `[SPECIALIST]` |
| 16.15 | **Parquet / ORC** — columnar file formats | `[SPECIALIST]` |

---

## PHASE 17 — AI/ML Backend Integration

> The backend engineer's role has expanded to building infrastructure that serves, orchestrates, and enhances AI systems.

| # | Topic | Tag |
|---|-------|-----|
| 17.1 | Serving ML models — REST API wrappers, latency, batching | `[ADVANCED]` |
| 17.2 | **ONNX** — open neural network exchange format | `[SPECIALIST]` |
| 17.3 | **TensorFlow Serving / TorchServe** — production ML model servers | `[SPECIALIST]` |
| 17.4 | **Triton Inference Server** (NVIDIA) — GPU inference at scale | `[SPECIALIST]` |
| 17.5 | LLM APIs — integrating OpenAI, Anthropic, Gemini, Cohere APIs | `[ADVANCED]` |
| 17.6 | LLM inference infrastructure — vLLM, Ollama, llama.cpp | `[ADVANCED]` |
| 17.7 | RAG (Retrieval Augmented Generation) backends | `[ADVANCED]` |
| 17.8 | Vector search pipelines — embedding, indexing, querying | `[ADVANCED]` |
| 17.9 | **LangChain / LlamaIndex** — LLM application frameworks | `[ADVANCED]` |
| 17.10 | Prompt caching and token optimization in LLM backends | `[ADVANCED]` |
| 17.11 | AI agent backends — tool calling, orchestration, memory | `[ADVANCED]` |
| 17.12 | Feature stores — **Feast, Tecton, Hopsworks** | `[SPECIALIST]` |
| 17.13 | Model registries — **MLflow, DVC, Weights & Biases** | `[SPECIALIST]` |
| 17.14 | **BentoML / Ray Serve** — ML model serving frameworks | `[SPECIALIST]` |
| 17.15 | GPU infrastructure for AI — CUDA basics, multi-GPU, distributed training | `[SPECIALIST]` |
| 17.16 | Streaming LLM responses — server-sent events + LLM | `[ADVANCED]` |

---

## PHASE 18 — Observability & SRE

> You cannot fix what you cannot see. Observability is not monitoring — it's the ability to ask new questions about your system without deploying new code.

| # | Topic | Tag |
|---|-------|-----|
| 18.1 | The three pillars of observability — logs, metrics, traces | `[CORE]` |
| 18.2 | Structured logging — JSON logs, log levels, what to include | `[CORE]` |
| 18.3 | **Elasticsearch + Kibana (ELK Stack)** — log aggregation and visualization | `[CORE]` |
| 18.4 | **Grafana Loki** — log aggregation, cheaper ELK alternative | `[ADVANCED]` |
| 18.5 | Metrics fundamentals — counters, gauges, histograms, summaries | `[CORE]` |
| 18.6 | **Prometheus** — pull-based metrics, PromQL, alerting rules | `[CORE]` |
| 18.7 | **Grafana** — dashboards, alerting, visualization | `[CORE]` |
| 18.8 | **Datadog** — all-in-one APM, logs, metrics | `[ADVANCED]` |
| 18.9 | **New Relic / Dynatrace** — enterprise APM | `[ADVANCED]` |
| 18.10 | Distributed tracing — OpenTelemetry, trace context propagation | `[ADVANCED]` |
| 18.11 | **Jaeger / Tempo / Zipkin** — distributed tracing backends | `[ADVANCED]` |
| 18.12 | **OpenTelemetry** — the standard for telemetry data | `[ADVANCED]` |
| 18.13 | **Sentry** — error tracking, performance monitoring | `[CORE]` |
| 18.14 | SLO/SLA/SLI — defining, measuring, alerting on reliability | `[ADVANCED]` |
| 18.15 | Error budgets and toil reduction | `[ADVANCED]` |
| 18.16 | On-call engineering — PagerDuty, incident response, post-mortems | `[ADVANCED]` |
| 18.17 | **PagerDuty / OpsGenie** — on-call alerting platforms | `[ADVANCED]` |
| 18.18 | Runbooks — documenting how to respond to incidents | `[ADVANCED]` |
| 18.19 | **Uptime Kuma / Checkly** — synthetic monitoring | `[ADVANCED]` |
| 18.20 | eBPF — low-level observability without code changes | `[SPECIALIST]` |

---

## PHASE 19 — Testing & Quality

> Tests are not about catching bugs — they're about designing systems that are correct by construction.

| # | Topic | Tag |
|---|-------|-----|
| 19.1 | Testing philosophy — what to test, what not to test | `[CORE]` |
| 19.2 | The testing pyramid — unit, integration, end-to-end | `[CORE]` |
| 19.3 | Unit testing — isolated, fast, deterministic | `[CORE]` |
| 19.4 | Integration testing — testing with real databases and services | `[CORE]` |
| 19.5 | Contract testing — **Pact**, consumer-driven contracts | `[ADVANCED]` |
| 19.6 | End-to-end testing — tools, cost, flakiness | `[CORE]` |
| 19.7 | **pytest** (Python) — fixtures, parameterization, plugins | `[CORE]` |
| 19.8 | **Jest / Vitest** (Node.js) — modern test runners | `[CORE]` |
| 19.9 | **Go testing** — stdlib testing package, table-driven tests | `[CORE]` |
| 19.10 | Mocking strategies — mocks vs. stubs vs. fakes vs. spies | `[CORE]` |
| 19.11 | Test containers — running real databases in tests | `[ADVANCED]` |
| 19.12 | Property-based testing — **Hypothesis** (Python), **fast-check** (JS) | `[ADVANCED]` |
| 19.13 | Mutation testing — are your tests actually testing anything? | `[SPECIALIST]` |
| 19.14 | Performance testing — k6, Locust, JMeter | `[CORE]` |
| 19.15 | API testing — Postman, Bruno, Hoppscotch | `[CORE]` |
| 19.16 | Chaos testing — intentional failure injection | `[ADVANCED]` |
| 19.17 | Security testing — SAST, DAST, dependency scanning | `[ADVANCED]` |
| 19.18 | Code coverage — what it tells you and what it doesn't | `[CORE]` |
| 19.19 | Test data management — factories, fixtures, seeding | `[ADVANCED]` |

---

## PHASE 20 — Career & System Design Interviews

> Your ability to navigate complex system design decisions is what separates mid-level engineers from senior engineers. And senior engineers from principals.

| # | Topic | Tag |
|---|-------|-----|
| 20.1 | How to approach a system design interview — the framework | `[CORE]` |
| 20.2 | Capacity estimation — back-of-envelope math every engineer must know | `[CORE]` |
| 20.3 | Design a URL shortener (Tiny URL) | `[CORE]` |
| 20.4 | Design a rate limiter | `[CORE]` |
| 20.5 | Design a notification system | `[CORE]` |
| 20.6 | Design a news feed (Twitter/Instagram) | `[CORE]` |
| 20.7 | Design a chat system (WhatsApp/Slack) | `[CORE]` |
| 20.8 | Design a distributed key-value store | `[ADVANCED]` |
| 20.9 | Design a search autocomplete system | `[ADVANCED]` |
| 20.10 | Design YouTube / video streaming | `[ADVANCED]` |
| 20.11 | Design Uber / ride sharing | `[ADVANCED]` |
| 20.12 | Design a distributed job scheduler | `[ADVANCED]` |
| 20.13 | Design an e-commerce checkout system | `[ADVANCED]` |
| 20.14 | Design a payment system | `[ADVANCED]` |
| 20.15 | Design an API gateway | `[ADVANCED]` |
| 20.16 | Design a CDN | `[SPECIALIST]` |
| 20.17 | Design Google Drive / Dropbox | `[SPECIALIST]` |
| 20.18 | Design a web crawler | `[SPECIALIST]` |
| 20.19 | Design Airbnb / hotel booking | `[SPECIALIST]` |
| 20.20 | The staff/principal engineer mindset — thinking at system scale | `[ADVANCED]` |

---

## QUICK REFERENCE: Technology Ecosystem Map

```
                     ┌─────────────────────────────────┐
                     │         CLIENT REQUEST           │
                     └────────────────┬────────────────┘
                                      │
                     ┌────────────────▼────────────────┐
                     │     DNS Resolution (1.4)         │
                     └────────────────┬────────────────┘
                                      │
                     ┌────────────────▼────────────────┐
                     │     CDN / Edge (1.16, 11.35)     │
                     └────────────────┬────────────────┘
                                      │
                     ┌────────────────▼────────────────┐
                     │  Load Balancer (1.18, 10.26)     │
                     └────────────────┬────────────────┘
                                      │
                     ┌────────────────▼────────────────┐
                     │  Reverse Proxy / API Gateway     │
                     │  Nginx / Caddy / Traefik (10.23) │
                     └────────────────┬────────────────┘
                                      │
                     ┌────────────────▼────────────────┐
                     │   Web Framework (Phase 4)        │
                     │  FastAPI / Express / Gin          │
                     └────┬───────────┬────────────────┘
                          │           │
           ┌──────────────▼──┐   ┌───▼──────────────────┐
           │  Auth (Phase 8) │   │  Cache (Phase 7)      │
           │  JWT / OAuth2   │   │  Redis / Memcached    │
           └─────────────────┘   └──────────────────────┘
                          │
           ┌──────────────▼──────────────────────────────┐
           │         Database (Phase 5)                   │
           │  PostgreSQL / MongoDB / Redis                │
           └──────────────┬──────────────────────────────┘
                          │
           ┌──────────────▼──────────────────────────────┐
           │    Message Queue (Phase 12)                  │
           │    Kafka / RabbitMQ / SQS                    │
           └──────────────┬──────────────────────────────┘
                          │
           ┌──────────────▼──────────────────────────────┐
           │    Background Workers (12.23)                │
           │    Celery / BullMQ / Sidekiq                 │
           └──────────────┬──────────────────────────────┘
                          │
           ┌──────────────▼──────────────────────────────┐
           │    Observability (Phase 18)                  │
           │    Prometheus + Grafana + OpenTelemetry      │
           └─────────────────────────────────────────────┘
```

---

## LEARNING PATH RECOMMENDATIONS

### The "Get Hired" Path (3-6 months)
```
Phase 0 → Phase 1 (1.1–1.15) → Phase 2 → Phase 3 (pick one language) →
Phase 4 (one framework) → Phase 5 (5.1–5.25, 5.26/5.27, 5.46–5.55) →
Phase 6 (6.1–6.13) → Phase 7 (7.1–7.9) → Phase 8 (8.1–8.24) →
Phase 10 (10.1–10.17) → Phase 20 (20.1–20.10)
```

### The "Senior Engineer" Path (6-12 months from hired)
```
Phase 9 → Phase 11 → Phase 12 (12.1–12.25) → Phase 14 →
Phase 15 → Phase 18 → Phase 19 → Phase 20 (all)
```

### The "Architect / Principal" Path (ongoing)
```
Phase 14 (all) → Phase 15 (all) → Phase 16 → Phase 17 →
Phase 12 (all) → System Design from Phase 20 →
Real-world reading: engineering blogs from Stripe, Cloudflare, Discord, Uber, Netflix
```

---

## ENGINEERING BLOGS WORTH READING

| Company | Best For |
|---------|----------|
| Stripe Engineering | Payments, API design, reliability |
| Cloudflare Blog | Networking, edge computing, security |
| Discord Engineering | Real-time systems, NoSQL at scale |
| Uber Engineering | Distributed systems, databases |
| Netflix Tech Blog | Resilience, data at scale, streaming |
| Shopify Engineering | Ruby/Rails at scale, e-commerce |
| Figma Engineering | WebSockets, collaborative systems |
| Notion Engineering | Database sharding, PostgreSQL |
| PlanetScale Blog | Database internals, MySQL |
| Martin Fowler's Blog | Architecture patterns, DDD |
| High Scalability | System design case studies |

---

## HOW TO NAVIGATE THIS BIBLE

```
To learn a topic:       "teach me [topic number or name]"
To go deeper:           "go deeper on [aspect of the topic]"
To compare tools:       "compare PostgreSQL vs MongoDB"
To see a real example:  "give me a real example of circuit breakers"
To find your next step: "what should I learn next?"
To test your knowledge: switch to /teach-backend:test
```

> **Remember:** You will not learn backend engineering by reading this list.
> You will learn it by building things, breaking things, debugging things at
> 2am, and slowly developing the intuition that only comes from shipping
> systems that real people use.
>
> This roadmap is the map. You still have to walk the territory.

---

*Last updated: June 2026 | 20 Phases | 350+ Topics | Complete Backend Ecosystem Coverage*
