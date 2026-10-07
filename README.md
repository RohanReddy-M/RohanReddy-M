# Rohan Reddy M

**Cloud engineer · data & decision science**

I build systems end to end: analytics pipelines that turn raw data into decisions a business can act on, and cloud platforms with AI-powered incident response, from Terraform provisioning up.

---

## Olist Retention Radar

**[github.com/RohanReddy-M/olist-churn-llm-insights](https://github.com/RohanReddy-M/olist-churn-llm-insights)** · [live dashboard](https://rohanreddy-m.github.io/olist-churn-llm-insights/)

Which of 57,143 existing e-commerce customers will buy again, what drives it, and where the retention budget should go. Built on 99,441 real orders.

- SQL star-schema feature layer with automated leakage tests; logistic regression chosen over random forest on cross-validated PR-AUC; calibrated probabilities; SHAP drivers
- Top decile beats random targeting **2.3×** in-time and **1.7×** on a later period the model never saw
- A/B test sized on the real segment before running anything; 20 dated entries in a decision log
- Claude API drafts the stakeholder read-out, and code checks every figure it cites

**[Automated weekly sales report](https://github.com/RohanReddy-M/weekly-report-automation)** · SQLite to a two-page PDF with week-on-week trends, z-score anomaly flags and an audit trail of every cleaning step, in about 5 seconds.

---

## ObserveOps

**[github.com/RohanReddy-M/observeops](https://github.com/RohanReddy-M/observeops)** · [run it locally](https://github.com/RohanReddy-M/observeops#run-it-locally)

Production-grade cloud platform on AWS with automated incident response. When a service fails:

1. AlertManager detects it in about a minute (measured: 60-90s, tuned to avoid paging for a self-healed blip)
2. Loki pulls the last 50 log lines automatically
3. LLM finds the root cause
4. Slack gets the fix command in **~3 seconds** — no human involved

**Cloud infrastructure:** Terraform IaC (VPC, EC2, ALB, Route53, DynamoDB, Lambda, EventBridge, SSM) · private subnets · IMDSv2 · least-privilege IAM · OIDC for CI/CD (zero static credentials)

**Platform:** Kubernetes + ArgoCD GitOps · GitHub Actions · Docker · nginx · OpenTelemetry

**Observability:** Prometheus · Grafana (5 dashboards) · Loki · AlertManager · Tempo · SLOs + error budgets · DORA metrics

**AI layer:** LangGraph RAG agent · FAISS · Groq · CloudTrail security alerting via Lambda

---

## Stack

`Python` `SQL` `pandas` `scikit-learn` `SHAP` `statistics` `A/B testing`  
`AWS` `Terraform` `Kubernetes` `ArgoCD` `Docker` `GitHub Actions` `FastAPI` `Flask`  
`Prometheus` `Grafana` `Loki` `AlertManager` `OpenTelemetry` `LangGraph` `FAISS` `nginx`

---

machireddy23@gmail.com
