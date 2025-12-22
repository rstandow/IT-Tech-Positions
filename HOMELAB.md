# IT Homelab Guide: Learn by Doing

Building a homelab is one of the best ways to gain hands-on IT experience without risking production systems. This guide provides budget-friendly setups and skills to practice.

---

## Why Build a Homelab?

**Learning > Certifications**  
- Employers value hands-on experience over theoretical knowledge
- Breaking things in your homelab teaches more than any textbook
- Portfolio projects from homelab separate you from certificate-only candidates

**Skills You'll Gain:**
- Server administration (Linux, Windows Server)
- Networking fundamentals (VLANs, routing, firewalls)
- Virtualization (Proxmox, VMware, Docker, Kubernetes)
- Automation and scripting
- Troubleshooting and problem-solving under pressure

**Career Acceleration:**
- Help Desk → System Admin: Show you can manage servers
- System Admin → DevOps: Demonstrate CI/CD pipelines and automation
- Developer → SRE: Prove you understand infrastructure and monitoring

---

## Budget Tier 1: Under $500 (The Starter Lab)

**Target roles:** IT Support, Junior System Admin, Entry-Level DevOps

### Hardware Option A: Used Business PC

**What to buy:**
- **Dell OptiPlex 7040/7050** or **HP EliteDesk G3** (eBay: $150-$250)
  - Intel i5-6500 or better (quad core)
  - 16GB RAM minimum (upgrade to 32GB for $40-$60)
  - 256GB SSD (add 1TB HDD for storage: $30)
- **TP-Link Gigabit Switch (8-port)** ($25-$35)
- **Old router** for learning (check garage sales, free on Facebook Marketplace)

**Total: ~$300-$400**

### Hardware Option B: Raspberry Pi Cluster

**What to buy:**
- **3x Raspberry Pi 4 (4GB)** ($55 each = $165)
- **Cluster case with cooling** ($40)
- **3x microSD cards (64GB)** ($30)
- **USB power hub** ($25)
- **Gigabit switch** ($25)

**Total: ~$285**

### Software Stack (All Free)

**Operating Systems:**
- **Proxmox VE** (virtualization platform - run multiple VMs/containers)
- **Ubuntu Server 22.04 LTS** (most popular Linux server)
- **Docker** (containerization)
- **Portainer** (Docker GUI - easier learning curve)

**Networking:**
- **pfSense** (firewall/router OS - learn network security)
- **Pi-hole** (DNS-based ad blocker - learn DNS and networking)

**Services to Practice:**
- **Nginx** (web server)
- **PostgreSQL** or **MySQL** (databases)
- **Gitea** (self-hosted Git server)
- **Nextcloud** (self-hosted cloud storage)

### Skills to Practice

**Month 1-2: Fundamentals**
- [ ] Install Proxmox and create 3-4 virtual machines
- [ ] Set up Ubuntu Server via SSH (no GUI)
- [ ] Configure static IPs and basic networking
- [ ] Install and manage services (Nginx, MySQL)
- [ ] Practice Linux commands (users, permissions, file management)

**Month 3-4: Services & Automation**
- [ ] Deploy Docker containers (Portainer, Nextcloud, Gitea)
- [ ] Set up reverse proxy with Nginx
- [ ] Write bash scripts to automate backups
- [ ] Configure cron jobs for scheduled tasks
- [ ] Set up monitoring (Prometheus + Grafana free tier)

**Month 5-6: Networking & Security**
- [ ] Install pfSense as your homelab firewall
- [ ] Create VLANs to segment networks
- [ ] Set up VPN (WireGuard or OpenVPN)
- [ ] Configure firewall rules
- [ ] Practice SSH key authentication

**Portfolio Projects:**
- Personal website with CI/CD pipeline
- Monitoring dashboard for your homelab
- Automated backup system
- Self-hosted Git server with Gitea

---

## Budget Tier 2: $1,000-$1,500 (The Serious Lab)

