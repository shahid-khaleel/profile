<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:2B213A,50:E5289E,100:EF8539&height=200&section=header&text=Shahid%20Khaleel&fontSize=48&fontColor=ffffff&fontAlignY=38&desc=Senior%20DevOps%20Engineer&descAlignY=58&descSize=20&animation=fadeIn" width="100%"/>

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&pause=1200&color=E5289E&center=true&vCenter=true&width=750&lines=Senior+DevOps+Engineer;Kubernetes+%7C+GitOps+%7C+Service+Mesh+%7C+IaC;Self-hosted+GitLab+%2B+Kubernetes-native+CI%2FCD;I+ship+the+debugging+notes%2C+not+just+the+demo)](https://github.com/shahid-khaleel)

[![LinkedIn](https://img.shields.io/badge/LinkedIn-shahidkhaleel78-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/shahidkhaleel78/)
[![GitHub followers](https://img.shields.io/github/followers/shahid-khaleel?style=for-the-badge&logo=github&label=Follow&color=181717)](https://github.com/shahid-khaleel)

</div>

Senior DevOps Engineer building real, working cloud-native infrastructure — **IaC**, **Kubernetes**, **service mesh**, **cloud infrastructure**, **GitOps**, **identity & security**, **CI/CD**, **observability**, and **MLOps**. Every repository ships source code, infrastructure definitions, deployment workflows, and architecture docs — plus the trade-offs, debugging, and challenges I actually hit, not a polished-outcomes-only highlight reel.

```bash
$ whoami
shahid-khaleel

$ kubectl get engineer shahid-khaleel -o wide
NAME              STATUS   ROLE                   UPTIME   RESTARTS
shahid-khaleel    Ready    Senior DevOps Engineer  24/7     0 (reads the postmortem first)

$ cat ./philosophy.md
> Ship it deployed, debugged, and documented — not just demoed.
> If it broke in production, it's in the README.
```

<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/shahid-khaleel/profile/output/github-contribution-grid-snake-dark.svg" />
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/shahid-khaleel/profile/output/github-contribution-grid-snake.svg" />
  <img alt="contribution snake animation" src="https://raw.githubusercontent.com/shahid-khaleel/profile/output/github-contribution-grid-snake.svg" width="100%" />
</picture>

</div>

---

## 🏆 Start here — 4 projects that show the range

<table>
<tr><td width="50%" valign="top">

### [gitops](https://github.com/shahid-khaleel/gitops)
Self-managed GitLab, a Kubernetes-executor GitLab Runner, and Argo CD all running on one Minikube cluster — Kaniko + Trivy build/scan pipeline, webhook-triggered sync, and drift/self-heal + Git-based rollback demonstrated live. Deployed and debugged end-to-end: chart version pinning, an in-cluster `clone_url` fix, a YAML lint bug caught via GitLab's own CI Lint API, and server-side apply for Argo CD's oversized CRDs.

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

16 more repositories across Cloud Infrastructure, Kubernetes Platform, Service Mesh, GitOps, and MLOps.

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

### 🤖 MLOps & Observability
| Repo | Focus |
|---|---|
| [mlops-credit-card-fraud-detection](https://github.com/shahid-khaleel/mlops-credit-card-fraud-detection) | A full MLOps stack (training → MLflow → model serving → prediction API) with Kubernetes manifests for autoscaling, RBAC, network policy, and a full observability stack (Prometheus/Grafana/Jaeger). |
| [mlops](https://github.com/shahid-khaleel/mlops) | A churn-prediction MLOps stack on Minikube: MLflow tracking + Model Registry, KServe (Standard/RawDeployment mode) serving both a test and the production model, Kubeflow Trainer, and a fully working Kubeflow Dashboard behind Istio + Dex + oauth2-proxy — backed by a 12-section reference manual documenting every API surface, real gotcha hit, and the exact reproduction runbook. |
| [kubeflow-implementation](https://github.com/shahid-khaleel/kubeflow-implementation) | A single-node Kubeflow proof-of-concept using real KServe/KFP custom resources for a training → serving pipeline |
| [fluentd-implementation](https://github.com/shahid-khaleel/fluentd-implementation) | A Kubernetes logging pipeline: a custom Fluentd image and Helm chart routing multi-service logs to Elasticsearch and S3, with real incident write-ups |

---

## 🛠️ Core Technologies

**Containers & Orchestration**
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white)
![Minikube](https://img.shields.io/badge/Minikube-4285F4?style=for-the-badge&logo=kubernetes&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Helm](https://img.shields.io/badge/Helm-0F1689?style=for-the-badge&logo=helm&logoColor=white)
![Istio](https://img.shields.io/badge/Istio-466BB0?style=for-the-badge&logo=istio&logoColor=white)

**Infrastructure as Code**
![Terraform](https://img.shields.io/badge/Terraform-7B42BC?style=for-the-badge&logo=terraform&logoColor=white)
![Ansible](https://img.shields.io/badge/Ansible-EE0000?style=for-the-badge&logo=ansible&logoColor=white)

**CI/CD & GitOps**
![GitLab](https://img.shields.io/badge/GitLab_(self--managed)-FC6D26?style=for-the-badge&logo=gitlab&logoColor=white)
![GitLab CI](https://img.shields.io/badge/GitLab_CI-FC6D26?style=for-the-badge&logo=gitlab&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)
![Jenkins](https://img.shields.io/badge/Jenkins-D24939?style=for-the-badge&logo=jenkins&logoColor=white)
![Argo CD](https://img.shields.io/badge/Argo_CD-EF7B4D?style=for-the-badge&logo=argo&logoColor=white)
![Kaniko](https://img.shields.io/badge/Kaniko-34A853?style=for-the-badge&logo=kaniko&logoColor=white)
![Trivy](https://img.shields.io/badge/Trivy-1A73E8?style=for-the-badge&logo=trivy&logoColor=white)
![SonarQube](https://img.shields.io/badge/SonarQube-4E9BCD?style=for-the-badge&logo=sonarqube&logoColor=white)

**Identity, Security & Supply Chain**
![HashiCorp Vault](https://img.shields.io/badge/HashiCorp_Vault-000000?style=for-the-badge&logo=vault&logoColor=FFEC6E)
![Keycloak](https://img.shields.io/badge/Keycloak-4D4D4D?style=for-the-badge&logo=keycloak&logoColor=white)
![Kyverno](https://img.shields.io/badge/Kyverno-2F8CB3?style=for-the-badge&logo=kyverno&logoColor=white)

**Observability**
![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=for-the-badge&logo=prometheus&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana-F46800?style=for-the-badge&logo=grafana&logoColor=white)
![Jaeger](https://img.shields.io/badge/Jaeger-666666?style=for-the-badge&logo=jaeger&logoColor=white)
![Elasticsearch](https://img.shields.io/badge/Elasticsearch-005571?style=for-the-badge&logo=elasticsearch&logoColor=white)
![Kibana](https://img.shields.io/badge/Kibana-005571?style=for-the-badge&logo=kibana&logoColor=white)
![Fluentd](https://img.shields.io/badge/Fluentd-0E83C8?style=for-the-badge&logo=fluentd&logoColor=white)

**Cloud & App/ML Frameworks**
![AWS](https://img.shields.io/badge/AWS-FF9900?style=for-the-badge&logo=amazonaws&logoColor=white) *(EKS · IAM · KMS · EFS)*
![MLflow](https://img.shields.io/badge/MLflow-0194E2?style=for-the-badge&logo=mlflow&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)

---

## ☁️ AWS Expertise

![AWS Solutions Architect](https://img.shields.io/badge/AWS_Solutions_Architect-FF9900?style=for-the-badge&logo=amazonaws&logoColor=white)
![AWS DevOps Professional](https://img.shields.io/badge/AWS_DevOps_Professional-FF9900?style=for-the-badge&logo=amazonaws&logoColor=white)
![AWS Security](https://img.shields.io/badge/AWS_Security-FF9900?style=for-the-badge&logo=amazonaws&logoColor=white)
![AWS Networking](https://img.shields.io/badge/AWS_Networking-FF9900?style=for-the-badge&logo=amazonaws&logoColor=white)
![AWS Serverless](https://img.shields.io/badge/AWS_Serverless-FF9900?style=for-the-badge&logo=amazonaws&logoColor=white)
![AWS EKS](https://img.shields.io/badge/AWS_EKS-FF9900?style=for-the-badge&logo=amazonaws&logoColor=white)

---

## 📫 Reach me

<div align="center">

[![LinkedIn](https://img.shields.io/badge/LinkedIn-shahidkhaleel78-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/shahidkhaleel78/)
[![GitHub](https://img.shields.io/badge/GitHub-shahid--khaleel-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/shahid-khaleel)
[![WhatsApp](https://img.shields.io/badge/WhatsApp-%2B91_REDACTED-25D366?style=for-the-badge&logo=whatsapp&logoColor=white)](https://wa.me/91REDACTED)

</div>

Open an issue on any of the repos above, connect on [LinkedIn](https://www.linkedin.com/in/shahidkhaleel78/), message me on [WhatsApp](https://wa.me/91REDACTED), or reach out via GitHub.
