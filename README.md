<!-- ═══════════════════════════════════════════════════════════════ -->
<!--  HERO — Animated wave banner (capsule-render)                    -->
<!-- ═══════════════════════════════════════════════════════════════ -->

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:232F3E,50:FF9900,100:232F3E&height=200&section=header&text=Armando&fontSize=70&fontColor=ffffff&animation=fadeIn&desc=AWS%20Cloud%20Architect%20%7C%20DevSecOps%20%7C%20SRE%20%7C%20FinOps&descSize=20&descAlignY=75" width="100%"/>

<!-- Typing animation — one focused element, AWS orange -->
<a href="https://git.io/typing-svg">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&duration=3000&pause=1000&color=FF9900&center=true&vCenter=true&width=800&height=50&lines=I+architect+secure%2C+cost-efficient+AWS+platforms;Multi-account+landing+zones+%7C+EKS+%7C+Terraform;Everything+as+Code.+Everything+observable.;If+it's+not+automated%2C+it's+not+finished." alt="Typing SVG" />
</a>

<br/><br/>

<!-- Contact row — 4 badges max, all functional -->
<a href="https://www.linkedin.com/in/armandofcom/"><img src="https://img.shields.io/badge/LinkedIn-armandofcom-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
<a href="https://www.syscu.es/"><img src="https://img.shields.io/badge/SysCu-syscu.es-FF9900?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Website"/></a>
<a href="https://www.credly.com/users/armandofcom/badges"><img src="https://img.shields.io/badge/Credly-Certifications-FF6B00?style=for-the-badge&logo=credly&logoColor=white" alt="Credly"/></a>
<a href="mailto:armandof@armandof.com"><img src="https://img.shields.io/badge/Email-Contact_Me-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/></a>

<br/><br/>

<img src="https://komarev.com/ghpvc/?username=armandofcom&color=FF9900&style=for-the-badge&label=PROFILE+VIEWS" alt="Profile views"/>

</div>

<br/>

<!-- ═══════════════════════════════════════════════════════════════ -->
<!--  ABOUT                                                           -->
<!-- ═══════════════════════════════════════════════════════════════ -->

## 🧑‍🚀 whoami

```hcl
resource "human" "armando" {
  role       = "Cloud Architect"
  location   = "Madrid, Spain 🇪🇸"
  origin     = "Linux / UNIX SysAdmin — I know what 3 AM on-call feels like"

  domains    = ["AWS", "DevSecOps", "SRE", "FinOps", "Platform Engineering"]

  builds = [
    "Multi-account AWS landing zones with governance baked in",
    "Reusable Terraform / OpenTofu modules teams can actually maintain",
    "EKS / ECS platforms with real observability, not just dashboards",
    "CI/CD pipelines that are fast, secure and repeatable",
    "FinOps visibility so AWS doesn't bill you for your thoughts",
  ]

  community  = ["Founder @ SysAdminsdeCuba", "Founder @ SysCu"]

  philosophy = "Automate everything you repeat twice."
}
```

<br/>

<!-- ═══════════════════════════════════════════════════════════════ -->
<!--  ARCHITECTURE — a Cloud Architect shows, not tells               -->
<!--  Mermaid renders natively on GitHub                              -->
<!-- ═══════════════════════════════════════════════════════════════ -->

## 🏗️ How I think — a reference architecture

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

> **Security by design. Observability by default. Cost-awareness always.**

<br/>

<!-- ═══════════════════════════════════════════════════════════════ -->
<!--  WHAT I DO                                                       -->
<!-- ═══════════════════════════════════════════════════════════════ -->

## 🧭 What I do

<table>
  <tr>
    <td width="33%" align="center">
      <h3>☁️</h3>
      <b>Cloud Architecture</b>
      <p align="left">Multi-account AWS, landing zones, networking, IAM, security baselines and production-ready designs that scale.</p>
    </td>
    <td width="33%" align="center">
      <h3>🧱</h3>
      <b>Infrastructure as Code</b>
      <p align="left">Terraform / OpenTofu modules, GitOps workflows, environment promotion and automated delivery.</p>
    </td>
    <td width="33%" align="center">
      <h3>🐳</h3>
      <b>Kubernetes & Containers</b>
      <p align="left">EKS, ECS Fargate, Helm, ArgoCD, autoscaling, ingress and operational best practices.</p>
    </td>
  </tr>
  <tr>
    <td width="33%" align="center">
      <h3>🔐</h3>
      <b>DevSecOps</b>
      <p align="left">Security from the design phase: secrets, scanning, compliance, auditability, controlled pipelines.</p>
    </td>
    <td width="33%" align="center">
      <h3>📊</h3>
      <b>Observability & SRE</b>
      <p align="left">Metrics, logs, traces, SLOs, alerting and systems you can understand under pressure.</p>
    </td>
    <td width="33%" align="center">
      <h3>💸</h3>
      <b>FinOps</b>
      <p align="left">Cost allocation, tagging strategies, rightsizing and making spend visible to engineering & business.</p>
    </td>
  </tr>