**Target roles:** System Admin, DevOps Engineer, SRE, Cloud Engineer

### Hardware Setup

**Server:**
- **Dell PowerEdge R720** (eBay/ServerMonkey: $300-$500)
  - Dual Xeon E5-2670 (16 cores, 32 threads total)
  - 64GB-128GB DDR3 ECC RAM ($100-$200)
  - 4x 1TB SAS drives in RAID 10 ($120)
  - **OR** modern budget build: Refurb Dell T3620 with i7-7700, 32GB RAM ($400-$600)

**Networking:**
- **Managed switch (24-port Gigabit)** - TP-Link TL-SG1024DE ($120)
- **Used enterprise router/firewall** - Ubiquiti EdgeRouter or pfSense box ($150-$200)

**Optional:**
- **UPS (Uninterruptible Power Supply)** - CyberPower 1500VA ($150-$200)
- **NAS for storage** - Synology DS220+ or build TrueNAS ($400-$600)

**Total: ~$1,000-$1,500**

### Software Stack (Production-Grade)

**Virtualization:**
- **Proxmox VE** or **VMware ESXi** (free tier)
- **10-15 VMs** running simultaneously

**Container Orchestration:**
- **Kubernetes** (k3s for resource-efficient learning)
- **Docker Swarm** (simpler alternative)
- **Rancher** (Kubernetes management UI)

**Infrastructure as Code:**
- **Terraform** (provision infrastructure)
- **Ansible** (configuration management automation)
- **GitOps with FluxCD** or **ArgoCD**

**Monitoring & Observability:**
- **Prometheus + Grafana** (metrics and dashboards)
- **ELK Stack** (Elasticsearch, Logstash, Kibana) - log aggregation
- **Uptime Kuma** or **Statuspage** for service monitoring

**CI/CD Pipeline:**
- **Jenkins** or **GitLab CI/CD**
- **SonarQube** (code quality)
- **Nexus** or **Artifactory** (artifact repository)

