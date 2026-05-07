# GitHub Portfolio Audit - DevOps / Systems / Backend

Audit date: 2026-05-07

Scope: public GitHub profile `darestack`, current pinned repositories, and local checkouts under `/home/daretechie/DevProject/GitHub`.

## Executive Verdict

The portfolio has strong raw material, but the recruiter signal is diluted by too many unrelated repos, blank descriptions, tutorial forks, and a few over-claimed projects.

The winning path is a small profile centered on:

- one profile README as the entry point;
- 5 pinned repositories maximum;
- clear project descriptions;
- screenshots, workflow runs, logs, and measured outputs;
- honest labels for labs and simulated deployments.
- deletion or archiving of repos that do not directly support DevOps, IT systems, or backend infrastructure roles.

## Current Credibility Risks

| Risk | Why It Hurts | Fix |
|---|---|---|
| `cloudcull` is pinned and over-claims heavily | Phrases like "Investor-Grade", "standard for multi-cloud cost optimization", "Sniper Agent", and "Kill-Switch" read like marketing without proof | Unpin now. Rewrite as a cost-audit CLI only if real cloud scans, IAM policy, dry-run output, and screenshots exist |
| `CommitVigil` is pinned with blank repo description | README says GitHub webhook risk monitor, but code inspected locally looks closer to commitment/agent/reporting workflows | Unpin until README, code, tests, and description match one clear product |
| `github-actions-ec2-pipeline` had thousands of duplicate open health-check issues | A health check that spams issues looks operationally unsafe, even if the pipeline idea is good | Deduplicate alert issue creation, reduce schedule noise, and close historical duplicate issues after GitHub API rate limit resets |
| Several project READMEs use "production" language without production evidence | Senior reviewers look for deployment logs, uptime, runbooks, monitoring, and failure handling | Replace broad claims with exact implementation details and evidence |
| `advanced-actions-demo` claims OIDC AWS deploy, but local workflow shows a placeholder deploy with `id-token: write` commented out | This is the kind of mismatch a technical screener notices quickly | Move to IMPROVE; implement real OIDC or describe it as a workflow-pattern lab |
| `github-actions-cicd-demo` README and workflow disagree | README says Node 12/14/16 and hard lint gate; workflow uses Node 18/20 and SARIF lint upload has `continue-on-error: true` | Update README to match workflow, or change workflow and prove it |
| Too many public repos compete for attention | Recruiters scan pins and recent repos first; unrelated AI/product/course repos blur the DevOps story | Archive, private, or leave unpinned; do not link from profile README |

## Recommended Pinned Repositories

Pin 5. Do not force a weak 6th pin.

| Rank | Repository | Purpose | Action |
|---|---|---|---|
| 1 | `api-reliability-suite` | Backend reliability, observability, auth, rate limiting, readiness checks | KEEP; add more result metrics and keep README modest |
| 2 | `github-actions-ec2-pipeline` | Real release automation to EC2 with rollback and health checks | KEEP; add deployment screenshots and workflow run links |
| 3 | `github-actions-cicd-demo` | CI/CD quality gates, Trivy SARIF, Docker Buildx, GHCR | KEEP after README correction; label deploy stage as simulated |
| 4 | `glpi-ticketing-system` | IT support / systems operations proof | KEEP; add GLPI screenshots and sample tickets/assets |
| 5 | `devops-labs` | Breadth across Linux, AWS, Docker, Kubernetes, Terraform, Ansible, monitoring | KEEP as lab index; promote only capstones in profile |

Optional 6th pin only after fixing:

- `advanced-actions-demo` after real OIDC is implemented; or
- a new focused `terraform-aws-observability-stack` repo extracted from `devops-labs`.

Unpin now:

- `cloudcull`
- `CommitVigil`

## Suggested Repo Names and Descriptions

Use these descriptions in GitHub repository settings.

