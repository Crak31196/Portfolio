# Portfolio Breakdown by Service Type

Each service line below maps to one flagship project. Every repo ships as a real, runnable MVP: working infrastructure code or a working stack, automated tests, a GitHub Actions CI workflow, and a client-facing README. Sample data, demo workloads, and any performance numbers are explicitly labeled as demo/illustrative — nothing here claims a real client outcome.

---

## 1. Kubernetes Migration & Container Platform Setup

**Project:** [EKS Migration & Helm Deployment Toolkit](https://github.com/Crak31196/eks-migration-toolkit)

**Problem it solves:** "We're running Kubernetes ourselves on raw EC2 instances. It's fragile, hard to scale, and nobody's sure it's secure."

**What it demonstrates:**

- Terraform modules for a production-shaped AWS EKS cluster (VPC, managed node groups, IRSA/OIDC)
- Terraform native tests run against a mocked AWS provider (no cloud credentials required to validate)
- A Helm chart with autoscaling, resource limits, and health probes for deploying workloads onto the cluster
- A migration-readiness audit script that scans existing Kubernetes manifests for EKS-incompatible patterns

**Resume skills proven:** AWS, Kubernetes (CKA), Terraform, Helm, Docker — mirrors a real production EC2 → EKS migration.

---

## 2. Infrastructure-as-Code & Cloud Security Baselines

**Project:** [Multi-Cloud Terraform Landing Zone](https://github.com/Crak31196/terraform-multicloud-landing-zone)

**Problem it solves:** "We just created our AWS/Azure account and have no idea what a secure baseline even looks like."

**What it demonstrates:**

- Reusable Terraform modules for both AWS (VPC, IAM baseline, KMS, budget guardrails) and Azure (VNet, RBAC baseline, Key Vault, WAF policy)
- Governance patterns (AWS Config rules, Azure Policy assignments) and cost-guardrail automation
- Terraform native tests against mocked AWS and Azure providers

**Resume skills proven:** AWS & Azure, Terraform, Azure WAF, KMS/Key Vault secrets management, Azure Solutions Architect Expert certification.

---

## 3. CI/CD Pipeline Engineering & DevSecOps

**Project:** [CI/CD Pipeline Accelerator with Security Gates](https://github.com/Crak31196/cicd-pipeline-accelerator)

**Problem it solves:** "Our pipeline takes forever, and we're not scanning our images for vulnerabilities before they ship."

**What it demonstrates:**

- Side-by-side naive vs. parallelized GitLab CI pipelines (DAG `needs:`, parallel jobs) plus an equivalent Jenkins declarative pipeline
- Working Trivy and Grype vulnerability scan scripts run against a real built container image
- Reference configs for SonarQube and KubeBench as pipeline stages

**Resume skills proven:** Jenkins, GitLab CI, Docker, Trivy, Grype, SonarQube, KubeBench, CKS — mirrors a real ~1-hour pipeline runtime reduction through parallelization.

---

## 4. Observability, Alerting & Incident Response

**Project:** [Kubernetes Observability & Alerting Stack](https://github.com/Crak31196/k8s-observability-stack)

**Problem it solves:** "We find out about outages from our customers, not our monitoring — and we have no consistent incident process."

**What it demonstrates:**

- A one-command Prometheus/Grafana/Alertmanager stack (Docker Compose) with dashboards and alert rules defined as code
- SLA-style alert rules (error rate, latency, target down) with a working end-to-end smoke test
- RCA runbook templates and an automated remediation script pattern for recurring maintenance tasks

**Resume skills proven:** Prometheus, Grafana, Splunk/Graylog-style logging, Kubernetes alert handling, SLA management, RCA, automated cron-based maintenance.

---

## Full Project Index

| Project | Repo |
|---|---|
| EKS Migration & Helm Deployment Toolkit | [Crak31196/eks-migration-toolkit](https://github.com/Crak31196/eks-migration-toolkit) |
| Multi-Cloud Terraform Landing Zone | [Crak31196/terraform-multicloud-landing-zone](https://github.com/Crak31196/terraform-multicloud-landing-zone) |
| CI/CD Pipeline Accelerator with Security Gates | [Crak31196/cicd-pipeline-accelerator](https://github.com/Crak31196/cicd-pipeline-accelerator) |
| Kubernetes Observability & Alerting Stack | [Crak31196/k8s-observability-stack](https://github.com/Crak31196/k8s-observability-stack) |

Back to [README.md](./README.md).
