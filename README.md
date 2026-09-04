---
title: "Backend Developer Roadmap"
description: "A practical, modern backend development roadmap covering programming, networking, databases, APIs, security, testing, DevOps, architecture, scalability, and system design."
---

# Backend Developer Roadmap

> A practical learning path for becoming a production-ready backend developer in 2026.
>
> Based on the topic areas covered by the [roadmap.sh Backend Developer roadmap](https://roadmap.sh/backend).

## How to use this roadmap

- [ ] Learn the fundamentals before jumping into frameworks.
- [ ] Pick **one** backend language and go deep.
- [ ] Build projects after each major section.
- [ ] Prefer understanding concepts over memorizing tools.
- [ ] Use PostgreSQL as your primary relational database.
- [ ] Learn deployment, observability, security, and scalability after you can build a complete API.

---

# 1. Pick a Backend Language

Choose one primary language.

### Recommended options

- [ ] Rust
- [ ] TypeScript / JavaScript
- [ ] Go
- [ ] Java
- [ ] C#
- [ ] Python
- [ ] PHP
- [ ] Ruby

### If choosing Rust

- [ ] Variables and mutability
- [ ] Primitive and compound types
- [ ] Functions
- [ ] Ownership
- [ ] Borrowing
- [ ] References
- [ ] Slices
- [ ] Structs
- [ ] Enums
- [ ] Pattern matching
- [ ] `Option`
- [ ] `Result`
- [ ] Traits
- [ ] Generics
- [ ] Lifetimes
- [ ] Error handling
- [ ] Iterators
- [ ] Closures
- [ ] Modules and crates
- [ ] Cargo
- [ ] Async/await
- [ ] Tokio
- [ ] Concurrency
- [ ] `Arc`
- [ ] `Mutex`
- [ ] Channels

### Rust Backend Stack

- [ ] Actix Web or Axum
- [ ] SQLx
- [ ] PostgreSQL
- [ ] Redis
- [ ] Serde
- [ ] Validator
- [ ] JWT / OAuth libraries
- [ ] Docker

---

# 2. Internet Fundamentals

Understand how a request travels from a client to a backend.

## Networking

- [ ] How the Internet works
- [ ] Client-server architecture
- [ ] IP addresses
- [ ] IPv4
- [ ] IPv6
- [ ] Ports
- [ ] TCP
- [ ] UDP
- [ ] TCP handshake
- [ ] DNS
- [ ] DNS records
- [ ] Domain names
- [ ] Routers
- [ ] NAT
- [ ] Firewalls
- [ ] Proxies
- [ ] Reverse proxies
- [ ] Load balancers

## HTTP

- [ ] HTTP request structure
- [ ] HTTP response structure
- [ ] HTTP methods
- [ ] GET
- [ ] POST
- [ ] PUT
- [ ] PATCH
- [ ] DELETE
- [ ] HTTP headers
- [ ] Cookies
- [ ] Query parameters
- [ ] Path parameters
- [ ] Request body
- [ ] Content-Type
- [ ] HTTP status codes
- [ ] HTTP/1.1
- [ ] HTTP/2
- [ ] HTTP/3
- [ ] HTTPS
- [ ] TLS
- [ ] Keep-alive
- [ ] Compression
- [ ] Caching headers

## Web infrastructure

- [ ] Hosting
- [ ] VPS
- [ ] Cloud hosting
- [ ] CDNs
- [ ] Static assets
- [ ] Reverse proxy with Nginx or Caddy

---

# 3. Linux & Operating Systems

- [ ] Linux filesystem
- [ ] Processes
- [ ] Threads
- [ ] Signals
- [ ] File permissions
- [ ] Users and groups
- [ ] Environment variables
- [ ] Processes and services
- [ ] Systemd basics
- [ ] SSH
- [ ] Bash
- [ ] Pipes
- [ ] Redirection
- [ ] `grep`
- [ ] `sed`
- [ ] `awk`
- [ ] `curl`
- [ ] `ss`
- [ ] `top` / `htop`
- [ ] Logs
- [ ] Disk usage
- [ ] Memory usage
- [ ] CPU usage

---

# 4. Version Control

## Git

- [ ] `git init`
- [ ] `git clone`
- [ ] `git add`
- [ ] `git commit`
- [ ] `git status`
- [ ] `git log`
- [ ] Branches
- [ ] Merging
- [ ] Rebasing
- [ ] Conflict resolution
- [ ] Stashing
- [ ] Tags
- [ ] Reverting
- [ ] Resetting
- [ ] Conventional commits

## Repository hosting

- [ ] GitHub
- [ ] GitLab
- [ ] Bitbucket
- [ ] Pull requests
- [ ] Code reviews
- [ ] Branch protection
- [ ] CI checks

---

# 5. Databases

## Relational databases

- [ ] PostgreSQL
- [ ] MySQL
- [ ] MariaDB
- [ ] SQLite
- [ ] SQL Server
- [ ] Oracle

### SQL fundamentals

- [ ] SELECT
- [ ] INSERT
- [ ] UPDATE
- [ ] DELETE
- [ ] WHERE
- [ ] ORDER BY
- [ ] GROUP BY
- [ ] HAVING
- [ ] LIMIT / OFFSET
- [ ] JOIN
- [ ] INNER JOIN
- [ ] LEFT JOIN
- [ ] RIGHT JOIN
- [ ] UNION
- [ ] Subqueries
- [ ] CTEs
- [ ] Window functions
- [ ] Aggregations
- [ ] CASE expressions
- [ ] NULL handling

### Database design

- [ ] Primary keys
- [ ] Foreign keys
- [ ] Unique constraints
- [ ] Check constraints
- [ ] NOT NULL
- [ ] Relationships
- [ ] One-to-one
- [ ] One-to-many
- [ ] Many-to-many
- [ ] Normalization
- [ ] Denormalization

### PostgreSQL advanced

- [ ] Indexes
- [ ] Composite indexes
- [ ] Partial indexes
- [ ] Unique indexes
- [ ] Full-text search
- [ ] Transactions
- [ ] ACID
- [ ] Isolation levels
- [ ] Row-level locking
- [ ] `SELECT ... FOR UPDATE`
- [ ] Deadlocks
- [ ] MVCC
- [ ] `EXPLAIN`
- [ ] `EXPLAIN ANALYZE`
- [ ] Query planning
- [ ] Connection pooling
- [ ] Database migrations
- [ ] Backups
- [ ] Replication

---

# 6. NoSQL Databases

Understand when relational databases are not the best fit.

- [ ] Key-value databases
- [ ] Document databases
- [ ] Wide-column databases
- [ ] Graph databases
- [ ] MongoDB
- [ ] Redis
- [ ] DynamoDB
- [ ] Neo4j

Do not learn every database deeply. Understand the trade-offs.

---

# 7. Caching

- [ ] Why caching exists
- [ ] Cache-aside
- [ ] Read-through caching
- [ ] Write-through caching
- [ ] Write-back caching
- [ ] Cache invalidation
- [ ] TTL
- [ ] Cache stampede
- [ ] Cache penetration
- [ ] Cache warming

## Redis

- [ ] Strings
- [ ] Hashes
- [ ] Lists
- [ ] Sets
- [ ] Sorted sets
- [ ] TTL
- [ ] Pub/Sub
- [ ] Streams
- [ ] Distributed locks
- [ ] Rate limiting
- [ ] Session storage

## Other caching layers

- [ ] Server-side cache
- [ ] Browser cache
- [ ] CDN cache

---

# 8. API Development

## REST

- [ ] Resource-oriented URLs
- [ ] HTTP methods
- [ ] Status codes
- [ ] Request validation
- [ ] Response serialization
- [ ] Error responses
- [ ] Pagination
- [ ] Filtering
- [ ] Sorting
- [ ] Searching
- [ ] Versioning
- [ ] Idempotency
- [ ] Rate limiting

Example:

```text
GET    /api/products
POST   /api/products
GET    /api/products/{id}
PATCH  /api/products/{id}
DELETE /api/products/{id}
```

## API documentation

- [ ] OpenAPI
- [ ] Swagger
- [ ] Request schemas
- [ ] Response schemas
- [ ] Authentication documentation
- [ ] Error documentation

## Other API styles

- [ ] JSON APIs
- [ ] GraphQL
- [ ] gRPC
- [ ] SOAP
- [ ] HATEOAS
- [ ] Webhooks

---

# 9. Authentication & Authorization

## Authentication

- [ ] Password authentication
- [ ] Password hashing
- [ ] Salt
- [ ] Sessions
- [ ] Cookies
- [ ] JWT
- [ ] Access tokens
- [ ] Refresh tokens
- [ ] Token expiration
- [ ] Token rotation

## Authorization

- [ ] Authentication vs authorization
- [ ] RBAC
- [ ] ABAC
- [ ] Permissions
- [ ] Roles
- [ ] Resource ownership
- [ ] Multi-tenant authorization

## Identity protocols

- [ ] OAuth 2.0
- [ ] OpenID Connect
- [ ] SAML
- [ ] Basic authentication
- [ ] API keys

---

# 10. Web Security

- [ ] HTTPS
- [ ] TLS
- [ ] SQL injection
- [ ] XSS
- [ ] CSRF
- [ ] SSRF
- [ ] CORS
- [ ] Clickjacking
- [ ] Session fixation
- [ ] Brute-force protection
- [ ] Rate limiting
- [ ] Input validation
- [ ] Output encoding
- [ ] Secure headers
- [ ] Secrets management
- [ ] Dependency vulnerabilities

## Cryptography basics

- [ ] Hashing
- [ ] SHA-256
- [ ] Password hashing
- [ ] bcrypt
- [ ] scrypt
- [ ] Argon2
- [ ] Encryption
- [ ] Symmetric encryption
- [ ] Asymmetric encryption
- [ ] Digital signatures
- [ ] Public/private keys

> Do not use MD5 or SHA-1 for password storage.

---

# 11. Testing

## Unit testing

- [ ] Unit tests
- [ ] Test isolation
- [ ] Mocking
- [ ] Fixtures
- [ ] Assertions

## Integration testing

- [ ] API integration tests
- [ ] Database integration tests
- [ ] Authentication tests
- [ ] Transaction tests

## End-to-end testing

- [ ] E2E tests
- [ ] API contract tests
- [ ] Critical user flows

## Rust testing

- [ ] `#[test]`
- [ ] Integration tests
- [ ] Async tests
- [ ] Test databases
- [ ] `cargo test`

---

# 12. Design Patterns

- [ ] Dependency Injection
- [ ] Repository Pattern
- [ ] Service Layer
- [ ] Factory
- [ ] Strategy
- [ ] Adapter
- [ ] Observer
- [ ] Builder
- [ ] Command
- [ ] Specification
- [ ] Unit of Work

Use patterns to solve real problems, not simply to increase abstraction.

---

# 13. Backend Architecture

## Layered architecture

```text
HTTP
 ↓
Handler / Controller
 ↓
Service
 ↓
Repository
 ↓
Database
```

## Other architectures

- [ ] Modular monolith
- [ ] Clean Architecture
- [ ] Hexagonal Architecture
- [ ] Domain-Driven Design
- [ ] Event-driven architecture
- [ ] Microservices
- [ ] Serverless

### Important concepts

- [ ] Separation of concerns
- [ ] Dependency inversion
- [ ] Domain boundaries
- [ ] Coupling
- [ ] Cohesion
- [ ] Business logic isolation
- [ ] Transaction boundaries

---

# 14. Background Jobs

Some operations should not block an HTTP request.

Examples:

```text
HTTP Request
     ↓
Create Order
     ↓
Queue Job
     ↓
Return 202
     ↓
Worker
     ↓
Send Email
Generate PDF
Process Payment
```

Learn:

- [ ] Job queues
- [ ] Workers
- [ ] Retries
- [ ] Exponential backoff
- [ ] Dead-letter queues
- [ ] Delayed jobs
- [ ] Scheduled jobs
- [ ] Idempotent jobs
- [ ] Job monitoring

Technologies:

- [ ] Redis queues
- [ ] RabbitMQ
- [ ] Kafka
- [ ] SQS
- [ ] BullMQ
- [ ] Celery
- [ ] Sidekiq

---

# 15. Message Brokers & Event Streaming

- [ ] Producer
- [ ] Consumer
- [ ] Topics
- [ ] Queues
- [ ] Partitions
- [ ] Consumer groups
- [ ] Message ordering
- [ ] Delivery guarantees
- [ ] At-most-once
- [ ] At-least-once
- [ ] Exactly-once concepts
- [ ] Event-driven architecture

Technologies:

- [ ] RabbitMQ
- [ ] Apache Kafka
- [ ] AWS SQS
- [ ] NATS

---

# 16. Containers

## Docker

- [ ] Images
- [ ] Containers
- [ ] Dockerfile
- [ ] Layers
- [ ] Volumes
- [ ] Networks
- [ ] Environment variables
- [ ] Docker Compose
- [ ] Multi-stage builds
- [ ] Container security

Example backend stack:

```text
┌──────────────┐
│ Actix API    │
├──────────────┤
│ PostgreSQL   │
├──────────────┤
│ Redis        │
└──────────────┘
```

---

# 17. CI/CD

- [ ] Continuous Integration
- [ ] Continuous Delivery
- [ ] Continuous Deployment
- [ ] Build pipelines
- [ ] Automated tests
- [ ] Linting
- [ ] Formatting
- [ ] Security scanning
- [ ] Docker builds
- [ ] Deployment pipelines
- [ ] Environment management
- [ ] Rollbacks

Tools:

- [ ] GitHub Actions
- [ ] GitLab CI
- [ ] Jenkins
- [ ] CircleCI

---

# 18. Cloud

Learn one cloud provider deeply enough to deploy production applications.

## AWS

- [ ] EC2
- [ ] S3
- [ ] RDS
- [ ] ElastiCache
- [ ] VPC
- [ ] IAM
- [ ] Route 53
- [ ] CloudFront
- [ ] SQS
- [ ] SES

Also understand:

- [ ] Azure
- [ ] Google Cloud

---

# 19. Web Servers & Reverse Proxies

- [ ] Nginx
- [ ] Caddy
- [ ] Apache
- [ ] Reverse proxy
- [ ] TLS termination
- [ ] Compression
- [ ] Static files
- [ ] Load balancing
- [ ] Health checks

---

# 20. Observability

## Logging

- [ ] Structured logging
- [ ] Log levels
- [ ] Request IDs
- [ ] Correlation IDs
- [ ] Centralized logs
- [ ] Error tracking

## Metrics

- [ ] Request rate
- [ ] Error rate
- [ ] Latency
- [ ] CPU
- [ ] Memory
- [ ] Database metrics
- [ ] Cache hit rate

## Tracing

- [ ] Distributed tracing
- [ ] Spans
- [ ] Trace IDs
- [ ] OpenTelemetry

Tools:

- [ ] Prometheus
- [ ] Grafana
- [ ] OpenTelemetry
- [ ] Sentry

---

# 21. Search

Understand dedicated search systems when PostgreSQL search is not enough.

- [ ] Full-text search
- [ ] Inverted indexes
- [ ] Tokenization
- [ ] Ranking
- [ ] Fuzzy search
- [ ] Elasticsearch
- [ ] OpenSearch
- [ ] Meilisearch

---

# 22. Real-Time Communication

- [ ] WebSockets
- [ ] Server-Sent Events
- [ ] Long polling
- [ ] Connection management
- [ ] Heartbeats
- [ ] Reconnection
- [ ] Pub/Sub
- [ ] Real-time notifications

---

# 23. Performance

## Application performance

- [ ] Profiling
- [ ] CPU optimization
- [ ] Memory optimization
- [ ] Async programming
- [ ] Concurrency
- [ ] Connection pooling
- [ ] Caching
- [ ] Batching
- [ ] Pagination

## Database performance

- [ ] Query optimization
- [ ] Index optimization
- [ ] `EXPLAIN ANALYZE`
- [ ] Avoid N+1 queries
- [ ] Connection pool sizing
- [ ] Slow query logging

## API performance

- [ ] Response compression
- [ ] HTTP caching
- [ ] CDN
- [ ] Keep-alive
- [ ] Streaming
- [ ] Rate limiting

---

# 24. Scalability

## Vertical scaling

```text
More CPU
More RAM
Faster disk
```

## Horizontal scaling

```text
             Load Balancer
                  │
       ┌──────────┼──────────┐
       ↓          ↓          ↓
    API #1     API #2     API #3
       │          │          │
       └──────────┼──────────┘
                  ↓
              Database
```

Learn:

- [ ] Stateless services
- [ ] Load balancing
- [ ] Horizontal scaling
- [ ] Database replication
- [ ] Read replicas
- [ ] Sharding concepts
- [ ] Caching
- [ ] Queue-based processing
- [ ] CDN
- [ ] Service discovery

---

# 25. Distributed Systems

- [ ] CAP theorem
- [ ] Consistency
- [ ] Availability
- [ ] Partition tolerance
- [ ] Eventual consistency
- [ ] Distributed locks
- [ ] Leader election
- [ ] Consensus concepts
- [ ] Idempotency
- [ ] Retries
- [ ] Timeouts
- [ ] Circuit breakers
- [ ] Bulkheads
- [ ] Backpressure
- [ ] Distributed transactions
- [ ] Saga pattern

---

# 26. System Design

Learn to design systems from requirements.

## Core concepts

- [ ] Functional requirements
- [ ] Non-functional requirements
- [ ] Availability
- [ ] Reliability
- [ ] Scalability
- [ ] Latency
- [ ] Throughput
- [ ] Durability
- [ ] Consistency
- [ ] Fault tolerance

## Design exercises

- [ ] URL shortener
- [ ] Authentication service
- [ ] E-commerce backend
- [ ] Payment system
- [ ] Notification system
- [ ] Chat application
- [ ] File storage service
- [ ] Food delivery backend
- [ ] Ride-sharing backend
- [ ] Social media feed
- [ ] Inventory management system

---

# 27. Advanced Backend Concepts

- [ ] Idempotency keys
- [ ] Optimistic locking
- [ ] Pessimistic locking
- [ ] Soft deletes
- [ ] Audit logs
- [ ] Outbox pattern
- [ ] Inbox pattern
- [ ] CQRS
- [ ] Event sourcing
- [ ] Feature flags
- [ ] Multi-tenancy
- [ ] API versioning
- [ ] Backward compatibility
- [ ] Data migrations
- [ ] Zero-downtime deployment

---

# 28. Production Backend Checklist

Before calling an API production-ready:

- [ ] Authentication implemented
- [ ] Authorization implemented
- [ ] Input validation
- [ ] Centralized error handling
- [ ] Structured logging
- [ ] Request IDs
- [ ] Rate limiting
- [ ] Database indexes
- [ ] Transactions where required
- [ ] Connection pooling
- [ ] Pagination
- [ ] Filtering
- [ ] Sorting
- [ ] API documentation
- [ ] Automated tests
- [ ] Health endpoint
- [ ] Readiness endpoint
- [ ] Metrics
- [ ] Error tracking
- [ ] Backups
- [ ] Secrets management
- [ ] HTTPS
- [ ] CI/CD
- [ ] Docker image
- [ ] Monitoring
- [ ] Rollback strategy

---

# 29. Rust + Actix Production Path

If your target is specifically **Rust Backend Developer**, use this sequence:

```text
Rust Fundamentals
        ↓
Ownership / Borrowing
        ↓
Traits / Generics
        ↓
Error Handling
        ↓
Async Rust
        ↓
Tokio
        ↓
Actix Web
        ↓
REST API
        ↓
PostgreSQL
        ↓
SQLx
        ↓
Advanced CRUD
        ↓
Authentication
        ↓
Redis
        ↓
Background Jobs
        ↓
Testing
        ↓
Docker
        ↓
CI/CD
        ↓
Observability
        ↓
Performance
        ↓
Concurrency
        ↓
System Design
```

## Capstone Project

Build one serious production-style application instead of many tiny tutorials.

### Example: Multi-tenant Inventory SaaS

- [ ] User registration
- [ ] Login
- [ ] JWT authentication
- [ ] RBAC
- [ ] Organizations / tenants
- [ ] Products
- [ ] Categories
- [ ] Warehouses
- [ ] Stock
- [ ] Stock movements
- [ ] Suppliers
- [ ] Customers
- [ ] Orders
- [ ] Invoices
- [ ] Pagination
- [ ] Filtering
- [ ] Search
- [ ] Redis caching
- [ ] Transactions
- [ ] Optimistic locking
- [ ] Audit logs
- [ ] Background jobs
- [ ] Email notifications
- [ ] API documentation
- [ ] Integration tests
- [ ] Docker
- [ ] CI/CD
- [ ] Monitoring

---

# 30. Interview Preparation

## Programming

- [ ] Data structures
- [ ] Algorithms
- [ ] Big-O
- [ ] Arrays
- [ ] Hash maps
- [ ] Stacks
- [ ] Queues
- [ ] Trees
- [ ] Graphs
- [ ] Recursion
- [ ] Sorting
- [ ] Searching

## Backend questions

- [ ] REST vs GraphQL
- [ ] PUT vs PATCH
- [ ] 401 vs 403
- [ ] Authentication vs authorization
- [ ] JWT vs sessions
- [ ] SQL vs NoSQL
- [ ] Indexes
- [ ] Transactions
- [ ] Isolation levels
- [ ] Optimistic vs pessimistic locking
- [ ] Caching strategies
- [ ] Connection pooling
- [ ] N+1 problem
- [ ] Rate limiting
- [ ] Idempotency
- [ ] Message queues
- [ ] Horizontal scaling
- [ ] Database replication
- [ ] Microservices trade-offs

## Rust interview topics

- [ ] Ownership
- [ ] Borrowing
- [ ] Lifetimes
- [ ] Traits
- [ ] Generics
- [ ] `Option`
- [ ] `Result`
- [ ] `Send`
- [ ] `Sync`
- [ ] `Arc`
- [ ] `Mutex`
- [ ] Async Rust
- [ ] Tokio
- [ ] Futures
- [ ] Actix Web
- [ ] SQLx
- [ ] Error handling
- [ ] Concurrency

---

# Final Milestones

## Beginner

- [ ] One programming language
- [ ] Git
- [ ] Linux basics
- [ ] HTTP
- [ ] SQL
- [ ] PostgreSQL
- [ ] Basic CRUD
- [ ] Basic REST API

## Junior Backend Developer

- [ ] Authentication
- [ ] Authorization
- [ ] Validation
- [ ] Testing
- [ ] API documentation
- [ ] Docker
- [ ] Deployment
- [ ] Basic caching

## Mid-Level Backend Developer

- [ ] Advanced PostgreSQL
- [ ] Transactions
- [ ] Query optimization
- [ ] Redis
- [ ] Background jobs
- [ ] Queues
- [ ] Observability
- [ ] Security
- [ ] CI/CD
- [ ] Performance optimization

## Senior Backend Developer

- [ ] System design
- [ ] Distributed systems
- [ ] Scalability
- [ ] High availability
- [ ] Event-driven architecture
- [ ] Advanced caching
- [ ] Database scaling
- [ ] Fault tolerance
- [ ] Architecture decisions
- [ ] Technical trade-offs

---

## Reference

This roadmap is an independently structured learning checklist based on the subject areas presented by the **roadmap.sh Backend Developer roadmap**.

Official roadmap: https://roadmap.sh/backend
