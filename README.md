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
| CI/CD release automation | [EC2 release pipeline](https://github.com/darestack/github-actions-ec2-pipeline) with Node 22/24 build/test gates, controlled manual/tag deploy, PM2 reload, rollback script, and scheduled health checks |
| Backend reliability | [API Reliability Suite](https://github.com/darestack/api-reliability-suite) with auth, rate limiting, readiness checks, Prometheus/Grafana/Jaeger, and circuit-breaker fallback |
| Container pipeline quality gates | [GitHub Actions CI/CD demo](https://github.com/darestack/github-actions-cicd-demo) with Node matrix tests, ESLint, Trivy SARIF, Docker Buildx, and GHCR publishing |
| IT systems operations | [GLPI ticketing system](https://github.com/darestack/glpi-ticketing-system) with Docker Compose, MariaDB, persistent volumes, ITSM workflow notes, and a [documented implementation write-up](https://dev.to/darestack/from-zero-to-helpdesk-hero-building-an-enterprise-it-support-system-with-glpi-hpe) |
| Infrastructure breadth | [DevOps labs](https://github.com/darestack/devops-labs) covering Linux, AWS, Docker, Kubernetes, Terraform, Ansible, Prometheus, Grafana, and capstone deployments |

## Selected Projects

| Project | What It Demonstrates | Evidence Status |
|---|---|---|
| [API Reliability Suite](https://github.com/darestack/api-reliability-suite) | FastAPI service with JWT auth, refresh-token rotation, rate limiting, readiness checks, structured logs, Prometheus metrics, Grafana dashboards, Jaeger tracing, and Redis-backed fallback behavior | Passing [CI](https://github.com/darestack/api-reliability-suite/actions/runs/25492789987), [Security](https://github.com/darestack/api-reliability-suite/actions/runs/25492790028), and [Docs](https://github.com/darestack/api-reliability-suite/actions/runs/25492790000) runs; load-test report, Grafana, and AI-debug screenshots |
| [EC2 Release Pipeline](https://github.com/darestack/github-actions-ec2-pipeline) | GitHub Actions workflow that tests a Node/Express app on Node 22/24, deploys to EC2 from a manual or pushed `v*` tag, reloads with PM2, and keeps rollback logic in `scripts/deploy.sh` | Passing [CI matrix run](https://github.com/darestack/github-actions-ec2-pipeline/actions/runs/25493804477), deploy script, and scheduled health-check workflow; live EC2 deploy evidence still needs to be captured |
| [Container CI/CD Pipeline](https://github.com/darestack/github-actions-cicd-demo) | Node.js pipeline with Node 22/24 tests, linting, Trivy SARIF upload, Docker Buildx, GHCR image publishing, and simulated staging/production rollout steps | Passing [GitHub Actions workflow](https://github.com/darestack/github-actions-cicd-demo/actions/runs/25490869471); real deployment target still needs to be connected |
| [GLPI Helpdesk Lab](https://github.com/darestack/glpi-ticketing-system) | Self-hosted ITSM/helpdesk lab using GLPI, MariaDB, Docker Compose, named volumes, internal-only database networking, ticket categories, SLA policy notes, and support roles | Compose file, operations runbook, backup/restore/smoke-test scripts, and [implementation write-up](https://dev.to/darestack/from-zero-to-helpdesk-hero-building-an-enterprise-it-support-system-with-glpi-hpe); copy redacted screenshots into the repo next |
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

- [GLPI helpdesk implementation](https://dev.to/darestack/from-zero-to-helpdesk-hero-building-an-enterprise-it-support-system-with-glpi-hpe) - ITSM setup, web server troubleshooting, roles, assets, tickets, SLA notes, and reporting.
- [dev.to/darestack](https://dev.to/darestack) - notes on DevOps, Linux, backend reliability, and hands-on infrastructure projects.
