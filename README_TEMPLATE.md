# High-Signal Project README Template

Use this structure for every pinned or recruiter-facing repository. Keep the top half readable in under 60 seconds.

## Project Name

> One sentence: what runs, where it runs, and what problem it solves.

Badges: use only badges that prove something real: CI, docs, container publish, coverage, security scan, or live endpoint. Avoid decorative badge walls.

## Problem

Describe the real operational problem in 2-4 sentences.

Good:
- "Manual EC2 deploys are slow and error-prone, so this project automates test, tag, release, deploy, rollback, and health checks."

Avoid:
- "Enterprise-grade scalable DevOps platform."
- "Production-ready system" unless there is a live deployment, runbook, monitoring, and hardening proof.

## Architecture

Show the flow first, then explain the pieces.

```text
Developer push
  -> GitHub Actions
  -> test/lint/security scan
  -> build artifact or image
  -> deploy target
  -> health check / rollback / alert
```

If the project has a diagram or screenshot, place it here and link to the source file.

## Tech Stack

| Tool | Purpose |
|---|---|
| GitHub Actions | CI/CD workflow orchestration |
| Docker | Repeatable local or deployment environment |
| AWS EC2 | Deployment target for the service |
| Prometheus/Grafana | Metrics collection and dashboarding |

Only include tools that are actually used in the repo. Remove tools that are planned but not implemented.

## What I Implemented

- Specific thing you built.
- Specific workflow, script, service, or configuration file.
- Specific failure case handled.
- Specific security or reliability decision.

Example:
- Added tag-triggered deploy workflow in `.github/workflows/release.yml`.
- Added `scripts/deploy.sh` rollback using timestamped releases and a `current` symlink.
- Added scheduled health check workflow that opens a GitHub Issue on failure.

## Evidence

| Evidence | Location | Status |
|---|---|---|
| CI workflow run | `Actions` tab or screenshot path | Required |
| Deployment log | `docs/assets/deploy-log.png` or linked run | Required for deployment projects |
| Dashboard screenshot | `docs/assets/grafana-dashboard.png` | Required for observability projects |
| Load-test result | `loadtests/results/latest-summary.json` | Use when claiming performance |
| Live endpoint | `https://.../health` | Optional; include only if stable |

Do not claim an impact metric unless this section proves it.

## Results

Use numbers only when measured.

Examples:
- "Deployment is reduced from manual SSH steps to one tag-triggered workflow."
- "Health check runs every 5 minutes and opens an issue when `/api/health` fails."
- "Local k6 smoke test summary is stored at `loadtests/results/latest-summary.json`."

Avoid:
- "Highly scalable."
- "Enterprise-grade."
- "Production-ready."
- "Battle-tested."

## How to Run

```bash
git clone https://github.com/darestack/<repo>.git
cd <repo>
<install command>
<test command>
<run command>
```

Include the health endpoint, dashboard URL, or test command that proves the project works.

## Operational Notes

Add the minimum runbook details a real teammate would need:

- Required environment variables or secrets.
- Deployment prerequisites.
- Rollback steps.
- Known failure modes.
- Where logs and metrics are available.

## Limitations

Be explicit. This builds trust.

Examples:
- "The staging and production deploy steps are simulated until a real target is attached."
- "The local demo uses SQLite; Docker Compose uses Postgres."
- "The dashboard screenshot is from a local environment."

## Challenges Solved

One short section with the most meaningful technical problem you solved and how.

## Recruiter Metadata

Suggested repository description:

> Short, evidence-based description with 1-2 role keywords.

Suggested topics:

`devops` `github-actions` `ci-cd` `aws` `docker` `linux` `monitoring`

## Final Credibility Checklist

- [ ] Top section is understandable in 30-60 seconds.
- [ ] Every tool listed has a clear purpose.
- [ ] Simulations are labeled as simulations.
- [ ] Screenshots/logs/metrics exist for the main claim.
- [ ] README grammar has been checked.
- [ ] No unproven words: "enterprise-grade", "production-ready", "highly scalable", "autonomous", "investor-grade", "standard".
