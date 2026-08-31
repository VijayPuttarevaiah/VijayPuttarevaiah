## Vijay Puttarevaiah

**Software Engineer — Java · Spring Boot · Microservices · AWS**

Five years in IT: three-plus building backend and full-stack applications in Java, Spring Boot, and TypeScript at Wipro and Acuver Consulting, and a year and a half in SQL-based fraud analysis at Amazon. The engineering work was integration-heavy — Spring Boot services talking to third-party APIs that fail in ways you don't control, and the retry, fallback, and failover logic that keeps them reliable anyway.

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

### Technical Skills

**Languages**

<p>
<img height="38" alt="Java" title="Java" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/java/java-original.svg" />&nbsp;
<img height="38" alt="TypeScript" title="TypeScript" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/typescript/typescript-original.svg" />&nbsp;
<img height="38" alt="JavaScript" title="JavaScript" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/javascript/javascript-original.svg" />&nbsp;
<img height="38" alt="Python" title="Python" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/python/python-original.svg" />&nbsp;
<img height="38" alt="HTML5" title="HTML5" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/html5/html5-original.svg" />&nbsp;
<img height="38" alt="CSS3" title="CSS3" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/css3/css3-original.svg" />&nbsp;
<img height="28" alt="SQL" src="https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logoColor=white" />
</p>

**Backend & APIs**

<p>
<img height="38" alt="Spring Boot" title="Spring Boot" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/spring/spring-original.svg" />&nbsp;
<img height="38" alt="Hibernate" title="Hibernate" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/hibernate/hibernate-original.svg" />&nbsp;
<img height="38" alt="Django" title="Django" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/django/django-plain.svg" />&nbsp;
<img height="38" alt="FastAPI" title="FastAPI" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/fastapi/fastapi-original.svg" />&nbsp;
<img height="38" alt="GraphQL" title="GraphQL" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/graphql/graphql-plain.svg" />
</p>

<p>
<img height="28" alt="Spring MVC" src="https://img.shields.io/badge/Spring_MVC-6DB33F?style=for-the-badge&logo=spring&logoColor=white" />&nbsp;
<img height="28" alt="Spring Security" src="https://img.shields.io/badge/Spring_Security-6DB33F?style=for-the-badge&logo=springsecurity&logoColor=white" />&nbsp;
<img height="28" alt="Spring Data JPA" src="https://img.shields.io/badge/Spring_Data_JPA-6DB33F?style=for-the-badge&logo=spring&logoColor=white" />&nbsp;
<img height="28" alt="REST APIs" src="https://img.shields.io/badge/REST_APIs-0F6C7E?style=for-the-badge&logoColor=white" />
</p>

**Frontend**

<p>
<img height="38" alt="React.js" title="React.js" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/react/react-original.svg" />&nbsp;
<picture><source media="(prefers-color-scheme: dark)" srcset="https://cdn.simpleicons.org/nextdotjs/ffffff"><img height="38" alt="Next.js" title="Next.js" src="https://cdn.simpleicons.org/nextdotjs/000000" /></picture>&nbsp;
<img height="28" alt="React Native" src="https://img.shields.io/badge/React_Native-20232A?style=for-the-badge&logo=react&logoColor=61DAFB" />
</p>

**Cloud & DevOps**

<p>
<img height="38" alt="AWS" title="AWS" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/amazonwebservices/amazonwebservices-original-wordmark.svg" />&nbsp;
<img height="38" alt="Docker" title="Docker" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/docker/docker-original.svg" />&nbsp;
<img height="38" alt="Kubernetes" title="Kubernetes" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/kubernetes/kubernetes-original.svg" />&nbsp;
<img height="38" alt="Jenkins" title="Jenkins" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/jenkins/jenkins-original.svg" />&nbsp;
<img height="38" alt="Terraform" title="Terraform" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/terraform/terraform-original.svg" />&nbsp;
<img height="38" alt="Maven" title="Maven" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/maven/maven-original.svg" />
</p>

<p>
<img height="28" alt="CI/CD" src="https://img.shields.io/badge/CI%2FCD-2088FF?style=for-the-badge&logo=githubactions&logoColor=white" />&nbsp;
<img height="28" alt="Continuous Delivery" src="https://img.shields.io/badge/Continuous_Delivery-2088FF?style=for-the-badge&logoColor=white" />
</p>

**Operating Systems**

<p>
<img height="38" alt="Linux" title="Linux" src="https://cdn.simpleicons.org/linux/FCC624" />&nbsp;
<img height="38" alt="Windows" title="Windows" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/windows11/windows11-original.svg" />
</p>

**Databases**

<p>
<img height="38" alt="PostgreSQL" title="PostgreSQL" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/postgresql/postgresql-original.svg" />&nbsp;
<img height="38" alt="MySQL" title="MySQL" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/mysql/mysql-original.svg" />&nbsp;
<img height="38" alt="MongoDB" title="MongoDB" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/mongodb/mongodb-original.svg" />&nbsp;
<img height="38" alt="DynamoDB" title="DynamoDB" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/dynamodb/dynamodb-original.svg" />&nbsp;
<img height="28" alt="H2" src="https://img.shields.io/badge/H2-09476B?style=for-the-badge&logoColor=white" />
</p>

