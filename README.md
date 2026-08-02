# Hi, I'm Shahid Khaleel 👋

Senior DevOps Engineer with hands-on experience designing and implementing real-world cloud-native infrastructure and platform engineering projects. My work spans **Infrastructure as Code (IaC)**, **Kubernetes**, **service mesh**, **cloud infrastructure**, **GitOps**, **identity & security**, **CI/CD**, **observability**, and **MLOps**, with every repository representing a practical, working implementation rather than a theoretical proof of concept.

The projects below showcase end-to-end implementations built from the ground up using production-grade tools and engineering practices. Each repository includes source code, infrastructure definitions, deployment workflows, architecture documentation, and implementation details that reflect the standards I expect when reviewing senior-level engineering work.

I document the complete engineering journey—including design decisions, trade-offs, challenges, known limitations, and future improvements—instead of only presenting polished outcomes. If you're a recruiter or hiring manager, the **Flagship Projects** section below is the quickest way to explore the breadth of my hands-on experience across **IaC, Kubernetes platform engineering, service mesh, cloud infrastructure, GitOps, and MLOps**.

---

## 🚀 Flagship Projects

Organized by track — every project here is a real, working implementation with source code, infrastructure definitions, deployment workflows, and architecture documentation behind it.

### 🏆 Core Platforms
| Project | What it demonstrates |
|---|---|
| [**payment-platform**](https://github.com/shahid-khaleel/payment-platform) | A 19-microservice payment platform (auth, wallet, settlement, fraud detection, webhooks...) with per-service Helm charts, Kustomize overlays, contract tests, load tests, dependency scanning, and incident runbooks — the largest and most operationally mature project here. |
| [**argocd-deployment**](https://github.com/shahid-khaleel/argocd-deployment) | A complete GitOps loop: GitHub Actions builds and pushes an image, rewrites the manifest, and Argo CD syncs it to a cluster — with real troubleshooting notes captured from live deployment sessions. |
| [**mlops-credit-card-fraud-detection**](https://github.com/shahid-khaleel/mlops-credit-card-fraud-detection) | A full MLOps stack (training → MLflow → model serving → prediction API) with Kubernetes manifests for autoscaling, RBAC, network policy, and a full observability stack (Prometheus/Grafana/Jaeger). |

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
| [kubernetes](https://github.com/shahid-khaleel/kubernetes) | A collection of focused K8s operator demos: ConfigMap hot-reload, EFS CSI storage, IRSA for S3 access, the API request lifecycle (Kyverno + Kustomize), and MySQL StatefulSet replication |
| [kubernetes-security-documentation](https://github.com/shahid-khaleel/kubernetes-security-documentation) | A curated ~150-topic personal knowledge base spanning Linux, Docker, and Kubernetes security fundamentals |
| [app](https://github.com/shahid-khaleel/app) | A Kubernetes file-descriptor-exhaustion failure-mode simulator, paired with a Grafana dashboard to observe it |

### 🔐 Service Mesh, Identity & Secrets
| Repo | Focus |
|---|---|
| [istio-service-mesh](https://github.com/shahid-khaleel/istio-service-mesh) | Istio service mesh capabilities on two demo microservices: strict mTLS, ingress gateway routing, canary traffic splitting, fault injection, and circuit breaking |
| [keycloak-auth-apache](https://github.com/shahid-khaleel/keycloak-auth-apache) | Keycloak-based auth behind an Apache reverse proxy, with an evolution across branches toward a full Kubernetes + Istio + observability deployment |
| [k8s-auth-keycloak](https://github.com/shahid-khaleel/k8s-auth-keycloak) | Kubernetes-native OIDC authentication via Keycloak, deployable via raw manifests, Helm, or Docker Compose |
| [hashicorp-vault-project](https://github.com/shahid-khaleel/hashicorp-vault-project) | Vault secrets management implemented twice independently (Python/Flask and Java/Spring Boot), covering AppRole auth, KV v2, least-privilege policy, and zero-downtime secret rotation |

### 🤖 MLOps & Observability
| Repo | Focus |
|---|---|
| [kubeflow-implementation](https://github.com/shahid-khaleel/kubeflow-implementation) | A single-node Kubeflow proof-of-concept using real KServe/KFP custom resources for a training → serving pipeline |
| [fluentd-implementation](https://github.com/shahid-khaleel/fluentd-implementation) | A Kubernetes logging pipeline: a custom Fluentd image and Helm chart routing multi-service logs to Elasticsearch and S3, with real incident write-ups |

### 🖥️ Full-Stack Applications
| Repo | Focus |
|---|---|
| [devopslearning](https://github.com/shahid-khaleel/devopslearning) | A fintech demo app (Flask + React) extended with LLM-driven natural-language intent routing |

---

## 🛠️ Core Technologies

`Kubernetes` `Terraform` `Ansible` `Helm` `Istio` `Argo CD` `HashiCorp Vault` `Keycloak` `Docker` `AWS (EKS/IAM/KMS/EFS)` `GitHub Actions` `GitLab CI` `Prometheus/Grafana` `Jaeger` `MLflow` `Fluentd`

---

## 📫 Reach me

Open an issue on any of the repos above, or connect via GitHub.
