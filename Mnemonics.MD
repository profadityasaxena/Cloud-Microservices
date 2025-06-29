# 📘 Microservices Architecture Mnemonics (for Zhou et al. Framework)

---

## 🔍 1. Assessment Phase — *Mnemonic: `SCOPE`*

- **S** – *Static analysis tools* (e.g., Structure101, SonarQube)
- **C** – *Code profiling* with runtime tools (e.g., Jaeger, Dynatrace)
- **O** – *Ownership* and organizational readiness
- **P** – *Pilot services* to start with (low coupling, high value)
- **E** – *Engage* SMEs using DDD and Event Storming

---

## 🏗️ 2. Reference Architecture Design — *Mnemonic: `VIEW`*

- **V** – *Viewpoints* (component, deployment, communication, operational)
- **I** – *Integration* with CI/CD and ADRs
- **E** – *Enterprise roles* collaborate (architects, devs, ops, QA, PMs)
- **W** – *Workflow* alignment and traceability tools

---

## 🔁 3. Migration Strategy — *Mnemonic: `STRIDE`*

- **S** – *Strangler* pattern for incremental migration
- **T** – *Tooling* for traffic routing and coexistence (Kong, Istio)
- **R** – *Risk management* via rollback and feature flags
- **I** – *Integration* points analyzed ahead (API, DB, events)
- **D** – *Database* strategies (CDC, dual-write, views)
- **E** – *Execution* phased, not Big Bang

---

## ⚙️ 4. DevOps and Tooling Integration — *Mnemonic: `PULSE`*

- **P** – *Pipelines* (CI/CD: Jenkins, ArgoCD, GitHub Actions)
- **U** – *Unified observability* stack (Prometheus, Jaeger, Loki)
- **L** – *Linting and scanning* for security (Trivy, Snyk, SonarQube)
- **S** – *Self-service infra* with IaC (Terraform, Helm)
- **E** – *Environment automation* and rollback support

---

## 🔁 5. Validation and Feedback Loops — *Mnemonic: `TRACE`*

- **T** – *Telemetry* dashboards (Grafana, alerts, SLOs)
- **R** – *Reviews* and retrospectives (postmortems, audits)
- **A** – *Architecture conformance* checks (ArchUnit, Sonargraph)
- **C** – *Change tracking* with drift detection
- **E** – *End-to-end* validation via feedback resolution metrics

---

## 🧱 Design Pattern Mnemonics

### 🪴 Strangler Fig Pattern — *Mnemonic: `GROW`*

- **G** – *Gradual extraction*
- **R** – *Routing* via gateway
- **O** – *Operational coexistence*
- **W** – *Wrap legacy*, then replace

---

### 🧩 Decomposition — *Mnemonic: `BOUND`*

- **B** – *Business capabilities*
- **O** – *Ownership* clarity
- **U** – *Use DDD subdomains*
- **N** – *No premature splitting*
- **D** – *Domain-driven design*

---

### 🔗 Communication Patterns — *Mnemonic: `API FIT`*

- **A** – *API Gateway* centralizes access
- **P** – *Patterns*: Sync (REST/gRPC) vs Async (MQ)
- **I** – *Interfaces* managed via schema tools (OpenAPI, Protobuf)
- **F** – *Fallbacks* via retries, circuit breakers, timeouts
- **I** – *Integration rules* via orchestration/choreography
- **T** – *Testing* with contract tests (e.g., Pact)

---

### 🛡️ Resilience Patterns — *Mnemonic: `BRICK`*

- **B** – *Bulkhead* for isolation
- **R** – *Retry* with exponential backoff
- **I** – *Isolation* via thread pools or containers
- **C** – *Circuit breaker* for failure containment
- **K** – *Kill switch* with timeout/fallbacks

---

### 🔍 Observability Patterns — *Mnemonic: `LOGS`*

- **L** – *Logs* centralized (Loki, ELK)
- **O** – *OpenTelemetry* for tracing
- **G** – *Grafana* dashboards and alerting
- **S** – *Sidecars* for uniform instrumentation

---
