# Adeleke Dare | DevOps & Infrastructure Engineer

[![GitHub Actions](https://img.shields.io/badge/CI/CD-GitHub%20Actions-24292f?logo=githubactions&logoColor=white)](https://github.com/darestack?tab=repositories)
[![AWS](https://img.shields.io/badge/Cloud-AWS-232f3e?logo=amazonwebservices&logoColor=white)](https://github.com/darestack/github-actions-ec2-pipeline)
[![Docker](https://img.shields.io/badge/Containers-Docker-2496ed?logo=docker&logoColor=white)](https://github.com/darestack/glpi-ticketing-system)
[![FastAPI](https://img.shields.io/badge/Backend-FastAPI-009688?logo=fastapi&logoColor=white)](https://github.com/darestack/api-reliability-suite)
[![Linux](https://img.shields.io/badge/Systems-Linux-fcc624?logo=linux&logoColor=black)](https://github.com/darestack/devops-labs)

Lagos, Nigeria | [LinkedIn](https://www.linkedin.com/in/darestack/) | [Blog](https://dev.to/darestack) | [Email](mailto:adelekedare2012@gmail.com)

I build backend services and infrastructure labs that are easy to verify: CI/CD pipelines, AWS EC2 release automation, Dockerized IT support systems, and observable FastAPI services.

Open to DevOps Engineer, IT Support / Systems, and Backend Infrastructure roles.

## 30-Second Scan

| Capability | Proof to Review |
|---|---|
| CI/CD release automation | [EC2 release pipeline](https://github.com/darestack/github-actions-ec2-pipeline) with build/test, tag-triggered deploy, PM2 reload, rollback script, and scheduled health checks |
| Backend reliability | [API Reliability Suite](https://github.com/darestack/api-reliability-suite) with auth, rate limiting, readiness checks, Prometheus/Grafana/Jaeger, and circuit-breaker fallback |
| Container pipeline quality gates | [GitHub Actions CI/CD demo](https://github.com/darestack/github-actions-cicd-demo) with Node matrix tests, ESLint, Trivy SARIF, Docker Buildx, and GHCR publishing |
| IT systems operations | [GLPI ticketing system](https://github.com/darestack/glpi-ticketing-system) deployed with Docker Compose, MariaDB, persistent volumes, SLA categories, roles, and asset workflow notes |
| Infrastructure breadth | [DevOps labs](https://github.com/darestack/devops-labs) covering Linux, AWS, Docker, Kubernetes, Terraform, Ansible, Prometheus, Grafana, and capstone deployments |

## Selected Projects

| Project | What It Demonstrates | Evidence Status |
|---|---|---|
| [API Reliability Suite](https://github.com/darestack/api-reliability-suite) | FastAPI service with JWT auth, refresh-token rotation, rate limiting, readiness checks, structured logs, Prometheus metrics, Grafana dashboards, Jaeger tracing, and Redis-backed fallback behavior | CI badge, docs site, test suite, load-test report, Grafana and AI-debug screenshots |
| [EC2 Release Pipeline](https://github.com/darestack/github-actions-ec2-pipeline) | GitHub Actions workflow that tests a Node/Express app, creates release tags, deploys to EC2 over SSH, reloads with PM2, and keeps rollback logic in `scripts/deploy.sh` | Workflow files, deploy script, scheduled health-check workflow |
| [Container CI/CD Pipeline](https://github.com/darestack/github-actions-cicd-demo) | Node.js pipeline with Node 22/24 tests, linting, Trivy SARIF upload, Docker Buildx, GHCR image publishing, and simulated staging/production rollout steps | Workflow file is reviewable; real deployment target still needs to be connected |
| [GLPI Helpdesk Lab](https://github.com/darestack/glpi-ticketing-system) | Self-hosted ITSM/helpdesk lab using GLPI, MariaDB, Docker Compose, named volumes, internal-only database networking, ticket categories, SLA policy notes, and support roles | Compose file plus [implementation write-up](https://dev.to/darestack/from-zero-to-helpdesk-hero-building-an-enterprise-it-support-system-with-glpi-hpe); screenshots should be added |
| [DevOps Labs](https://github.com/darestack/devops-labs) | Training portfolio with capstones for AWS HA WordPress, e-commerce CI/CD, and Terraform plus observability stack | Lab READMEs are indexed; best screenshots and metrics should be promoted to the root README |

## Skills Mapped to Work

| Skill Area | Projects |
|---|---|
| GitHub Actions, CI/CD, release automation | `github-actions-ec2-pipeline`, `github-actions-cicd-demo` |
| AWS, EC2, IAM, deployment operations | `github-actions-ec2-pipeline`, `devops-labs` |
| Docker and service deployment | `glpi-ticketing-system`, `github-actions-cicd-demo`, `api-reliability-suite` |
| Monitoring and observability | `api-reliability-suite`, `devops-labs` |
| Linux and systems administration | `devops-labs`, `glpi-ticketing-system` |
| Backend infrastructure | `api-reliability-suite`, `github-actions-ec2-pipeline` |

## Portfolio Standard

I keep the pinned portfolio small and evidence-based. Training projects are labeled as labs, simulated deployments are called out as simulations, and every major project should include at least one reviewable artifact: workflow run, screenshot, log output, dashboard, load-test result, or deployment note.

## Writing

[dev.to/darestack](https://dev.to/darestack) - notes on DevOps, Linux, backend reliability, and hands-on infrastructure projects.
