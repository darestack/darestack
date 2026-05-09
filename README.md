# Adeleke Dare | DevOps & Infrastructure Engineer

Lagos, Nigeria | [LinkedIn](https://www.linkedin.com/in/darestack/) | [Blog](https://dev.to/darestack) | [Email](mailto:adelekedare2012@gmail.com)

I work on the practical side of backend and infrastructure: getting services deployed, watched, recovered, and documented well enough that another engineer can understand what is going on.

Right now my strongest work sits around CI/CD, Docker, AWS EC2 deployments, monitoring, and small backend systems that show reliability thinking.

## What I Work On

| Area | Work You Can Review |
|---|---|
| CI/CD and release automation | [github-actions-ec2-pipeline](https://github.com/darestack/github-actions-ec2-pipeline) - Node 22/24 build and test checks, controlled EC2 deployment, PM2 reloads, rollback script, and scheduled health checks |
| Backend reliability | [api-reliability-suite](https://github.com/darestack/api-reliability-suite) - FastAPI service with auth, rate limiting, readiness checks, metrics, tracing, dashboards, and fallback behavior |
| Container pipeline checks | [github-actions-cicd-demo](https://github.com/darestack/github-actions-cicd-demo) - GitHub Actions matrix tests, ESLint, Trivy SARIF upload, Docker Buildx, and GHCR publishing |
| IT systems operations | [glpi-ticketing-system](https://github.com/darestack/glpi-ticketing-system) - Docker Compose GLPI helpdesk lab with MariaDB, persistent storage, operations scripts, and ITSM workflow notes |
| DevOps lab work | [devops-labs](https://github.com/darestack/devops-labs) - hands-on labs across Linux, AWS, Docker, Kubernetes, Terraform, Ansible, Prometheus, and Grafana |

## Projects To Start With

| Project | Why It Is Here | Evidence |
|---|---|---|
| [API Reliability Suite](https://github.com/darestack/api-reliability-suite) | A backend reliability project: JWT auth, refresh-token rotation, rate limits, readiness checks, structured logs, Prometheus metrics, Grafana dashboards, Jaeger tracing, and Redis-backed fallback behavior | Passing [CI](https://github.com/darestack/api-reliability-suite/actions/runs/25492789987), [Security](https://github.com/darestack/api-reliability-suite/actions/runs/25492790028), and [Docs](https://github.com/darestack/api-reliability-suite/actions/runs/25492790000) runs, plus local load-test and dashboard evidence |
| [EC2 Release Pipeline](https://github.com/darestack/github-actions-ec2-pipeline) | A GitHub Actions release flow for a Node/Express app on EC2. It tests on Node 22/24, deploys from a manual run or `v*` tag, reloads with PM2, and keeps rollback logic in `scripts/deploy.sh` | Passing [CI matrix run](https://github.com/darestack/github-actions-ec2-pipeline/actions/runs/25493804477), deploy script, and scheduled health-check workflow. Live EC2 screenshots still need to be captured |
| [Container CI/CD Pipeline](https://github.com/darestack/github-actions-cicd-demo) | A container pipeline lab with tests, linting, Trivy SARIF, Docker Buildx, GHCR publishing, and simulated staging/production rollout steps | Passing [GitHub Actions workflow](https://github.com/darestack/github-actions-cicd-demo/actions/runs/25490869471). The deploy stage is intentionally marked as simulated until a real target is connected |
| [GLPI Helpdesk Lab](https://github.com/darestack/glpi-ticketing-system) | A self-hosted ITSM/helpdesk lab using GLPI, MariaDB, Docker Compose, named volumes, internal database networking, ticket categories, SLA notes, and support roles | Compose file, operations runbook, backup/restore/smoke-test scripts, and a [setup write-up](https://dev.to/darestack/from-zero-to-helpdesk-hero-building-an-enterprise-it-support-system-with-glpi-hpe) |
| [DevOps Labs](https://github.com/darestack/devops-labs) | My broader lab archive. It is useful because it shows the path from Linux and AWS basics into Terraform, Ansible, Kubernetes, and monitoring work | The root README now points to the strongest capstones and separates finished evidence from areas that still need screenshots or run logs |

## Skills In Practice

| Skill Area | Projects |
|---|---|
| GitHub Actions and release automation | `github-actions-ec2-pipeline`, `github-actions-cicd-demo` |
| AWS, EC2, IAM, and deployment operations | `github-actions-ec2-pipeline`, `devops-labs` |
| Docker and service deployment | `glpi-ticketing-system`, `github-actions-cicd-demo`, `api-reliability-suite` |
| Monitoring and observability | `api-reliability-suite`, `devops-labs` |
| Linux and systems administration | `devops-labs`, `glpi-ticketing-system` |
| Backend infrastructure | `api-reliability-suite`, `github-actions-ec2-pipeline` |

## How I Present The Work

I try to keep the portfolio honest. Labs are called labs. Simulated deployments are called simulated. When a project is strong, I want the proof to be close by: a workflow run, a screenshot, a log, a dashboard, a test report, or a short note explaining what was verified.

## Writing

- [GLPI helpdesk implementation](https://dev.to/darestack/from-zero-to-helpdesk-hero-building-an-enterprise-it-support-system-with-glpi-hpe) - my write-up on setting up GLPI, troubleshooting the web server, and organizing tickets, roles, assets, SLA notes, and reports.
- [dev.to/darestack](https://dev.to/darestack) - notes from my DevOps, Linux, backend reliability, and infrastructure work.
