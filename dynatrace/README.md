**Here's a comprehensive, hands-on quick-start lab for Dynatrace monitoring.** This guide gets you from zero to observing real data in under 30-60 minutes (plus any deployment time). It covers the official recommended path using free resources.

### Step 1: Sign Up and Explore the Playground (No Installation Needed, 5-10 mins)
Dynatrace provides a **public Playground** (sandbox) with sample data from real applications, Kubernetes clusters, etc. Perfect for immediate exploration.

1. Go to [https://www.dynatrace.com/signup/playground/](https://www.dynatrace.com/signup/playground/) and sign up (business email, no credit card).
2. Log into the Playground tenant (example: wkf10640.apps.dynatrace.com).

**Key things to explore first:**
- **Dashboards** (pre-built examples): Getting Started, K8s Cluster Overview, EasyTrade app, etc.
- **Notebooks** (interactive analysis): Getting Started Notebook, Log analysis, etc.
- **Hands-on Tutorial Notebooks** (step-by-step):
  - Distributed Trace & Database Diagnostics
  - Analyze Infrastructure
  - Kubernetes Clusters & Workloads
  - Davis-detected Problems (AI root cause)
  - Application Security
  - Synthetic Tests, Logs, DORA Metrics, Ownership, etc.
- Apps: Problems (Davis AI), Kubernetes, Services, Distributed Traces, Application Security, SLOs, Synthetics, Session Replay.

**Tip:** Use the left menu to navigate: **Observe & explore** > **Kubernetes**, **Services**, **Problems**, etc. This shows full-stack observability (hosts, containers, services, traces, logs, metrics, user experience, security) in one platform.

### Step 2: Start Your Own Free Trial (15 Days, No Credit Card)
1. Go to [https://www.dynatrace.com/signup/](https://www.dynatrace.com/signup/) or [https://www.dynatrace.com/try-free/](https://www.dynatrace.com/try-free/).
2. Create your tenant. You'll get your own environment immediately.

### Step 3: Ingest Data – Install OneAgent (Core of Dynatrace Monitoring)
OneAgent is a single agent for **automatic, deep observability** (auto-discovery, code-level tracing, logs, metrics, etc.).

#### Quick Options:
- **Easiest: Single Host/VM (Linux/Windows)** — Go to **Deployment status** or **Install OneAgent** in the UI. Download the installer, run the one-liner command.
- **Kubernetes (Recommended for modern apps)**:
  - Use **Dynatrace Operator** (quickstart in <1 minute).
  - In UI: **Kubernetes** > **Add cluster** > Follow wizard (select distribution like EKS, GKE, etc., download `dynakube.yaml`, apply with `kubectl`).
- **Cloud**: Enable AWS, Azure, GCP integrations directly from the UI.
- **Other**: OpenTelemetry, Prometheus, logs ingestion, 600+ Hub extensions.

Data starts flowing automatically. Check **Deployment status** for coverage.

### Step 4: Analyze Your Data (Core Skills)
Once data ingests:
1. **Smartscape** — Visualize full topology (hosts → processes → services → databases).
2. **Services App** — See response times, throughput, errors, dependencies.
3. **Problems App** — Let Davis AI detect issues and provide root-cause analysis.
4. **Distributed Traces** (PurePath) — End-to-end traces with code-level details.
5. **Kubernetes App** — Cluster, namespace, workload views.
6. **Dashboards & Notebooks** — Build custom views or use Notebooks for ad-hoc queries (Grail + DQL).
7. **Logs, Metrics, Events** — Unified analysis.
8. **Application Security** — Runtime vulnerabilities.

**Pro Tip:** Follow the tutorial Notebooks from the Playground in your own tenant for guided diagnostics.

### Step 5: Next-Level Features (Automation & Extension)
- **Alerts & Notifications** — Set up problem notifications (email, Slack, PagerDuty, etc.).
- **SLOs** — Define Service Level Objectives.
- **Workflows** — Automate responses.
- **Extensions & Apps** — Extend via Dynatrace Hub or build custom apps.
- **Configuration as Code** — Manage via API or Git.

### Recommended Resources for Deeper Hands-On
- **GitHub Lab Repo** (highly recommended): [dynatrace-perfclinics/dynatrace-getting-started](https://github.com/dynatrace-perfclinics/dynatrace-getting-started) — Includes demo apps, dashboards, workflows, and detailed readmes.
- Official Docs: [Get Started](https://docs.dynatrace.com/docs/discover-dynatrace/get-started).
- Dynatrace University (free courses).
- YouTube: Search "Dynatrace Zero to Hero" or official tutorials.
- Dynatrace Community for questions.

### Common Quick-Win Scenarios to Practice
- Deploy a sample app (e.g., EasyTrade from the repo) on Kubernetes.
- Simulate load and watch Davis AI find root causes.
- Analyze a slow database call via PurePath.
- Set up a synthetic monitor for an endpoint.
- Create a custom dashboard for your team.

This lab gives you production-grade monitoring foundations quickly. Dynatrace's strength is **automation + AI (Davis)** — minimal manual configuration for deep insights.

If you have a specific environment (AWS EKS, Azure, Java/.NET app, etc.), let me know for tailored commands! Start with the Playground today.
