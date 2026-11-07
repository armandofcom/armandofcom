<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/header-dark.svg">
  <img alt="Armando Felipe — AWS Cloud Architect · FinOps & DevSecOps" src="assets/header-light.svg" width="100%">
</picture>

<br/>

[![LinkedIn](https://img.shields.io/badge/LinkedIn-armandofcom-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/armandofcom/) [![SysCu](https://img.shields.io/badge/SysCu-syscu.es-00A7E1?style=for-the-badge&logo=googlechrome&logoColor=white)](https://www.syscu.es/) [![Credly](https://img.shields.io/badge/Credly-badges-FF6B00?style=for-the-badge&logo=credly&logoColor=white)](https://www.credly.com/users/armandofcom/badges) [![Email](https://img.shields.io/badge/Email-contact-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:armandof@armandof.com)

[![Diagnóstico FinOps AWS gratuito](https://img.shields.io/badge/Diagn%C3%B3stico%20FinOps%20AWS%20gratuito-con%20SysCu-00A7E1?style=for-the-badge)](https://www.syscu.es/contacto)

</div>

## ⚡ Now

- 🌱 **Founder @ [SysCu](https://www.syscu.es/)** — DevOps & FinOps on AWS for companies in Spain.
- 🧪 **Open-sourcing FinOps tooling**, like [syscu-kiro-report-usage](https://github.com/syscu-es/syscu-kiro-report-usage): one command, one HTML file, Kiro usage and cost per user.
- ✍️ **Writing** about FinOps, ECS, Bedrock AgentCore and AI at work on [LinkedIn](https://www.linkedin.com/in/armandofcom/recent-activity/all/) (2,200+ followers).

## 📈 Impact

<div align="center">
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/impact-dark.svg">
  <img alt="63% lower quarterly AWS invoices · 100+ pipelines and clusters as code · 400+ B2B clients kept compliant · 80+ branches on VPN/MPLS" src="assets/impact-light.svg" width="100%">
</picture>
</div>

<sub>Opinno, 2023–2026 (cloud engineer, independent). Figures from my [LinkedIn experience](https://www.linkedin.com/in/armandofcom/).</sub>

## 🧭 What I do

| ☁️ **Cloud architecture** | 💸 **FinOps** | 🔐 **DevSecOps** |
|---|---|---|
| Multi-account AWS, landing zones, networking, migrations and disaster recovery. | Cost allocation, tagging, rightsizing and spend made visible to engineering and business. | Security as code, secrets, IAM/RBAC, Zero Trust, GDPR and ISO 27001 controls in the pipeline. |
| 🧱 **Platform & IaC** | ☸️ **Containers** | 📡 **SRE & observability** |
| Terraform / OpenTofu modules, GitOps, repeatable delivery. | EKS, ECS Fargate, Nomad, Consul, Helm, ArgoCD. | Metrics, logs, traces and SLOs: CloudWatch, Prometheus, Grafana, ELK. |

<details>
<summary><b>🏗️ How I think — a reference architecture</b></summary>

```mermaid
%%{init: {'theme':'dark', 'themeVariables': { 'primaryColor':'#232F3E', 'primaryTextColor':'#fff', 'primaryBorderColor':'#FF9900', 'lineColor':'#FF9900', 'secondaryColor':'#1a2332', 'tertiaryColor':'#0d1117'}}}%%
flowchart LR
    subgraph GOV["🏛️ Governance Layer"]
        ORG[AWS Organizations]
        SCP[SCPs & Guardrails]
        IAM[IAM Identity Center]
    end

    subgraph PLAT["⚙️ Platform Layer"]
        NET[VPC / TGW / Networking]
        EKS[EKS + ArgoCD GitOps]
        IAC[Terraform Modules]
    end

    subgraph OPS["📊 Operations Layer"]
        OBS[Prometheus / Grafana / CloudWatch]
        SEC[Prowler / Wazuh / Vault]
        FIN[CUR / Cost Dashboards]
    end

    ORG --> NET
    SCP --> EKS
    IAM --> EKS
    IAC --> NET & EKS
    EKS --> OBS
    NET --> SEC
    OBS & SEC & FIN --> DECIDE{{"💡 Informed<br/>Decisions"}}
```

**Security by design. Observability by default. Cost-awareness always.**

</details>

## 🧳 Experience

| When | Role | Where |
|---|---|---|
| Now | **Founder** | [SysCu](https://www.syscu.es/) — DevOps & FinOps on AWS |
| 2025 – 2026 | Senior Cloud Systems Architect | Paradigma Digital · remote, Madrid |
| 2023 – 2026 | Cloud Engineer | Opinno Ecuador · independent |
| 2024 – 2025 | DevOps Engineer | CloudAPPi · hybrid, Madrid |
| 2023 – 2024 | DevOps Team Lead | Irontec · remote, Bilbao |
| 2016 – 2024 | CEO | SysAdmins de Cuba · community |

🎓 Computer Science Engineering (in progress) — Universidad de las Ciencias Informáticas.

## 🛠️ Stack

<div align="center">
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://skillicons.dev/icons?i=aws%2Cterraform%2Ckubernetes%2Cdocker%2Cansible%2Cpython%2Cbash%2Cgo%2Cgithubactions%2Cgitlab%2Cprometheus%2Cgrafana%2Clinux%2Cpostgres&perline=14&theme=dark">
  <img alt="AWS, Terraform, Kubernetes, Docker, Ansible, Python, Bash, Go, GitHub Actions, GitLab, Prometheus, Grafana, Linux, PostgreSQL" src="https://skillicons.dev/icons?i=aws,terraform,kubernetes,docker,ansible,python,bash,go,githubactions,gitlab,prometheus,grafana,linux,postgres&perline=14&theme=light">
</picture>
</div>

<sub>Also: OpenTofu · Vault · Consul · Nomad · ArgoCD · OpenStack · Prowler · Wazuh · CloudWatch · ELK · Sentry.</sub>

## 🧩 Open source

| Project | What it does | |
|---|---|---|
| [**syscu-kiro-report-usage**](https://github.com/syscu-es/syscu-kiro-report-usage) | Self-contained HTML report of **Kiro** usage and cost per IAM Identity Center user. Works with any AWS account through SSO. | [![PyPI](https://img.shields.io/pypi/v/syscu-kiro-report-usage?style=flat-square&color=00A7E1)](https://pypi.org/project/syscu-kiro-report-usage/) |
| [**ECS-RDS-Control-Dashboard**](https://github.com/armandofcom/ECS-RDS-Control-Dashboard) | Internal ops panel to start/stop ECS services and RDS databases, with authentication, short-lived tokens and centralised visibility. | ![Stars](https://img.shields.io/github/stars/armandofcom/ECS-RDS-Control-Dashboard?style=flat-square&color=FF9900) |
| [**awscert**](https://github.com/syscu-es/awscert) | AWS certification practice-exam simulator covering all current AWS certifications. | ![Stars](https://img.shields.io/github/stars/syscu-es/awscert?style=flat-square&color=FF9900) |

## ✍️ Recent writing

On [LinkedIn](https://www.linkedin.com/in/armandofcom/recent-activity/all/), in Spanish:

- **«Un agente de IA sin guardrails es una API pública con imaginación»** — a Bedrock AgentCore reference flow, simulated with and without guardrails.
- **«El meme es un chiste. La factura no.»** — ECS Gateway: 25 ALBs vs. one shared ALB, and where the saving stops being the point.
- **«Sácate la certificación y te cambia la carrera… ¿Seguro?»** — what an exam measures and what a senior's week actually looks like.
- **«La IA te va a ahorrar horas de trabajo… ¿Seguro?»** — who gets the hours AI frees up.

## 🏅 Certifications

| Certification | Issuer | Date |
|---|---|---|
| **AWS Certified Solutions Architect – Associate** | AWS | Sep 2024 |
| **AWS Certified Cloud Practitioner** | AWS | Dec 2023 |
| **Well-Architected Proficient** | AWS | Nov 2024 |
| DevOps Professional Certificate | PagerDuty × LinkedIn | Jun 2026 |
| Introduction to FinOps (course) | FinOps Foundation | Aug 2025 |

<details>
<summary><b>🎓 Training badges — 84 on Credly</b> (learning credentials, not professional certifications)</summary>
<br/>

- **AWS Partner:** Kiro Learning Plan · Agentic AI Essentials · Generative AI Essentials · Cloud Operations Essentials · DevOps Essentials · Cloud Economics Essentials · Migration Acceleration Program Authorized
- **Linux Foundation:** Kubernetes · OpenTofu · GitOps · OpenTelemetry · Istio · Jenkins · DevSecOps for Managers · DevOps & SRE
- **Google:** Cybersecurity Professional Certificate · IT Automation with Python · Apigee X
- **Others:** LPI Linux Essentials · Cisco networking and cybersecurity paths · Scrum Foundation

All of them, verifiable, on [Credly](https://www.credly.com/users/armandofcom/badges).

</details>

## 🌍 Community

- 🇨🇺 **SysAdmins de Cuba** — CEO and community lead, 2016–2024: IT professionals sharing systems, Linux, DevOps and cloud knowledge.
- 🐧 **GUTL** (Free Technology Users Group) — coordinator since 2010 · **CubaConf** — event organiser since 2016.
- 📡 **FRCUBA** — designed the internet connectivity and routing for the Cuban radio amateurs' federation, serving about 3,900 users.

## 🐍 Activity

<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/armandofcom/armandofcom/output/github-contribution-grid-snake-dark.svg"/>
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/armandofcom/armandofcom/output/github-contribution-grid-snake.svg"/>
  <img alt="Contribution snake" src="https://raw.githubusercontent.com/armandofcom/armandofcom/output/github-contribution-grid-snake-dark.svg"/>
</picture>

</div>

<details>
<summary><b>🇪🇸 Resumen en español</b></summary>
<br/>

Soy **Armando Felipe**, arquitecto cloud en España. Diseño plataformas AWS seguras y eficientes en costes (landing zones multi-cuenta, EKS/ECS, Terraform), con DevSecOps, SRE y FinOps. Fundé **[SysCu](https://www.syscu.es/)**, consultora de DevOps y FinOps en AWS para empresas en España, y lideré durante siete años la comunidad **SysAdmins de Cuba**.

¿Quieres bajar tu factura de AWS? [Pide el diagnóstico gratuito](https://www.syscu.es/contacto).

</details>

<div align="center">
<sub>SysAdmin de alma · Cloud Architect de profesión · DevSecOps por responsabilidad · SRE porque producción no perdona · FinOps para que AWS no te cobre hasta los pensamientos.</sub>
</div>
