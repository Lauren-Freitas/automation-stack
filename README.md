# 🚀 Automation Stack for Nutrition Clinics

![Docker](https://img.shields.io/badge/Docker-Swarm-blue)
![Traefik](https://img.shields.io/badge/Traefik-ReverseProxy-blueviolet)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-16-blue)
![Redis](https://img.shields.io/badge/Redis-Cache-red)
![Automation](https://img.shields.io/badge/Automation-Healthcare-success)

Production-ready self-hosted automation infrastructure designed to support nutrition clinics, healthcare workflows, chatbot systems and AI-powered automations.

This stack powers:

* patient communication
* WhatsApp automation
* workflow orchestration
* chatbot experiences
* media storage
* AI-ready workflows
* scalable self-hosted infrastructure

---

# ✨ Use Cases

* Automated patient onboarding
* Nutrition follow-up automation
* WhatsApp appointment reminders
* Lead qualification flows
* AI-powered workflows
* Chatbot-based support
* Internal clinic automations
* Secure self-hosted infrastructure

---

# 📦 Core Stack

## Infrastructure

* Traefik
* Docker Swarm
* Portainer
* PostgreSQL
* MySQL
* Redis
* MinIO

## Automation & AI

* n8n → workflow automation
* Evolution API → WhatsApp integration
* Typebot → conversational chatbot platform
* pgvector → vector database for AI applications

---

# 🔐 Features

* Automatic HTTPS with Let's Encrypt
* Reverse Proxy Architecture
* Persistent Volumes
* Overlay Networking
* Environment Variable Management
* AI-ready Infrastructure
* S3-compatible Storage
* Modular Stack Design
* Production-ready Deployment Structure

---

# 🏗️ Architecture

```text id="c2q9nr"
Internet
   │
   ▼
Traefik (SSL + Reverse Proxy)
   │
   ├── Typebot
   ├── Evolution API
   ├── n8n
   ├── MinIO
   ├── Portainer
   │
   ├── PostgreSQL
   ├── MySQL
   └── Redis
```

---

# 📁 Project Structure

```bash id="fz8f4f"
automation-stack/
│
├── traefik/
├── portainer/
├── postgres/
├── mysql/
├── redis/
├── pgvector/
├── evolution/
├── n8n/
├── typebot/
├── minio/
│
├── .env
├── .gitignore
└── README.md
```

---

# 🚀 Deployment

Initialize Docker Swarm:

```bash id="i4x03l"
docker swarm init
```

Deploy services:

```bash id="bhh6m2"
docker stack deploy -c docker-stack.yml traefik
docker stack deploy -c docker-stack.yml postgres
docker stack deploy -c docker-stack.yml mysql
docker stack deploy -c docker-stack.yml redis
docker stack deploy -c docker-stack.yml pgvector
docker stack deploy -c docker-stack.yml portainer
docker stack deploy -c docker-stack.yml evolution
docker stack deploy -c docker-stack.yml n8n
docker stack deploy -c docker-stack.yml typebot
docker stack deploy -c docker-stack.yml minio
```

---

# 🔒 Security

* Environment variable management
* HTTPS enabled with Let's Encrypt
* Isolated overlay networks
* Infrastructure versioned with Git
* Secrets removed from repository history

---

# 📈 Future Improvements

* Docker Secrets
* CI/CD pipelines
* Monitoring stack
* Automated backups
* Multi-node Swarm cluster
* Infrastructure as Code improvements

---

# 👩‍💻 Author

Lauren Freitas

* GitHub: [https://github.com/Lauren-Freitas](https://github.com/Lauren-Freitas)
* LinkedIn: [https://www.linkedin.com/in/lauren-freitas](https://www.linkedin.com/in/lauren-freitas)

---

Built for scalable healthcare automation, AI workflows and self-hosted infrastructure experiments.