</table>

<br/>

<!-- ═══════════════════════════════════════════════════════════════ -->
<!--  TECH STACK — skill-icons: modern, clean, no badge walls         -->
<!-- ═══════════════════════════════════════════════════════════════ -->

## 🛠️ Tech Stack

<div align="center">

### ☁️ Cloud & Platform
<img src="https://skillicons.dev/icons?i=aws,gcp,azure,cloudflare,linux&theme=dark" alt="Cloud"/>

### 🧱 IaC & Automation
<img src="https://skillicons.dev/icons?i=terraform,ansible,bash,py,go&theme=dark" alt="IaC"/>

### 🐳 Containers & GitOps
<img src="https://skillicons.dev/icons?i=docker,kubernetes,helm&theme=dark" alt="Containers"/>
<img src="https://img.shields.io/badge/EKS-FF9900?style=for-the-badge&logo=amazoneks&logoColor=white" alt="EKS"/>
<img src="https://img.shields.io/badge/ArgoCD-EF7B4D?style=for-the-badge&logo=argo&logoColor=white" alt="ArgoCD"/>

### 🔐 Security & Observability
<img src="https://skillicons.dev/icons?i=prometheus,grafana&theme=dark" alt="Observability"/>
<img src="https://img.shields.io/badge/Vault-FFEC6E?style=for-the-badge&logo=vault&logoColor=black" alt="Vault"/>
<img src="https://img.shields.io/badge/Wazuh-005571?style=for-the-badge&logo=wazuh&logoColor=white" alt="Wazuh"/>
<img src="https://img.shields.io/badge/CloudWatch-FF4F8B?style=for-the-badge&logo=amazoncloudwatch&logoColor=white" alt="CloudWatch"/>

### 🗄️ Data & CI/CD
<img src="https://skillicons.dev/icons?i=postgres,mysql,mongodb,redis,rabbitmq,githubactions,gitlab,jenkins,git&theme=dark" alt="Data & CI/CD"/>

</div>

<details>
<summary><b>📌 Full engineering map (click to expand)</b></summary>
<br/>

```txt
Cloud Architecture     AWS (core), GCP, Azure, Apigee X, Cloudflare
AWS Services           VPC · IAM · Organizations · RDS/Aurora · ECS · EKS · Lambda · S3 · CloudFront · Route 53
Containers             Docker · EKS · ECS Fargate · Helm · ArgoCD · OpenShift
IaC                    Terraform · OpenTofu · CloudFormation · Ansible
DevSecOps              Prowler · SonarCloud · Wazuh · OpenVAS · Vault · Consul · PKI
Observability          CloudWatch · Prometheus · Grafana · OpenSearch · Sentry
FinOps                 Cost Explorer · CUR / Data Exports · Tagging · Dashboards · Rightsizing
Databases              PostgreSQL · Aurora · MySQL · MongoDB · Redis
CI/CD                  GitHub Actions · GitLab CI · Bitbucket Pipelines · Jenkins
Languages              Bash · Python · Go · HCL · YAML (unfortunately fluent)
```

</details>

<br/>

<!-- ═══════════════════════════════════════════════════════════════ -->
<!--  CURRENT FOCUS                                                   -->
<!-- ═══════════════════════════════════════════════════════════════ -->

## 🚀 Current focus

