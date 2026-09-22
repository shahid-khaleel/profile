<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:2B213A,50:E5289E,100:EF8539&height=200&section=header&text=Shahid%20Khaleel&fontSize=48&fontColor=ffffff&fontAlignY=38&desc=Senior%20DevOps%20Engineer&descAlignY=58&descSize=20&animation=fadeIn" width="100%"/>

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&pause=1200&color=E5289E&center=true&vCenter=true&width=750&lines=Senior+DevOps+Engineer;Kubernetes+%7C+GitOps+%7C+Service+Mesh+%7C+IaC;Self-hosted+GitLab+%2B+Kubernetes-native+CI%2FCD;I+ship+the+debugging+notes%2C+not+just+the+demo)](https://github.com/shahid-khaleel)

[![LinkedIn](https://img.shields.io/badge/LinkedIn-shahidkhaleel78-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/shahidkhaleel78/)
[![GitHub followers](https://img.shields.io/github/followers/shahid-khaleel?style=for-the-badge&logo=github&label=Follow&color=181717)](https://github.com/shahid-khaleel)

📍 Bengaluru, India · Open to relocation (hybrid/on-site)

</div>

Senior DevOps Engineer with close to 7 years building secure, reliable, cost-optimized cloud infrastructure for fintech/BFSI platforms processing **1M+ transactions/day at 99.99% uptime**. Outside of work, I build real, working cloud-native infrastructure in the open — **IaC**, **Kubernetes**, **service mesh**, **cloud infrastructure**, **GitOps**, **identity & security**, **CI/CD**, **observability**, and **MLOps**. Every repository ships source code, infrastructure definitions, deployment workflows, and architecture docs — plus the trade-offs, debugging, and challenges I actually hit, not a polished-outcomes-only highlight reel.

## ⚡ Highlights

**In production (fintech/BFSI):**
- **Cut manual deployment effort by 80%** building GitLab CI/CD pipelines to automate AWS EKS deployments, then layering in GitOps via Argo CD for declarative, version-controlled rollouts.
- **Cut AWS infrastructure costs by 25%** through resource right-sizing and autoscaling, without touching uptime SLAs.
- **Cut incident response time by 60%** building out observability across microservices with Prometheus, Grafana, and Kibana.
- **Led disaster recovery** for a public-sector banking client — on-premises infrastructure buildout (Bengaluru–Kolkata) and cloud business continuity (Mumbai–Hyderabad) — including DR drills and RCSA remediation.
- **Built compliance readiness** across RBI, REBIT, SOC 2, and ISO 27001, supporting successful regulatory audits with banking partners.
- **Cut release time by 50%+** earlier in my career by automating builds and deployments with Jenkins.

**In the open-source projects below:**
- **Root-caused a production-grade tracing bug** in Python's OpenTelemetry auto-instrumentation that was silently splitting every distributed trace in two — diagnosed, fixed, and documented step by step in a runbook.
- **Built a self-managed GitOps platform end-to-end**: GitLab, a Kubernetes-executor GitLab Runner, and Argo CD on one cluster with a Kaniko + Trivy build/scan pipeline, webhook-triggered sync, and Git-based rollback — then debugged it through a chart-pinning issue, an in-cluster `clone_url` fix, a YAML lint failure caught via GitLab's own CI Lint API, and server-side apply for Argo CD's oversized CRDs.
- **Verified a 5-service mesh end-to-end on Istio**: STRICT mTLS, RED metrics, one real distributed trace with correct parent-child spans across every hop, and an EFK pipeline that splits routine logs from a compliance audit index.
- **Implemented kernel-level observability with zero application instrumentation** using Cilium/Hubble + Tetragon, backed by a threat-intel alerting pipeline and Kyverno admission control.
- **Authored a 12-section MLOps reference manual** for a full stack — MLflow, KServe, Kubeflow Trainer, and a Kubeflow Dashboard behind Istio + Dex + oauth2-proxy — documenting every API surface and the exact reproduction steps for each gotcha hit.
- **Curated a ~150-topic Kubernetes/Docker/Linux security knowledge base** from hands-on work, not just reading docs.

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
| [terraform](https://github.com/shahid-khaleel/terraform) | **Provisioned** a modular, environment-scoped (`qa`) EKS + KMS stack from reusable community modules |
| [eks-deployment](https://github.com/shahid-khaleel/eks-deployment) | **Built** a standalone EKS reference deployment with IRSA, Cluster Autoscaler, and the AWS Load Balancer Controller, plus a secondary-IP automation script |
| [ansible](https://github.com/shahid-khaleel/ansible) | **Automated** role-based provisioning (Apache, Docker, Java, Keycloak, MySQL, MongoDB, Node.js, Redis) through a GitLab CI deploy pipeline |
| [helm](https://github.com/shahid-khaleel/helm) | **Shipped** a Helm chart + CI scripting to deploy a Spring Boot app to EKS via an S3-backed chart repository |

### ⎈ Kubernetes Platform & Security
| Repo | Focus |
|---|---|
| [kubernetes](https://github.com/shahid-khaleel/kubernetes) | **Built** a focused set of K8s operator demos: ConfigMap hot-reload, EFS CSI storage, IRSA for S3 access, the API request lifecycle (Kyverno + Kustomize), MySQL StatefulSet replication, and a full Jenkins → SonarQube → Docker → Minikube CI/CD pipeline end-to-end |
| [kubernetes-security-documentation](https://github.com/shahid-khaleel/kubernetes-security-documentation) | **Curated** a ~150-topic knowledge base spanning Linux, Docker, and Kubernetes security fundamentals |
| [kubernetes-fds](https://github.com/shahid-khaleel/kubernetes-fds) | **Simulated** a Kubernetes file-descriptor-exhaustion failure mode, paired with a Grafana dashboard to observe it live |

### 🔐 Service Mesh, Identity & Secrets
| Repo | Focus |
|---|---|
| [istio-service-mesh](https://github.com/shahid-khaleel/istio-service-mesh) | **Demonstrated** core Istio mesh capabilities on two live microservices: strict mTLS, ingress gateway routing, canary traffic splitting, fault injection, and circuit breaking |
| [keycloak-auth-apache](https://github.com/shahid-khaleel/keycloak-auth-apache) | **Evolved** Keycloak-based auth behind an Apache reverse proxy across branches into a full Kubernetes + Istio + observability deployment |
| [k8s-auth-keycloak](https://github.com/shahid-khaleel/k8s-auth-keycloak) | **Implemented** Kubernetes-native OIDC authentication via Keycloak, deployable via raw manifests, Helm, or Docker Compose |
| [hashicorp-vault-project](https://github.com/shahid-khaleel/hashicorp-vault-project) | **Implemented** Vault secrets management twice, independently, in Python/Flask and Java/Spring Boot — covering AppRole auth, KV v2, least-privilege policy, and zero-downtime secret rotation |

### 🚀 GitOps & Delivery
| Repo | Focus |
|---|---|
| [argocd-deployment](https://github.com/shahid-khaleel/argocd-deployment) | **Built** a complete GitOps loop: GitHub Actions builds and pushes an image, rewrites the manifest, and Argo CD syncs it to a cluster — with real troubleshooting notes captured from live deployment sessions |

### 🤖 MLOps & Observability
| Repo | Focus |
|---|---|
| [mlops-credit-card-fraud-detection](https://github.com/shahid-khaleel/mlops-credit-card-fraud-detection) | **Built** a full MLOps stack (training → MLflow → model serving → prediction API) with Kubernetes manifests for autoscaling, RBAC, network policy, and a full observability stack (Prometheus/Grafana/Jaeger) |
| [mlops](https://github.com/shahid-khaleel/mlops) | **Built** a churn-prediction MLOps stack on Minikube: MLflow tracking + Model Registry, KServe (Standard/RawDeployment mode) serving both a test and the production model, Kubeflow Trainer, and a fully working Kubeflow Dashboard behind Istio + Dex + oauth2-proxy — backed by a 12-section reference manual documenting every API surface, real gotcha hit, and the exact reproduction runbook |
| [kubeflow-implementation](https://github.com/shahid-khaleel/kubeflow-implementation) | **Built** a single-node Kubeflow proof-of-concept using real KServe/KFP custom resources for a training → serving pipeline |
| [fluentd-implementation](https://github.com/shahid-khaleel/fluentd-implementation) | **Built** a Kubernetes logging pipeline — a custom Fluentd image and Helm chart routing multi-service logs to Elasticsearch and S3 — with real incident write-ups |

---

## 🛠️ Core Technologies

**Containers & Orchestration**
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white)
![Minikube](https://img.shields.io/badge/Minikube-4285F4?style=for-the-badge&logo=kubernetes&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Helm](https://img.shields.io/badge/Helm-0F1689?style=for-the-badge&logo=helm&logoColor=white)
![Istio](https://img.shields.io/badge/Istio-466BB0?style=for-the-badge&logo=istio&logoColor=white)
![Kiali](https://img.shields.io/badge/Kiali-1D2A5B?style=for-the-badge&logoColor=white)

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
![AWS Secrets Manager](https://img.shields.io/badge/AWS_Secrets_Manager-FF9900?style=for-the-badge&logo=amazonaws&logoColor=white)
![Keycloak](https://img.shields.io/badge/Keycloak-4D4D4D?style=for-the-badge&logo=keycloak&logoColor=white)
![Kyverno](https://img.shields.io/badge/Kyverno-2F8CB3?style=for-the-badge&logo=kyverno&logoColor=white)

**Observability & Tracing**
![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=for-the-badge&logo=prometheus&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana-F46800?style=for-the-badge&logo=grafana&logoColor=white)
![Jaeger](https://img.shields.io/badge/Jaeger-666666?style=for-the-badge&logo=jaeger&logoColor=white)
![OpenTelemetry](https://img.shields.io/badge/OpenTelemetry-425CC7?style=for-the-badge&logo=opentelemetry&logoColor=white)
![Elasticsearch](https://img.shields.io/badge/Elasticsearch-005571?style=for-the-badge&logo=elasticsearch&logoColor=white)
![Kibana](https://img.shields.io/badge/Kibana-005571?style=for-the-badge&logo=kibana&logoColor=white)
![Fluentd](https://img.shields.io/badge/Fluentd-0E83C8?style=for-the-badge&logo=fluentd&logoColor=white)

**Cloud & App/ML Frameworks**
![AWS](https://img.shields.io/badge/AWS-FF9900?style=for-the-badge&logo=amazonaws&logoColor=white) *(EKS · Lambda · IAM · KMS · VPC · Route53 · ALB/NLB · Security Groups · EFS)*
![MLflow](https://img.shields.io/badge/MLflow-0194E2?style=for-the-badge&logo=mlflow&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)

**Caching & Databases**
![Valkey](https://img.shields.io/badge/Valkey-2D2D2D?style=for-the-badge&logo=valkey&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)

**Application Servers & Virtualization**
![Tomcat](https://img.shields.io/badge/Tomcat-F8DC75?style=for-the-badge&logo=apachetomcat&logoColor=black)
![JBoss](https://img.shields.io/badge/JBoss-EC1C24?style=for-the-badge&logoColor=white)
![WebLogic](https://img.shields.io/badge/WebLogic-F80000?style=for-the-badge&logoColor=white)
![VMware](https://img.shields.io/badge/VMware-607078?style=for-the-badge&logo=vmware&logoColor=white)

---

## ☁️ AWS Focus Areas

![Solutions Architecture](https://img.shields.io/badge/Solutions_Architecture-FF9900?style=for-the-badge&logo=amazonaws&logoColor=white)
![DevOps & Automation](https://img.shields.io/badge/DevOps_%26_Automation-FF9900?style=for-the-badge&logo=amazonaws&logoColor=white)
![Cloud Security](https://img.shields.io/badge/Cloud_Security-FF9900?style=for-the-badge&logo=amazonaws&logoColor=white)
![Networking](https://img.shields.io/badge/Networking-FF9900?style=for-the-badge&logo=amazonaws&logoColor=white)
![Serverless](https://img.shields.io/badge/Serverless-FF9900?style=for-the-badge&logo=amazonaws&logoColor=white)
![EKS & Containers](https://img.shields.io/badge/EKS_%26_Containers-FF9900?style=for-the-badge&logo=amazonaws&logoColor=white)

---

## 📫 Reach me

<div align="center">

[![LinkedIn](https://img.shields.io/badge/LinkedIn-shahidkhaleel78-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/shahidkhaleel78/)
[![GitHub](https://img.shields.io/badge/GitHub-shahid--khaleel-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/shahid-khaleel)
[![Gmail](https://img.shields.io/badge/Gmail-shahidkhaleel78%40gmail.com-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:shahidkhaleel78@gmail.com)

</div>

Open an issue on any of the repos above, connect on [LinkedIn](https://www.linkedin.com/in/shahidkhaleel78/), email me at [shahidkhaleel78@gmail.com](mailto:shahidkhaleel78@gmail.com), or reach out via GitHub.
