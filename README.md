# Hi, I'm Shahid Khaleel 👋

[![LinkedIn](https://img.shields.io/badge/LinkedIn-shahidkhaleel78-0A66C2?logo=linkedin&logoColor=white)](https://www.linkedin.com/in/shahidkhaleel78/)

Senior DevOps Engineer building real, working cloud-native infrastructure — **IaC**, **Kubernetes**, **service mesh**, **cloud infrastructure**, **GitOps**, **identity & security**, **CI/CD**, **observability**, and **MLOps**. Every repository ships source code, infrastructure definitions, deployment workflows, and architecture docs — plus the trade-offs, debugging, and challenges I actually hit, not a polished-outcomes-only highlight reel.

---

## 🏆 Start here — 4 projects that show the range

<table>
<tr><td width="50%" valign="top">

### [payment-platform](https://github.com/shahid-khaleel/payment-platform)
19 microservices — auth, wallet, settlement, fraud detection, webhooks — with per-service Helm charts, Kustomize overlays, contract tests, load tests, dependency scanning, and incident runbooks. The largest and most operationally mature project here.

</td><td width="50%" valign="top">

### [observability](https://github.com/shahid-khaleel/observability)
5 services, 5 observability planes, verified end-to-end on Istio: STRICT mTLS, RED metrics, one real distributed trace with correct parent-child spans across every service, and an EFK pipeline splitting routine logs from a compliance audit index.

</td></tr>
<tr><td width="50%" valign="top">

### [istio](https://github.com/shahid-khaleel/istio)
Root-caused a bug in Python's OpenTelemetry auto-instrumentation that was silently splitting every trace in two — full Istio + Jaeger + Kiali stack on Bookinfo, fix documented step by step in a runbook.

</td><td width="50%" valign="top">

### [ebpf-observability](https://github.com/shahid-khaleel/ebpf-observability)
Kernel-level observability with **zero application instrumentation** — Cilium/Hubble + Tetragon watching network connections, process creation, file access, and syscalls, plus a threat-intel alerting pipeline and Kyverno admission control.

</td></tr>
</table>

---

## 📂 Everything else, by track

17 more repositories across Cloud Infrastructure, Kubernetes Platform, Service Mesh, GitOps, and MLOps.

### ☁️ Cloud Infrastructure & IaC
| Repo | Focus |
|---|---|
| [terraform](https://github.com/shahid-khaleel/terraform) | Modular EKS + KMS provisioning (community-module-based), environment-scoped (`qa`) |
| [eks-deployment](https://github.com/shahid-khaleel/eks-deployment) | Standalone EKS + IRSA + Cluster Autoscaler + AWS Load Balancer Controller reference build, plus a secondary-IP automation script |
| [ansible](https://github.com/shahid-khaleel/ansible) | Role-based provisioning (Apache, Docker, Java, Keycloak, MySQL, MongoDB, Node.js, Redis) with a GitLab CI deploy pipeline |
| [helm](https://github.com/shahid-khaleel/helm) | A Helm chart + CI scripting for deploying a Spring Boot app to EKS via an S3-backed chart repository |

### ⎈ Kubernetes Platform & Security
| Repo | Focus |
|---|---|
| [kubernetes](https://github.com/shahid-khaleel/kubernetes) | A collection of focused K8s operator demos: ConfigMap hot-reload, EFS CSI storage, IRSA for S3 access, the API request lifecycle (Kyverno + Kustomize), MySQL StatefulSet replication, and a full Jenkins → SonarQube → Docker → Minikube CI/CD pipeline built end-to-end |
| [kubernetes-security-documentation](https://github.com/shahid-khaleel/kubernetes-security-documentation) | A curated ~150-topic personal knowledge base spanning Linux, Docker, and Kubernetes security fundamentals |
| [kubernetes-fds](https://github.com/shahid-khaleel/kubernetes-fds) | A Kubernetes file-descriptor-exhaustion failure-mode simulator, paired with a Grafana dashboard to observe it |

### 🔐 Service Mesh, Identity & Secrets
| Repo | Focus |
|---|---|
| [istio-service-mesh](https://github.com/shahid-khaleel/istio-service-mesh) | Istio service mesh capabilities on two demo microservices: strict mTLS, ingress gateway routing, canary traffic splitting, fault injection, and circuit breaking |
| [keycloak-auth-apache](https://github.com/shahid-khaleel/keycloak-auth-apache) | Keycloak-based auth behind an Apache reverse proxy, with an evolution across branches toward a full Kubernetes + Istio + observability deployment |
| [k8s-auth-keycloak](https://github.com/shahid-khaleel/k8s-auth-keycloak) | Kubernetes-native OIDC authentication via Keycloak, deployable via raw manifests, Helm, or Docker Compose |
| [hashicorp-vault-project](https://github.com/shahid-khaleel/hashicorp-vault-project) | Vault secrets management implemented twice independently (Python/Flask and Java/Spring Boot), covering AppRole auth, KV v2, least-privilege policy, and zero-downtime secret rotation |

### 🚀 GitOps & Delivery
| Repo | Focus |
|---|---|
| [argocd-deployment](https://github.com/shahid-khaleel/argocd-deployment) | A complete GitOps loop: GitHub Actions builds and pushes an image, rewrites the manifest, and Argo CD syncs it to a cluster — with real troubleshooting notes captured from live deployment sessions. |
| [gitops](https://github.com/shahid-khaleel/gitops) | Self-managed GitLab, a Kubernetes-executor GitLab Runner, and Argo CD all running on one Minikube cluster — Kaniko + Trivy build/scan pipeline, Docker Hub as the only registry, webhook-triggered sync, and drift/self-heal + Git-based rollback demonstrated live. Deployed and debugged end-to-end, not just written: chart version pinned after the default dropped bundled Postgres/Redis, an in-cluster `clone_url` fix for the Runner, a YAML lint bug caught via GitLab's own CI Lint API, and server-side apply required for Argo CD's oversized CRDs. |

### 🤖 MLOps & Observability
| Repo | Focus |
|---|---|
| [mlops-credit-card-fraud-detection](https://github.com/shahid-khaleel/mlops-credit-card-fraud-detection) | A full MLOps stack (training → MLflow → model serving → prediction API) with Kubernetes manifests for autoscaling, RBAC, network policy, and a full observability stack (Prometheus/Grafana/Jaeger). |
| [mlops](https://github.com/shahid-khaleel/mlops) | A churn-prediction MLOps stack on Minikube: MLflow tracking + Model Registry, KServe (Standard/RawDeployment mode) serving both a test and the production model, Kubeflow Trainer, and a fully working Kubeflow Dashboard behind Istio + Dex + oauth2-proxy — backed by a 12-section reference manual documenting every API surface, real gotcha hit, and the exact reproduction runbook. |
| [kubeflow-implementation](https://github.com/shahid-khaleel/kubeflow-implementation) | A single-node Kubeflow proof-of-concept using real KServe/KFP custom resources for a training → serving pipeline |
| [fluentd-implementation](https://github.com/shahid-khaleel/fluentd-implementation) | A Kubernetes logging pipeline: a custom Fluentd image and Helm chart routing multi-service logs to Elasticsearch and S3, with real incident write-ups |

---

## 🛠️ Core Technologies

`Kubernetes` `Minikube` `Terraform` `Ansible` `Helm` `Istio` `Argo CD` `HashiCorp Vault` `Keycloak` `Docker` `AWS (EKS/IAM/KMS/EFS)` `GitHub Actions` `GitLab CI` `GitLab (self-managed)` `Jenkins` `SonarQube` `Prometheus/Grafana` `Jaeger` `MLflow` `FastAPI` `Elasticsearch` `Fluentd` `Kibana` `Kyverno` `Kaniko` `Trivy` `cosign/Sigstore` `SLSA`

---

## ☁️ AWS Expertise

`AWS Solutions Architect` `AWS DevOps Professional` `AWS Security` `AWS Networking` `AWS Serverless` `AWS EKS`

---

## 📫 Reach me

[![LinkedIn](https://img.shields.io/badge/LinkedIn-shahidkhaleel78-0A66C2?logo=linkedin&logoColor=white)](https://www.linkedin.com/in/shahidkhaleel78/)

Open an issue on any of the repos above, connect on [LinkedIn](https://www.linkedin.com/in/shahidkhaleel78/), or reach out via GitHub.
