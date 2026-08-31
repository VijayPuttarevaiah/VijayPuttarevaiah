## Vijay Puttarevaiah

**Software Engineer — Java · Spring Boot · Microservices · AWS**

Five years building production backend systems: order management and logistics integrations at Acuver Consulting, healthcare claims infrastructure at Wipro, and fraud-detection tooling at Amazon. The work was integration-heavy — Spring Boot services talking to third-party APIs that fail in ways you don't control, and the retry, fallback, and failover logic that keeps them reliable anyway.

Now completing a Master of Applied Computer Science at Dalhousie University, Halifax, focused on distributed architecture and cloud systems.

Halifax, NS · Eligible to work in Canada

---

### Professional Work

**Vendor failover for same-day delivery** · *Acuver Consulting, 2025*
Rerouting system that automatically moves same-day orders between delivery vendors when one initiates a cancellation, shipped behind per-location kill switches for controlled rollout. Cut the client's vendor-caused cancellation rate from ~10% to under 1% of yearly online order volume.
`Java` `Spring Boot` `Spring Security` `JWT` `Microservices` `AWS` `DynamoDB` `Kubernetes`

**Carrier management integrations** · *Acuver Consulting, 2025*
Turnaround-time and waybill-generation APIs across four logistics carriers — scheduled polling for the three without webhook support, event-driven for the one that had it. Strategy pattern for swappable per-carrier logic, plus AWB-failure fallbacks so one carrier's outage never blocked shipment creation.
`Java` `Spring Boot` `Spring WebFlux` `Spring Data JPA` `MongoDB` `React`

**Claims platform modernization** · *Wipro, 2022–2024*
Migrated real-time claims scrubbing off a legacy BPM platform, containerized the resulting Spring Boot services, and led the Kubernetes rollout across environments through Jenkins — cutting infrastructure cost 20%. Built the organization-wide health-check service from scratch.
`Java` `Spring Boot` `OAuth 2.0` `MySQL` `Docker` `Kubernetes` `Jenkins`

**Fraud detection** · *Amazon, 2020–2022*
Detection-tool features in Java and performance tuning on the existing pipeline, contributing to a 30% increase in fraud-detection accuracy.
`Java` `SQL`

---

### Projects

**[Triage](https://github.com/VijayPuttarevaiah/triage) — Autonomous incident response**
Detects, diagnoses, and remediates production incidents on a Spring Boot fintech workload. Ten Lambdas orchestrated through a Step Functions state machine, triggered by CloudWatch alarms. The model only ever *names* an action — a separate policy engine decides auto-remediate versus human approval, so the LLM never calls an AWS API directly. Sub-120s MTTR target, validated through built-in chaos endpoints. ~100 Terraform-managed resources, 16 least-privilege IAM roles, OIDC-federated CI/CD with no stored credentials.
`AWS Bedrock` `Step Functions` `Lambda` `DynamoDB` `Terraform` `Python` `Spring Boot`

**[MeetFocus](https://github.com/VijayPuttarevaiah/meetfocus) — Link-less video conferencing**
Five Spring Boot microservices plus a FastAPI moderation service, coordinated over Kafka with Eureka discovery. Invites relay from Kafka straight into an attendee's open WebSocket session; chat routes through a toxicity classifier and back, blocking flagged messages before broadcast. Thread-safe telemetry engine validated against 150 parallel connections.
`Java` `Spring Boot` `Kafka` `WebSocket` `Eureka` `FastAPI` `PostgreSQL` `Redis` `Docker`

**[LEDGR](https://github.com/VijayPuttarevaiah/ledgr) — Personal finance and bill splitting**
A user's share of any shared group expense flows into their personal ledger with no manual reconciliation. Row-Level Security at the database, zod as the server-side authorization boundary on every mutating route, and AI features behind a kill switch that re-verifies server-side regardless of client state. Semgrep SAST clean, OWASP ZAP findings resolved, 63 tests in CI including property-based fuzzing of the split-math invariant.
`Next.js` `TypeScript` `Supabase` `PostgreSQL` `React Native` `Vitest` `Playwright`

**[Recalibrate](https://github.com/VijayPuttarevaiah/recalibrate) — Adaptive goal tracking**
Four-person team, largest individual contributor, owning CI/CD and code quality. GitLab CI through deployment to AWS EC2, Alembic-versioned MySQL schema, and DPy static design-smell detection as an enforced CI gate. LLM goal-detection built behind a provider-agnostic interface rather than a hardcoded integration.
`Python` `FastAPI` `React` `MySQL` `Alembic` `GitLab CI` `AWS EC2` `Docker`

**Open source** — Refactoring pull request to [Shopizer](https://github.com/shopizer-ecommerce/shopizer), an established Java e-commerce platform: strategy pattern replacing an if-else chain in payment processing, extracted shipping facade, consolidated mapper duplication. Zero new issues on the project's quality gate, full existing suite green. *Open for review.*

---

### Technology

**Production, daily** — Java · Spring Boot · Spring MVC · Spring WebFlux · Spring Data JPA · Microservices · REST APIs · Spring Security · JWT · OAuth 2.0 · Docker · Kubernetes · Jenkins · Git

**Cloud & infrastructure** — AWS (Lambda, Step Functions, ECS Fargate, EC2, DynamoDB, S3, SNS, SQS, API Gateway, EventBridge, CloudWatch, IAM, VPC, Bedrock) · Terraform · Kafka · Redis · GitHub Actions · GitLab CI

**Data** — PostgreSQL · MySQL · MongoDB · DynamoDB

**Frontend** — React · Next.js · Redux · TypeScript · React Native

**Also work with** — Python · FastAPI · JUnit · Mockito · pytest · Vitest · Hibernate · Postman

---

### Education & Certifications

**Master of Applied Computer Science** — Dalhousie University, Halifax · Jan 2026 – Apr 2027 · GPA 3.88/4.30
**B.E. Electrical & Electronics Engineering** — National Institute of Engineering, Mysuru

AWS Certified AI Practitioner · AWS Certified Cloud Practitioner
*In progress* — AWS Certified Solutions Architect – Associate · Claude Certified Architect – Foundations

---

### Contact

[LinkedIn](LINKEDIN_URL_HERE) · [vijayputtarevaiah@gmail.com](mailto:vijayputtarevaiah@gmail.com)