**Testing**

<p>
<img height="38" alt="JUnit 5" title="JUnit 5" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/junit/junit-original.svg" />&nbsp;
<img height="38" alt="Vitest" title="Vitest" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/vitest/vitest-original.svg" />&nbsp;
<img height="38" alt="Pytest" title="Pytest" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/pytest/pytest-original.svg" />
</p>

<p>
<img height="28" alt="Mockito" src="https://img.shields.io/badge/Mockito-78A641?style=for-the-badge&logoColor=white" />&nbsp;
<img height="28" alt="TDD" src="https://img.shields.io/badge/TDD-2C3E50?style=for-the-badge&logoColor=white" />&nbsp;
<img height="28" alt="Automated Testing" src="https://img.shields.io/badge/Automated_Testing-2C3E50?style=for-the-badge&logoColor=white" />&nbsp;
<img height="28" alt="Unit, Integration and E2E" src="https://img.shields.io/badge/Unit_%7C_Integration_%7C_E2E-2C3E50?style=for-the-badge&logoColor=white" />
</p>

**Observability**

<p>
<img height="38" alt="Grafana" title="Grafana" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/grafana/grafana-original.svg" />&nbsp;
<img height="38" alt="Prometheus" title="Prometheus" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/prometheus/prometheus-original.svg" />&nbsp;
<img height="28" alt="AWS CloudWatch" src="https://img.shields.io/badge/AWS_CloudWatch-FF4F8B?style=for-the-badge&logo=amazonwebservices&logoColor=white" />&nbsp;
<img height="28" alt="Structured Logging" src="https://img.shields.io/badge/Structured_Logging-2C3E50?style=for-the-badge&logoColor=white" />
</p>

**AI & LLM**

<p>
<picture><source media="(prefers-color-scheme: dark)" srcset="https://cdn.simpleicons.org/claude/ffffff"><img height="38" alt="Anthropic Claude API" title="Anthropic Claude API" src="https://cdn.simpleicons.org/claude/000000" /></picture>&nbsp;
<picture><source media="(prefers-color-scheme: dark)" srcset="https://cdn.simpleicons.org/githubcopilot/ffffff"><img height="38" alt="GitHub Copilot" title="GitHub Copilot" src="https://cdn.simpleicons.org/githubcopilot/000000" /></picture>&nbsp;
<picture><source media="(prefers-color-scheme: dark)" srcset="https://cdn.simpleicons.org/cursor/ffffff"><img height="38" alt="Cursor" title="Cursor" src="https://cdn.simpleicons.org/cursor/000000" /></picture>
</p>

<p>
<img height="28" alt="AWS Bedrock" src="https://img.shields.io/badge/AWS_Bedrock-232F3E?style=for-the-badge&logo=amazonwebservices&logoColor=FF9900" />&nbsp;
<img height="28" alt="Groq API" src="https://img.shields.io/badge/Groq_API-F55036?style=for-the-badge&logoColor=white" />&nbsp;
<img height="28" alt="LLM Integration" src="https://img.shields.io/badge/LLM_Integration-6E56CF?style=for-the-badge&logoColor=white" />
</p>

**Tools**

<p>
<img height="38" alt="Git" title="Git" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/git/git-original.svg" />&nbsp;
<picture><source media="(prefers-color-scheme: dark)" srcset="https://cdn.simpleicons.org/github/ffffff"><img height="38" alt="GitHub" title="GitHub" src="https://cdn.simpleicons.org/github/181717" /></picture>&nbsp;
<img height="38" alt="GitLab" title="GitLab" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/gitlab/gitlab-original.svg" />&nbsp;
<img height="38" alt="Bitbucket" title="Bitbucket" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/bitbucket/bitbucket-original.svg" />&nbsp;
<img height="38" alt="Confluence" title="Confluence" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/confluence/confluence-original.svg" />
</p>

**Core CS & Practices**

Data Structures & Algorithms · Object-Oriented Programming · Software Design Principles · Distributed Systems · Microservices · Cloud-Native Applications · Scalable Application Design · Agile/Scrum · Code Reviews · SDLC

---

### Education & Certifications

**Master of Applied Computer Science** — Dalhousie University, Halifax · Jan 2026 – Apr 2027 · GPA 3.88/4.30
**B.E. Electrical & Electronics Engineering** — National Institute of Engineering, Mysuru

AWS Certified AI Practitioner · AWS Certified Cloud Practitioner
*In progress* — AWS Certified Solutions Architect – Associate · Claude Certified Architect – Foundations

---

### Contact

[LinkedIn](LINKEDIN_URL_HERE) · [vijayputtarevaiah@gmail.com](mailto:vijayputtarevaiah@gmail.com)