| Current Repo | Suggested Name | Suggested Description |
|---|---|---|
| `api-reliability-suite` | keep | FastAPI reliability reference with JWT auth, rate limiting, readiness checks, Prometheus/Grafana/Jaeger, circuit-breaker fallback, and tested LLM log triage. |
| `github-actions-ec2-pipeline` | keep or `ec2-release-pipeline` | GitHub Actions pipeline for a Node/Express app: test, tag, deploy to EC2 via SSH/PM2, rollback with atomic symlinks, and scheduled health checks. |
| `github-actions-cicd-demo` | `github-actions-container-pipeline` | Node.js CI/CD lab using GitHub Actions matrix tests, ESLint, Trivy SARIF, Docker Buildx, GHCR publishing, and simulated staged deploys. |
| `glpi-ticketing-system` | `docker-glpi-helpdesk-lab` | Dockerized GLPI helpdesk lab with MariaDB, persistent volumes, SLA categories, user roles, and asset workflow notes. |
| `devops-labs` | keep | Indexed DevOps lab portfolio covering Linux, AWS, Docker, Kubernetes, Terraform, Ansible, Prometheus, Grafana, and capstone infrastructure builds. |
| `advanced-actions-demo` | `github-actions-oidc-lab` after fix | GitHub Actions workflow-pattern lab with reusable workflows, Node matrix tests, environment-gated deploys, and real AWS OIDC role assumption. |
| `CommitVigil` | `commit-risk-webhook` only after rewrite | FastAPI webhook service that validates GitHub events, scans commit risk signals, queues background checks, and sends Slack alerts. |
| `cloudcull` | `cloud-cost-audit-cli` only after rewrite | CLI-first cloud cost audit tool with dry-run reports, provider adapters, and safe remediation notes. |

## Keep / Improve / Archive

## Remote-Only Repository Policy

Several repositories exist on GitHub but are not cloned under `/home/daretechie/DevProject/GitHub`. Do not judge the portfolio from local folders alone.

For remote-only repos:

- clone only repos that can improve interview probability;
- create an issue before larger cleanup work;
- use a branch and PR for each repo change;
- avoid spending time on tutorial forks, old training repos, or unrelated experiments unless they have deployment evidence.

Remote-only repos worth inspecting first:

| Repo | Status | Why |
|---|---|
| `book-to-podcast-ai` | IMPROVE | Has Railway deployment records, so it can serve as backend/app deployment proof after README cleanup |
| `django-dynamic-app` | IMPROVE | Has Django, Docker, and Terraform/ECS material; useful only if described as a lab until deployment evidence is added |
| `policycraft-ai` | IMPROVE LOW PRIORITY | Data-app export with broken hosted link; useful only if packaged as a reproducible Python/Dash project |
| `jenkins-scm` | DELETE OR ARCHIVE | One README only, typo in description, no Jenkinsfile, no pipeline evidence |

## Delete / Archive Queue

Use this as the removal queue before touching GitHub settings. The goal is not to keep every learning artifact; the goal is to make the public profile look intentional.

### Delete Now If You Do Not Need The History

These are the clearest permanent-delete candidates because they are empty, tiny, duplicated, forked tutorial work, or old beginner training that does not increase interview probability.

Empty or tiny practice repos:

- `git_test`
- `zero_day`
- `m3l2_forking_lab`
- `m4l1_managing_a_project`
- `warp-dummy`
- `jenkins-scm` unless it is rebuilt from scratch as a Jenkins pipeline lab

Old beginner/course repos:

- `alx-zero_day`
- `alxPreCourse`
- `alx-low_level_programming`
- `DataStructure_and_Algo-Python`
- `IntroToPython_Deitel`
- `FSND_Udacity`
- `LittleLemon`
- `odin-recipes`
- `playing-with-css-flexbox`
- `sentiment_analyzer_flask`

Forks and tutorial copies:

- `30-Days-Of-JavaScript`
- `ai-dev-tasks`
- `build-your-own-x`
- `css-exercises`
- `example-voting-app`
- `fullstack-ecommerce`
- `gayolGate`
- `gitops-argocd`
- `holberton-system_engineering-devops`
- `html-css-js-portfolio-tutorial-2`
- `langchain`
- `linux-basics-course`
- `one-off-resources`
- `portfolio-template`
- `python-extensions-static-site-generator`
- `python-static-site-generator`
- `ruff`
- `shell-scripting-for-beginners-course`
- `wells-fargo-task-2`
- `Your-First-Contribution`

### Archive First, Delete Later If No Evidence Exists

These may contain personal work, but they currently distract from the target roles unless they have deployments, tests, or infrastructure proof.

- `agentproof`
- `ai-startup-website`
- `customer-service-chatbot`
- `CustomerAgent`
- `football-players-perfomance-analyses`
- `gen_ai`
- `image_detection`
- `LangExpert`
- `pic-gen`
- `clinician`
- `medicalrag`
- `verimed`

### Do Not Delete Yet

These either support the current portfolio directly or may be useful after cleanup.

