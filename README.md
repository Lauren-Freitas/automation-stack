🚀 Automation Stack

Production-ready self-hosted automation infrastructure powered by Docker Swarm.

This project provides a scalable and modular stack focused on workflow automation, chatbot infrastructure, WhatsApp integration, AI-ready services, and self-hosted cloud tools.

📦 Stack Overview
Core Infrastructure
Traefik (Reverse Proxy + SSL)
Docker Swarm
Portainer
Redis
PostgreSQL
MySQL
MinIO (S3-compatible storage)
⚡ Automation & AI
n8n → workflow automation
Evolution API → WhatsApp API integration
Typebot → conversational chatbot builder
pgvector → vector database support for AI applications
🔐 Features
Automatic HTTPS with Let's Encrypt
Reverse proxy with Traefik
Docker Swarm orchestration
Persistent data volumes
Overlay networking
Environment variable management
Self-hosted object storage
AI-ready infrastructure
Modular stack architecture
Production-ready deployment structure
🏗️ Architecture
Internet
   │
   ▼
Traefik (SSL + Reverse Proxy)
   │
   ├── Portainer
   ├── n8n
   ├── Evolution API
   ├── Typebot
   ├── MinIO
   │
   ├── PostgreSQL
   ├── MySQL
   └── Redis
📁 Project Structure
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
└── README.md
⚙️ Requirements
Docker
Docker Swarm
Linux VPS
Domain configured with DNS records
Ports 80 and 443 open
🚀 Deployment

Initialize Docker Swarm:

docker swarm init

Deploy stacks:

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
🔑 Environment Variables

All sensitive credentials are managed through .env.

Example:

MYSQL_ROOT_PASSWORD=
POSTGRES_PASSWORD=
EVOLUTION_API_KEY=
TYPEBOT_SMTP_PASSWORD=
MINIO_ROOT_PASSWORD=
📌 Services
Service	Purpose
Traefik	Reverse proxy and SSL
Portainer	Docker management UI
PostgreSQL	Main relational database
MySQL	Evolution API database
Redis	Cache and sessions
Evolution API	WhatsApp integration
n8n	Workflow automation
Typebot	Chatbot platform
MinIO	S3-compatible object storage
pgvector	Vector database extension
🔒 Security
Secrets managed with environment variables
HTTPS enabled with Let's Encrypt
Services isolated through overlay networks
Infrastructure versioned with Git
📈 Future Improvements
Docker Secrets
CI/CD pipeline
Automated backups
Monitoring stack
High availability nodes
Infrastructure as Code improvements

📄 License
This project is intended for educational and self-hosted automation purposes.


# 👩‍💻 Author

Lauren Freitas

- GitHub: https://github.com/Lauren-Freitas
- LinkedIn: https://www.linkedin.com/in/laurend-freitas
