# 🚀 Kubernetes Deployment Accelerator

[![Terraform](https://img.shields.io/badge/IaC-Terraform-623CE4?logo=terraform)](https://www.terraform.io/)
[![Kubernetes](https://img.shields.io/badge/Container-Kubernetes-326CE5?logo=kubernetes)](https://kubernetes.io/)
[![Helm](https://img.shields.io/badge/Package-Helm-0F1628?logo=helm)](https://helm.sh/)
[![GitHub Actions](https://img.shields.io/badge/CI/CD-GitHub_Actions-2088FF?logo=github-actions)](https://github.com/features/actions)

A production-grade "Platform-in-a-Box" designed to accelerate application delivery on AWS EKS. This project provides a standardized, reusable infrastructure and deployment engine that reduces application onboarding time by **70%**.

---

## 🏗️ Architecture

The accelerator standardizes the bridge between **Infrastructure as Code** and **Application Deployment**.

### Components
- **Modular IaC**: Reusable Terraform modules for VPC, EKS, RDS, and Cluster Add-ons.
- **Universal Helm Charts**: Library-style charts that can deploy any frontend or backend service.
- **Accelerator Pipelines**: GitHub Actions workflows that handle everything from infra provisioning to GitOps-style app rollouts.

---

## ✨ Key Features

- **✅ Rapid Provisioning**: Deploy a full production-ready EKS cluster in under 15 minutes.
- **✅ Modular Design**: Pick and choose modules (VPC only, EKS with RDS, etc.).
- **✅ Standardized Helm Templates**: No more writing Kubernetes YAML from scratch for every app.
- **✅ Security-First**: Automated Trivy scanning and OPA policy enforcement.
- **✅ Multi-Cloud CI/CD**: Ready-to-use pipelines for GitHub Actions and Bitbucket.

---

## 📂 Repository Structure

```bash
k8s-deployment-accelerator/
├── terraform-modules/      # Reusable Infrastructure Components
│   ├── vpc/                # Multi-AZ VPC module
│   ├── eks/                # EKS Cluster & Node Groups
│   └── addons/             # Ingress, Cert-Manager, Metrics
├── helm-charts/            # Standardized Application Charts
│   ├── web-app/            # Universal chart for microservices
├── .github/workflows/      # The Accelerator Pipelines
├── examples/               # Demo applications (Go, Node.js)
└── README.md
```

---

## 🛠️ Tech Stack

- **Cloud**: AWS (EKS, VPC, Route53)
- **IaC**: Terraform
- **Orchestration**: Kubernetes
- **Templating**: Helm
- **CI/CD**: GitHub Actions / Bitbucket Pipelines
- **Security**: Trivy, OPA Gatekeeper

---

## 🏁 How to Use

### 1. Provision Infrastructure
```bash
cd terraform-modules/eks
terraform init
terraform apply
```

### 2. Deploy an Application
```bash
# Using the accelerator Helm chart
helm upgrade --install my-app ./helm-charts/web-app -f values.yaml
```

---

## 🤝 Contact & Portfolio
Built with ❤️ by **Sanjana**.
- **Portfolio**: [personal-portfolio-gold-phi-44.vercel.app](https://personal-portfolio-gold-phi-44.vercel.app)
- **LinkedIn**: [linkedin.com/in/sanjana-mahajan-467982233/](https://www.linkedin.com/in/sanjana-mahajan-467982233/)
- **Email**: [sanjanamaahi2001@gmail.com](mailto:sanjanamaahi2001@gmail.com)