- `darestack`
- `api-reliability-suite`
- `github-actions-ec2-pipeline`
- `github-actions-cicd-demo`
- `glpi-ticketing-system`
- `devops-labs`
- `advanced-actions-demo`
- `book-to-podcast-ai`
- `django-dynamic-app`
- `policycraft-ai`
- `CommitVigil`
- `cloudcull`
- `100-days-of-devops-xfusioncorp`
- `warp-support-case-lab`
- `greenwood-library-website`
- `MarketPeak_Ecommerce`
- `ecommerce-platform`

### KEEP

These can support DevOps, systems, or backend roles.

| Repo | Why It Stays | Required Evidence |
|---|---|---|
| `api-reliability-suite` | Strong backend + observability signal | CI run, Grafana screenshot, load-test summary, docs link |
| `github-actions-ec2-pipeline` | Strong CI/CD and deployment signal | Successful workflow run, EC2 health endpoint screenshot, rollback log |
| `github-actions-cicd-demo` | Strong pipeline-quality signal if wording is fixed | Actions run, SARIF screenshot, GHCR package link |
| `glpi-ticketing-system` | Clear IT support / systems signal | GLPI dashboard screenshots, sample ticket workflow, SLA config screenshots |
| `devops-labs` | Good breadth and capstone index | Capstone screenshots, architecture diagrams, cost notes |

### IMPROVE

These may be useful later, but should not lead the profile today.

| Repo | Problem | Fix |
|---|---|---|
| `advanced-actions-demo` | Claims OIDC/AWS but deploy workflow is placeholder | Implement real OIDC trust policy and AWS action, or rewrite as placeholder pattern lab |
| `CommitVigil` | README and code direction are not aligned; repo description is blank | Decide one product: GitHub risk webhook or commitment extractor. Delete or move unrelated agent/sales features |
| `cloudcull` | Over-marketed and too broad for current proof | Rewrite as a dry-run cost audit CLI; remove multi-cloud/AI/kill-switch claims unless demonstrated |
| `100-days-of-devops-xfusioncorp` | Curriculum repo can show consistency but is not high-signal enough to pin | Keep public, but link only from `devops-labs` if organized |
| `jenkins-scm` | Title/description feels beginner-level and repo contains only a README | Delete/archive unless you want to rebuild a full Jenkinsfile lab |
| `warp-support-case-lab` | Useful troubleshooting angle, but not central to DevOps hiring scan | Keep unpinned; add incident format, logs, root cause, resolution |
| `book-to-podcast-ai` | App is outside the main DevOps track, but it has real Railway deployment records | Keep unpinned; reposition as backend/app deployment proof with Railway deployment dates, live URL, runtime config, and screenshots |
| `medicalrag`, `verimed`, `clinician` | Backend/AI healthcare work may distract from DevOps unless deployed and documented | Move to backend section only if live, tested, and infrastructure is clear |
| `ecommerce-platform`, `MarketPeak_Ecommerce`, `greenwood-library-website` | Frontend/e-commerce work is not aligned with the target roles | Keep unpinned; use only if demonstrating deployment pipeline |

### ARCHIVE OR HIDE FROM RECRUITER VIEW

These do not directly increase interview probability for DevOps, IT systems, or backend infrastructure roles.

Training / beginner repos:

- `alx-low_level_programming`
- `alx-zero_day`
- `alxPreCourse`
- `zero_day`
- `DataStructure_and_Algo-Python`
- `IntroToPython_Deitel`
- `FSND_Udacity`
- `LittleLemon`
- `odin-recipes`
- `playing-with-css-flexbox`
- `git_test`
- `Dev`
- `sentiment_analyzer_flask`

Forks and external tutorials:

- `30-Days-Of-JavaScript`
- `build-your-own-x`
- `css-exercises`
- `example-voting-app`
- `fullstack-ecommerce`
- `gitops-argocd`
- `holberton-system_engineering-devops`
- `html-css-js-portfolio-tutorial-2`
- `linux-basics-course`
- `m3l2_forking_lab`
- `m4l1_managing_a_project`
- `portfolio-template`
- `python-extensions-static-site-generator`
- `python-static-site-generator`
- `shell-scripting-for-beginners-course`
- `wells-fargo-task-2`
- `Your-First-Contribution`

Low-alignment product experiments unless they have strong deployment evidence:

- `ai-startup-website`
- `customer-service-chatbot`
- `CustomerAgent`
- `gen_ai`
- `image_detection`
- `LangExpert`
- `pic-gen`
- `agentproof`

Already archived or safe to keep out of view:

- `bank-prompt-chain`
- `CollabCrate`
- `hello-devops`
- `it-lab-portfolio`
- `kenya-clinical-challenge`
- `kubernetes-hotel-guide`
- `modai-app`
- `my-dev-to-posts`
- `node-ci-demo`
- `warp-dummy`

## Before vs After - Key Projects

### `api-reliability-suite`

Before:

- "Backend + DevOps + AI reliability template" is mostly fine, but "production backend patterns" can sound broad.
- The README is strong, but it should keep emphasizing scope boundaries.

After:

- "FastAPI reliability reference with JWT auth, rate limiting, readiness checks, Prometheus/Grafana/Jaeger, circuit-breaker fallback, and tested LLM log triage."

Why this is better:

- It lists reviewable capabilities instead of implying full production readiness.

Evidence to add:

- Screenshot of Grafana dashboard.
- Latest CI run link.
- `loadtests/results/latest-summary.json`.
- Screenshot or log from `/ready`, `/slo/report`, and a circuit-breaker fallback case.

### `github-actions-ec2-pipeline`

Before:

- "Zero manual steps" and "zero-downtime deploy" are strong claims.

After:

- "GitHub Actions tests, tags, and deploys a Node/Express app to EC2 using SSH, PM2 reload, timestamped releases, rollback script, and scheduled health checks."

Why this is better:

- It explains the implementation without claiming uptime that has not been measured.

Evidence to add:

- Successful `release.yml` run screenshot.
- EC2 `/api/health` screenshot.
- PM2 status screenshot.
- Rollback log from a failed deploy test.
- Continue closing historical duplicate `Application Health Check Failed` issues after the GitHub API rate limit resets. Cleanup reduced the count from 5,506 to at least 1,036 before rate limiting.

### `github-actions-cicd-demo`

Before:

- README says Node 12/14/16, but workflow uses Node 18/20.
- README implies hard lint gate, but the SARIF lint upload step has `continue-on-error: true`.
- README says staged deploy, but workflow deploy steps are simulated.

After:

- "Node.js CI/CD lab using GitHub Actions matrix tests on Node 18/20, ESLint, Trivy SARIF, Docker Buildx, GHCR image publishing, and simulated staged deploy steps."

Why this is better:

- It prevents a senior engineer from finding a mismatch between README and workflow.

Evidence to add:

- Actions run screenshot.
- GHCR package link.
- GitHub Code Scanning screenshot.
- If deploying for real, replace simulation echoes with actual deploy commands and logs.

### `glpi-ticketing-system`

Before:

- "Enterprise IT support system" may overstate a Docker Compose lab.

After:

- "Dockerized GLPI helpdesk lab with MariaDB, persistent volumes, SLA categories, user roles, and asset workflow notes."

Why this is better:

- It shows IT systems skill without pretending the lab is an enterprise deployment.

Evidence to add:

- GLPI login/dashboard screenshot.
- Asset inventory screenshot.
- Sample P1/P2/P3 ticket screenshots.
- Screenshot showing MariaDB is not exposed publicly.

### `devops-labs`

Before:

- "59 hands-on projects" shows breadth, but recruiters may not dig into 59 folders.
- "Production-grade capstone" is stronger than the evidence visible in the root README.

After:

- "DevOps lab index with three highlighted capstones: AWS HA WordPress, e-commerce CI/CD, and Terraform plus observability."

Why this is better:

- It turns a large curriculum repo into a curated evidence map.

Evidence to add:

- Root README links to the 3 best capstone screenshots.
- Architecture diagrams for each capstone.
- Cost estimate or teardown note for AWS labs.
- Terraform plan/apply screenshot with sensitive values hidden.

### `advanced-actions-demo`

Before:

- Claims OIDC AWS auth, least-privilege IAM, and EC2 deploy.
- Local workflow currently has `id-token: write` commented out and says "Deploy (Placeholder)".

After:

- Option A: implement real OIDC and keep the repo.
- Option B: rewrite as "GitHub Actions workflow patterns: reusable workflows, Node matrix tests, and environment-gated placeholder deploy."

Why this is better:

- It removes the fastest credibility failure in the current portfolio.

Evidence to add:

- IAM trust policy snippet.
- `aws-actions/configure-aws-credentials@v4` in workflow.
- Successful workflow run with AWS account ID masked.

### `book-to-podcast-ai`

Before:

- Treated as a low-alignment product experiment.
- Deployment proof was unclear because it was initially remembered as Render.

After:

- "Flask app that converts uploaded books into podcast-style audio; deployed to Railway with production deployment records."

Why this is better:

- It uses the real platform and keeps the project in a modest backend/app-deployment lane instead of pretending it is a DevOps centerpiece.

Evidence found:

- GitHub deployment records show Railway production deployments.
- First production deployment found: March 27, 2025 at 07:18 UTC.
- Latest production deployment found: May 18, 2025 at 20:22 UTC, updated May 18, 2025 at 21:37 UTC.

Evidence to add:

- Railway live URL or screenshot.
- Deployment settings screenshot with sensitive values hidden.
- Runtime/start command and environment variable notes.
- A short README section: "Deployment: Railway".
- Health check or manual smoke-test screenshot after deploy.

### `CommitVigil`

Before:

- README describes a GitHub webhook listener for risky commits.
- Local code includes commitment extraction, agents, reports, sales docs, and broader product behavior.

After:

- Pick one story:
  - "GitHub commit-risk webhook service"; or
  - "AI commitment extraction and reporting service."

Why this is better:

- One clear problem beats a pile of clever features.

Evidence to add:

- Webhook payload fixture.
- HMAC validation test.
- Slack alert screenshot.
- Background worker log.
- Remove unrelated modules from the recruiter path.

### `cloudcull`

Before:

- Heavy marketing: "autonomous", "Investor-Grade", "standard", "Sniper", "Kill-Switch".
- Multi-cloud + AI + Terraform remediation is a very large claim.

After:

- "Cloud cost audit CLI that scans configured provider data, produces a dry-run waste report, and writes a remediation manifest for manual review."

Why this is better:

- Cost control is credible when it starts with dry-run evidence and safe review.

Evidence to add:

- Redacted cloud inventory fixture.
- Dry-run report screenshot.
- IAM permission policy.
- Unit tests for no-delete-by-default behavior.
- Real cost estimate calculation.

## Missing Critical Projects

Highest-value additions for DevOps and IT roles:

| Missing Project | Why It Helps | Keep It Simple |
|---|---|---|
| `terraform-aws-observability-stack` | Direct Terraform/AWS/monitoring proof | One VPC, one EC2, security group, S3 remote state, DynamoDB lock, Node Exporter, Prometheus/Grafana screenshots |
| `linux-incident-response-lab` | Strong IT support and systems troubleshooting signal | 3 incidents: disk full, failed service, SSH auth issue. Include commands, logs, root cause, and fix |
| `backup-restore-runbook` | Practical operations credibility | Dockerized app + Postgres backup + restore drill + verification screenshot |
| `kubernetes-deployment-lab` | Kubernetes keyword proof | Only do this if it has real manifests, probes, resources, rollout/rollback, and screenshots. No fake microservices |

Do not add Kubernetes just to look advanced. A clean Docker + EC2 + monitoring deployment is more credible than artificial Kubernetes complexity.

## Grammar and Metadata Fixes

| Repo | Issue | Fix |
|---|---|---|
| `bank-prompt-chain` | "utlines" | "outlines" |
| `football-players-perfomance-analyses` | "perfomance" and awkward plural | "football-player-performance-analysis" |
| `jenkins-scm` | "Jenkin" | "Jenkins" |
| `linux-basics-course` | "Learn Linux fundamental." | "Linux fundamentals course notes." |
| `github-actions-ec2-pipeline` | Blank description | Add suggested description above |
| `CommitVigil` | Blank description | Add only after product story is corrected |
| `cloudcull` | Blank description and over-marketed README | Unpin or rewrite before adding description |
| `glpi-ticketing-system` | Generic description | Use suggested description above |

## Keyword Strategy

Use keywords naturally in repo names, descriptions, and README headings:

- DevOps Engineer
- Backend Engineer
- CI/CD
- GitHub Actions
- AWS
- EC2
- Terraform
- Docker
- Kubernetes
- Monitoring
- Prometheus
- Grafana
- Linux
- System Administration
- IT Support
- Incident Response

Do not stuff every keyword into every repo. Each pinned repo should own one capability.

## 7-Day Action Plan

1. Update profile README with the new hub copy.
2. Pin only the recommended 5 repos.
3. Add GitHub descriptions from the table above.
4. Fix `github-actions-cicd-demo` README/workflow mismatch.
5. Rewrite or unpin `advanced-actions-demo`.
6. Add screenshots to `api-reliability-suite`, `github-actions-ec2-pipeline`, and `glpi-ticketing-system`.
7. Archive or hide the listed low-signal repos from the recruiter path.

## Final Rule

Anything that cannot be verified in 5 minutes should not be a headline claim.
