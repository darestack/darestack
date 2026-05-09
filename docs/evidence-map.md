# Portfolio Evidence Map

This is the working map for the portfolio. The profile README stays short; this file keeps the proof links, companion repo notes, and remaining evidence gaps in one place.

## Evidence Ready Now

| Project | Evidence |
|---|---|
| [api-reliability-suite](https://github.com/darestack/api-reliability-suite) | Passing [CI](https://github.com/darestack/api-reliability-suite/actions/runs/25492789987), [Security](https://github.com/darestack/api-reliability-suite/actions/runs/25492790028), and [Docs](https://github.com/darestack/api-reliability-suite/actions/runs/25492790000) runs; committed [Grafana dashboard](https://github.com/darestack/api-reliability-suite/blob/main/docs/assets/grafana-dashboard.png) and [AI-debug screenshot](https://github.com/darestack/api-reliability-suite/blob/main/docs/assets/ai-debug-screenshot.png) |
| [github-actions-ec2-pipeline](https://github.com/darestack/github-actions-ec2-pipeline) | Passing [CI matrix run](https://github.com/darestack/github-actions-ec2-pipeline/actions/runs/25493804477), passing [scheduled health check](https://github.com/darestack/github-actions-ec2-pipeline/actions/runs/25594858992), controlled release workflow, and rollback script |
| [github-actions-cicd-demo](https://github.com/darestack/github-actions-cicd-demo) | Passing [CI/CD workflow](https://github.com/darestack/github-actions-cicd-demo/actions/runs/25490869471) with Node 22/24 matrix, linting, Trivy SARIF upload, Docker Buildx, and GHCR publish path |
| [glpi-ticketing-system](https://github.com/darestack/glpi-ticketing-system) | Docker Compose runtime, operations runbook, backup/restore/smoke-test scripts, and [implementation write-up](https://dev.to/darestack/from-zero-to-helpdesk-hero-building-an-enterprise-it-support-system-with-glpi-hpe) |
| [devops-labs](https://github.com/darestack/devops-labs) | Root evidence map, capstone write-ups, screenshots inside module folders, Terraform files, Ansible playbooks, and GitHub Actions workflow files |

## Capstone And Companion Repo Positioning

| Work | Main Place To Review | Companion Repo | How To Position It |
|---|---|---|---|
| WordPress HA on AWS | [devops-labs Capstone 4](https://github.com/darestack/devops-labs/tree/main/Module-2/capstone-project-4) | None yet | Keep inside `devops-labs` until it is extracted as a focused `terraform-aws-wordpress-ha` or `aws-wordpress-ha-lab` repo with IaC and fresh screenshots |
| E-commerce CI/CD | [devops-labs Capstone 5](https://github.com/darestack/devops-labs/tree/main/Module-3/capstone-project-5) | [ecommerce-platform](https://github.com/darestack/ecommerce-platform) | Treat as a companion app repo. It now has passing CI and Docker Publish evidence, but still needs current screenshots before it should be promoted |
| EC2 release automation | [github-actions-ec2-pipeline](https://github.com/darestack/github-actions-ec2-pipeline) | Related devops-labs mini-project notes | This is polished enough to stay as a headline repo because the workflow, health check, and rollback story are easy to review |
| Container CI/CD quality gates | [github-actions-cicd-demo](https://github.com/darestack/github-actions-cicd-demo) | Related devops-labs mini-project notes | Keep as a headline repo. It is clearer than burying the Actions work inside `devops-labs` |
| MarketPeak EC2 deployment | [devops-labs Capstone 3](https://github.com/darestack/devops-labs/tree/main/Module-2/capstone-project-3) | [MarketPeak_Ecommerce](https://github.com/darestack/MarketPeak_Ecommerce) | Keep as historical/manual deployment evidence. Do not pin unless it gets a clean README, current screenshots, and a reproducible setup |
| Git collaboration capstone | [devops-labs Capstone 1](https://github.com/darestack/devops-labs/tree/main/Module-1/capstone-project-1) | [greenwood-library-website](https://github.com/darestack/greenwood-library-website) | Keep as foundational Git workflow evidence. It is useful context, not a portfolio headline |
| Django + Terraform ECS lab | [django-dynamic-app](https://github.com/darestack/django-dynamic-app) | Module 4 Terraform notes | Keep public and unpinned until it has Terraform apply output, ECS task evidence, and an ALB screenshot |

## Evidence To Capture Next

| Project | Next Proof To Add |
|---|---|
| `glpi-ticketing-system` | Add `docs/screenshots/` with GLPI dashboard, sample ticket, asset inventory, SLA/reporting view, and a smoke-test command output |
| `github-actions-ec2-pipeline` | Capture EC2 `/api/health`, PM2 process status, and one rollback log with sensitive values hidden |
| `devops-labs` | Add a root screenshot index with the strongest 6-8 images, plus AWS teardown/cost notes for the HA WordPress capstone |
| `devops-labs` Capstone 6 | Promote Grafana/Gatus exports and sanitized Terraform plan/apply output into the capstone folder |
| `ecommerce-platform` | Add current app screenshots and deployment logs before treating it as a headline repo |
| `django-dynamic-app` | Add Terraform plan/apply evidence, ECS task screenshot, ALB response screenshot, and CloudWatch log screenshot |

## Public Repo Cleanup Notes

The profile should stay centered on five pinned repos. Supporting public repos are fine when they are honestly framed as labs or prototypes:

- `CommitVigil` and `cloudcull` should stay unpinned until their proof is stronger.
- `django-dynamic-app`, `book-to-podcast-ai`, and `warp-support-case-lab` can stay public as supporting work, but they should not compete with the main DevOps pins.
- Archived companion repos are still linkable as history, but they should not be treated as headline projects until their evidence is refreshed.