**Security:**
- **pfSense** + **Snort/Suricata** (intrusion detection)
- **CrowdSec** (community-powered threat intelligence - blocks IPs attacking others' servers)
- **Traefik** (modern reverse proxy with automatic SSL, better than Nginx for containers)
- **Wazuh** (security monitoring)
- **Vault** (secrets management)

### Skills to Practice (Advanced)

**Months 1-3: Infrastructure Automation**
- [ ] Deploy Kubernetes cluster (3 nodes minimum)
- [ ] Use Terraform to provision VMs
- [ ] Automate server configuration with Ansible playbooks
- [ ] Set up GitOps workflow (infrastructure in Git)
- [ ] Implement Infrastructure as Code for entire lab

**Months 4-6: Production Simulation**
- [ ] Build full CI/CD pipeline (git push → automated deploy)
- [ ] Deploy microservices app on Kubernetes
- [ ] Configure service mesh (Istio or Linkerd)
- [ ] Set up high-availability (HA) database cluster
- [ ] Practice disaster recovery (break things, restore from backup)

**Months 7-9: Monitoring & SRE**
- [ ] Deploy Prometheus + Grafana for full observability
- [ ] Create SLO dashboards and error budgets
- [ ] Set up centralized logging with ELK stack
- [ ] Configure alerting (PagerDuty integration for "on-call" practice)
- [ ] Conduct chaos engineering experiments (kill random services, see what breaks)

**Months 10-12: Security & Scale**
- [ ] Implement zero-trust networking
- [ ] Configure mTLS (mutual TLS) between services
- [ ] Set up intrusion detection (Snort/Suricata)
- [ ] Practice security incident response
- [ ] Load test your applications (K6, Locust)

### Portfolio Projects (Job-Ready)

**DevOps Engineer:**
- Fully automated Kubernetes cluster deployed via Terraform
- Multi-environment CI/CD pipeline (dev, staging, prod)
- Complete monitoring stack with real dashboards

**SRE:**
- HA application with SLO/SLI dashboards
- Automated incident response runbooks
- Chaos engineering test results

**Cloud Engineer:**
- Hybrid cloud setup (homelab + AWS/GCP integration)
- Multi-region disaster recovery simulation
- Cost optimization documentation

---

## Homelab Learning Path by Career Goal

### Path 1: IT Support → System Administrator

**Hardware:** Budget Tier 1 ($300-$500)

**Focus:**
- Windows Server + Active Directory
- Basic Linux (Ubuntu/CentOS)
- Networking fundamentals
- Virtualization basics

**Key Projects:**
- Set up Active Directory domain
- Configure DHCP, DNS servers
- User/group management automation
- Basic PowerShell scripting

**Timeline:** 6-12 months

---

### Path 2: Developer → DevOps Engineer

**Hardware:** Budget Tier 2 ($1,000-$1,500)

**Focus:**
- CI/CD pipelines
- Docker and Kubernetes
- Infrastructure as Code (Terraform + Ansible)
- Monitoring and logging

**Key Projects:**
- Containerize applications
- Build automated deployment pipeline
- Deploy to Kubernetes
- Implement GitOps workflow

**Timeline:** 6-9 months (faster if already coding)

---

### Path 3: System Admin → Site Reliability Engineer

**Hardware:** Budget Tier 2 ($1,000-$1,500)

**Focus:**
- SLO/SLI/Error budgets
- Production incident response
- Observability (metrics, logs, traces)
- Automation and toil reduction

**Key Projects:**
- HA application deployment
- Complete monitoring stack
- Automated runbooks
- Load testing and chaos engineering

**Timeline:** 9-12 months

---

### Path 4: Cybersecurity Focus

**Hardware:** Budget Tier 1 or 2

**Focus:**
- Network security (pfSense, VLANs, firewall rules)
- Intrusion detection (Snort, Suricata, Wazuh)
- Security monitoring (SIEM with Wazuh or Security Onion)
- Vulnerability scanning

**Key Projects:**
- Segmented network with VLANs
- IDS/IPS implementation
- Security information dashboard
- Practice CTF challenges on your lab

**Timeline:** 6-12 months

---

## Cost Breakdown by Skill Level

| Experience Level | Budget | Hardware | What You Get |
|:---|:---|:---|:---|
| **Absolute Beginner** | $0-$200 | Old laptop + VirtualBox | Learn Linux, Docker basics, SSH |
| **Entry IT Support** | $300-$500 | Used business PC or Pi cluster | Virtualization, networking, basic services |
| **Mid-Career Pivot** | $1,000-$1,500 | Enterprise server + networking | Kubernetes, automation, production simulation |
| **Advanced / SRE** | $2,000-$3,000 | Multiple servers, NAS, UPS | HA clusters, disaster recovery, scale testing |

---

## Common Homelab Questions

**Q: Will my electricity bill skyrocket?**  
A: Budget Tier 1 uses ~50-100W ($5-$10/month). Tier 2 server can use 200-400W (~$20-$40/month). Consider used low-power servers or run them only when practicing.

**Q: Is noise an issue?**  
A: Yes - enterprise servers (Dell R720) have loud fans. Solutions: Run in garage/basement, buy quieter fans, or use modern low-power hardware (less learning value but quieter).

**Q: What if I break something?**  
A: That's the point! Homelab is for breaking things safely. Use VM snapshots before risky changes. Worst case: reinstall (good practice).

**Q: Can I use cloud (AWS Free Tier) instead?**  
A: Yes, but: Free tier is limited, costs creep up fast, and you don't learn hardware. Best approach: Homelab for foundation, then expand to hybrid (homelab + cloud).

**Q: How do I avoid "tutorial hell"?**  
A: Build projects with end goals. "Set up monitoring" is vague. "Build dashboard showing uptime of 5 services with alerts" is a project. Break things intentionally and fix them.

---

## Progression Timeline

**Months 1-3:** Basics (SSH, Linux, Docker, basic networking)  
**Months 4-6:** Services (web servers, databases, automation scripts)  
**Months 7-9:** Advanced (Kubernetes, CI/CD, monitoring)  
**Months 10-12:** Production simulation (HA, disaster recovery, chaos engineering)

**After 12 months:** You'll have portfolio projects and real experience to discuss in interviews. You'll know more than many people with certifications alone.

---

## Resources

**Communities:**
- r/homelab (Reddit - show off setups, get advice)
- r/selfhosted (Reddit - service recommendations)
- ServeTheHome forums (enterprise hardware deals)

**Learning:**
- **TechnoTim** (YouTube - homelab tutorials)
- **NetworkChuck** (YouTube - networking and homelab)
- **Awesome-Selfhosted** (GitHub - huge list of self-hostable services)
- **Learn Linux TV** (YouTube - Linux fundamentals)

**Where to Buy:**
- eBay, Facebook Marketplace (used hardware)
- ServerMonkey, TechMikeNY (refurbished enterprise gear)
- Micro Center (if near you - open box deals)

---

## Key Takeaway

**Your homelab is your portfolio.** When interviewers ask "Tell me about a time you troubleshot a complex issue," you have real stories. When they ask "Do you know Kubernetes?" you can show them your actual deployment.

Start small, break things, fix them, and document your learning. Your homelab is better than any certification for proving you can do the job.

---

**Last Updated:** December 2024 | **Next Review:** June 2025

---

## Documentation: The Skill That Separates Professionals from Hobbyists

**Critical Truth:** If you didn't document it, you didn't learn it. Documentation proves you understand what you built.

### What to Document

**1. Your Setup (Infrastructure Documentation)**
- Network diagram (what talks to what)
- Server inventory (hostname, IP, purpose, specs)
- Services running on each machine
- Backup procedures
- Disaster recovery plan

**2. Your Projects (Technical Documentation)**
- **Problem:** What were you trying to solve?
- **Solution:** How did you solve it (architecture, tools used)?
- **Challenges:** What broke? How did you fix it?
- **Results:** Screenshots, metrics, proof it works
- **Lessons Learned:** What would you do differently?

**3. Runbooks (Operational Documentation)**
- Step-by-step procedures for common tasks
- Troubleshooting guides ("If X breaks, do Y")
- Incident response procedures
- Rollback procedures

### How to Document (The IT Way)

**Option 1: Docs-as-Code (Professional Standard)**

Use **Markdown + Git** - same workflow as code:

```markdown
# Homelab Infrastructure

## Network Topology
[Diagram here]

## Servers
- **prox01**: Proxmox host (192.168.1.10)
  - CPU: i7-7700, 32GB RAM
  - VMs: k3s-master, gitlab-runner, monitoring

## Monitoring Setup
1. Install Prometheus
   ```bash
   docker run -d -p 9090:9090 prom/prometheus
   ```
2. Configure targets in prometheus.yml
3. Access at http://localhost:9090
```

**Tools:**
- **MkDocs** - Generates beautiful static site from markdown (free, open source)
- **Docusaurus** - Meta's documentation framework (free, very polished)
- **GitBook** - Clean docs site, free for open source
- **Wiki.js** - Self-hosted wiki with WYSIWYG editor

**Option 2: Self-Hosted Wiki**

- **BookStack** - Best for homelab documentation (free, self-hosted)
  - Organized in Books → Chapters → Pages
  - Markdown support, diagrams, code blocks
  - Easy to search and navigate
- **Outline** - Modern, collaborative wiki (free, self-hosted)
- **Wiki.js** - Feature-rich, supports multiple storage backends

**Option 3: Diagramming Tools**

- **draw.io (diagrams.net)** - Network diagrams, flowcharts (free, web-based or desktop)
- **Excalidraw** - Hand-drawn style diagrams (free, open source)
- **Mermaid** - Text-to-diagram in markdown (free, renders in GitHub/GitLab)

### Documentation Workflow

**1. Create a Git Repo for Your Homelab**
```bash
mkdir homelab-docs
cd homelab-docs
git init
```

**2. Structure Your Docs**
```
homelab-docs/
├── README.md              (Overview)
├── infrastructure/
│   ├── network.md
│   ├── servers.md
│   └── diagrams/
├── projects/
│   ├── kubernetes-cluster.md
│   ├── monitoring-stack.md
│   └── ci-cd-pipeline.md
├── runbooks/
│   ├── backup-restore.md
│   ├── incident-response.md
│   └── common-issues.md
└── changelog.md           (What changed when)
```

**3. Document as You Build**
- **Before:** What you're about to do and why
- **During:** Commands you ran, errors you hit, how you fixed them
- **After:** Final configuration, screenshots of working system

**4. Use MkDocs to Publish**
```bash
pip install mkdocs mkdocs-material
mkdocs new .
mkdocs serve  # View at http://localhost:8000
```

### What Employers Look For

**Portfolio on GitHub/GitLab:**
- **README.md** - Professional overview with screenshots
- **Architecture diagram** - Shows you understand system design
- **Step-by-step setup** - Proves you can communicate technical concepts
- **Troubleshooting section** - Shows problem-solving skills
- **Clean commits** - Demonstrates Git proficiency

**Example:**
> "Built HA Kubernetes cluster with automated CI/CD pipeline. [View documentation](https://yourname.github.io/homelab)"

Hiring managers click that link and see professional documentation = instant credibility.

### Documentation Tools Comparison

| Tool | Best For | Hosting | Learning Curve |
|:---|:---|:---|:---|
| **MkDocs + Material** | Technical docs, portfolios | GitHub Pages (free) | Low |
| **BookStack** | Self-hosted homelab wiki | Your server | Very Low |
| **Docusaurus** | Professional portfolios | GitHub Pages, Vercel | Medium |
| **Obsidian + Git** | Personal notes + version control | Your computer + GitHub | Low |
| **Wiki.js** | Feature-rich team wiki | Your server | Medium |

### Pro Tips

**1. Screenshot Everything**
- Before (broken state)
- During (error messages, troubleshooting steps)
- After (working dashboard, metrics)

**2. Version Control Your Configs**
Keep ALL config files in Git:
```bash
/etc/nginx/nginx.conf
/etc/docker/daemon.json
/home/user/docker-compose.yml
```

**3. Write Postmortems**
When something breaks badly:
- Timeline of events
- Root cause
- What you did to fix it
- How to prevent it next time

This is what SREs do at Google. Practice it in your homelab.

**4. Document Your Mistakes**
"I tried X, it failed because Y, learned Z" = valuable content. Employers want to see learning and problem-solving.

### Quick Start: Your First Doc

**In 15 minutes, create this:**

1. Create `homelab-README.md`:
```markdown
# My Homelab

## Hardware
- Dell OptiPlex 7050: Proxmox host, 32GB RAM
- Raspberry Pi 4: Pi-hole DNS

## Services Running
- Nginx reverse proxy
- Nextcloud (file storage)
- Gitea (Git server)
- Grafana + Prometheus (monitoring)

## Network Diagram
[Insert draw.io diagram]

## Recent Projects
- [Kubernetes Cluster Setup](projects/k8s-cluster.md)
- [Automated Backup System](projects/backups.md)

## Learned Skills
- Linux server administration
- Docker containerization
- Reverse proxy configuration
- Infrastructure monitoring
```

2. Push to GitHub
3. Add link to your resume

**Result:** You now have documented proof you can build and maintain IT infrastructure. That's more valuable than 5 certifications.

---


## Video Tutorials (Step-by-Step Setup Guides)

The best way to learn is watching someone do it, then doing it yourself. Here are the best YouTube channels and specific tutorials:

### Proxmox Setup

**TechnoTim - Proxmox Complete Setup**
- [Proxmox VE Install and Setup Tutorial](https://www.youtube.com/watch?v=GoZaMgEgrHw) - Complete beginner setup
- [Ultimate Beginner's Guide to Proxmox](https://www.youtube.com/watch?v=LCjuiIswXGs) - VMs, containers, networking

**Learn Linux TV**
- [Proxmox Full Course](https://www.youtube.com/watch?v=5j0Zb6x_hOk) - 14-part series covering everything
- [Proxmox Clustering](https://www.youtube.com/watch?v=Nb0JAf28y4I) - For advanced setup

### Docker & Kubernetes

**TechnoTim**
- [Docker Compose Tutorial](https://www.youtube.com/watch?v=DM65_JyGxCo)
- [k3s Kubernetes Cluster](https://www.youtube.com/watch?v=CbkEWcUZ7zM) - Lightweight K8s perfect for homelab

**NetworkChuck**
- [Docker Crash Course](https://www.youtube.com/watch?v=eGz9DS-aIeY) - Fun, beginner-friendly
- [You need to learn Kubernetes RIGHT NOW!!](https://www.youtube.com/watch?v=7bA0gTroJjw)

### pfSense / Firewall

**Lawrence Systems**
- [pfSense Complete Installation & Setup](https://www.youtube.com/watch?v=y2SXHgyMNiQ)
- [pfSense + VLANs Tutorial](https://www.youtube.com/watch?v=kBXcd0RvEZ8)

**NetworkChuck**
- [Build a Firewall with pfSense](https://www.youtube.com/watch?v=HO2ZIvEldSo)

### Monitoring (Prometheus + Grafana)

**TechnoTim**
- [Ultimate Grafana + Prometheus Setup](https://www.youtube.com/watch?v=h4Sl21AKiDg)
- [Monitor your Homelab with Netdata](https://www.youtube.com/watch?v=AJDv94KNmmo) - Easier alternative

### Traefik Reverse Proxy

**TechnoTim**
- [Traefik 2 Setup with Docker](https://www.youtube.com/watch?v=wLrmmh1eI94)
- [Traefik + LetsEncrypt + Docker](https://www.youtube.com/watch?v=liV3c9m_OX8) - Auto SSL

### CrowdSec Security

**TechnoTim**
- [Protect your Server with CrowdSec](https://www.youtube.com/watch?v=9kGW-LBSDac) - Community threat intelligence

### Automation (Terraform + Ansible)

**TechnoTim**
- [Terraform in 15 Minutes](https://www.youtube.com/watch?v=QyM92WFcbSE)
- [Ansible 101](https://www.youtube.com/watch?v=xRMPKQweySE)

**Jeff Geerling**
- [Ansible for Beginners](https://www.youtube.com/watch?v=goclfp6a2IQ) - Best Ansible teacher

### Recommended Channels to Subscribe

| Channel | Focus | Style |
|:---|:---|:---|
| **TechnoTim** | Homelab, Docker, K8s | Professional, step-by-step |
| **NetworkChuck** | Networking, security | Fun, energetic |
| **Learn Linux TV** | Linux, Proxmox | Detailed, thorough |
| **Lawrence Systems** | pfSense, networking | Business-focused |
| **Jeff Geerling** | Ansible, automation | Teaching-oriented |
| **Christian Lempa** | Cloud, DevOps | Concise, practical |

### Learning Path Videos

**Month 1-2: Foundations**
1. Watch TechnoTim's Proxmox setup
2. Follow along NetworkChuck's Docker course
3. Set up pfSense with Lawrence Systems guide

**Month 3-4: Services**
4. Deploy containers with TechnoTim's Docker Compose tutorial
5. Set up Traefik reverse proxy
6. Install Grafana monitoring

**Month 5-6: Advanced**
7. Build k3s cluster with TechnoTim
8. Learn Ansible with Jeff Geerling
9. Harden security with CrowdSec

**Pro Tip:** Don't just watch - pause video, do the step, verify it works, then continue. Passive watching ≠ learning.

---