- 🏛️ Designing **secure multi-account AWS architectures** for real production environments
- 🧩 Building reusable **Terraform/OpenTofu modules** and automation patterns
- ☸️ Running **EKS/ECS workloads** with observability and reliability built-in
- 🤖 Applying **AI to operations**: automation, documentation and cloud workflows
- 📉 Creating **FinOps dashboards** and cost optimization strategies
- 🌱 Growing **[SysCu](https://www.syscu.es/)** — cloud, FinOps, observability & automation

<br/>

<!-- ═══════════════════════════════════════════════════════════════ -->
<!--  GITHUB ANALYTICS — one clean unified block                      -->
<!-- ═══════════════════════════════════════════════════════════════ -->

## 📊 GitHub Analytics

<div align="center">

<img height="170" src="https://github-readme-stats.vercel.app/api?username=armandofcom&show_icons=true&theme=github_dark&hide_border=true&bg_color=0d1117&title_color=FF9900&icon_color=FF9900&rank_icon=github" alt="GitHub Stats"/>
<img height="170" src="https://github-readme-stats.vercel.app/api/top-langs/?username=armandofcom&layout=compact&theme=github_dark&hide_border=true&bg_color=0d1117&title_color=FF9900" alt="Top Languages"/>

<br/><br/>

<img src="https://streak-stats.demolab.com/?user=armandofcom&theme=dark&hide_border=true&background=0d1117&ring=FF9900&fire=FF9900&currStreakLabel=FF9900" alt="GitHub Streak"/>

<br/><br/>

<img src="https://github-readme-activity-graph.vercel.app/graph?username=armandofcom&bg_color=0d1117&color=FF9900&line=FF9900&point=ffffff&area=true&hide_border=true" alt="Activity Graph"/>

<br/><br/>

<!-- 🐍 Contribution Snake — requires the GitHub Action (see snake.yml) -->
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/armandofcom/armandofcom/output/github-contribution-grid-snake-dark.svg"/>
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/armandofcom/armandofcom/output/github-contribution-grid-snake.svg"/>
  <img src="https://raw.githubusercontent.com/armandofcom/armandofcom/output/github-contribution-grid-snake-dark.svg" alt="Contribution snake"/>
</picture>

</div>

<br/>

<!-- ═══════════════════════════════════════════════════════════════ -->
<!--  CERTIFICATIONS                                                  -->
<!-- ═══════════════════════════════════════════════════════════════ -->

## 🏅 Certifications & Learning

<div align="center">

<a href="https://www.credly.com/users/armandofcom/badges"><img src="https://img.shields.io/badge/AWS-Certified-232F3E?style=for-the-badge&logo=amazonwebservices&logoColor=FF9900" alt="AWS"/></a>
<a href="https://www.credly.com/users/armandofcom/badges"><img src="https://img.shields.io/badge/HashiCorp-Terraform-623CE4?style=for-the-badge&logo=terraform&logoColor=white" alt="Terraform"/></a>
<a href="https://www.credly.com/users/armandofcom/badges"><img src="https://img.shields.io/badge/Kubernetes-Cloud_Native-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white" alt="Kubernetes"/></a>
<a href="https://www.credly.com/users/armandofcom/badges"><img src="https://img.shields.io/badge/Linux_Foundation-Learning-FCC624?style=for-the-badge&logo=linuxfoundation&logoColor=black" alt="Linux Foundation"/></a>

<sub>👉 All verified badges on <a href="https://www.credly.com/users/armandofcom/badges">Credly</a></sub>

</div>

<br/>

<!-- ═══════════════════════════════════════════════════════════════ -->
<!--  COMMUNITY & COLLABORATION                                       -->
<!-- ═══════════════════════════════════════════════════════════════ -->

## 🌍 Community

- 🇨🇺 Founder of **SysAdminsdeCuba** — systems, Linux, DevOps and cloud knowledge community
- 🚀 Founder of **[SysCu](https://www.syscu.es/)** — cloud, automation, FinOps, observability & AI applied to operations
- 🇪🇸 Active in AWS, DevOps, SRE and automation communities in Spain

## 🤝 Let's collaborate on

<div align="center">

| ☁️ Cloud Migration | 🔐 DevSecOps | 💸 FinOps |
|:---:|:---:|:---:|
| Architecture, security and cost control from day one | Secure pipelines & workloads from the design phase | Understand, allocate and optimize cloud spend |
| **📊 Observability** | **🐳 Kubernetes** | **🧱 IaC** |
| Metrics, logs and alerts that actually help | EKS, Helm, GitOps & operational excellence | Reusable modules & repeatable delivery |

</div>

<br/>

<!-- ═══════════════════════════════════════════════════════════════ -->
<!--  FOOTER                                                          -->
<!-- ═══════════════════════════════════════════════════════════════ -->

<div align="center">

```txt
SysAdmin de alma.
Cloud Architect de profesión.
DevSecOps por responsabilidad.
SRE porque producción no perdona.
FinOps para que AWS no te cobre hasta los pensamientos.
```

<br/>

<a href="https://www.linkedin.com/in/armandofcom/"><img src="https://img.shields.io/badge/-LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
<a href="https://github.com/armandofcom"><img src="https://img.shields.io/badge/-GitHub-181717?style=flat-square&logo=github&logoColor=white" alt="GitHub"/></a>
<a href="https://www.syscu.es/"><img src="https://img.shields.io/badge/-SysCu-FF9900?style=flat-square&logo=googlechrome&logoColor=white" alt="SysCu"/></a>
<a href="mailto:armandof@armandof.com"><img src="https://img.shields.io/badge/-Email-EA4335?style=flat-square&logo=gmail&logoColor=white" alt="Email"/></a>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:232F3E,50:FF9900,100:232F3E&height=120&section=footer" width="100%"/>

</div>