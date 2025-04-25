# 🧠 Go Tasking

**Go Tasking** is a simple, full-stack task management application built with Go and React (Vite). It provides secure authentication (JWT + OAuth2), task CRUD operations, and a modern DevOps workflow with Docker, Terraform, and CI/CD.

---

## 🛠️ Tech Stack

### Frontend
- **Vite + React** — fast, modern UI

### Backend
- **Go** — RESTful API with:
  - Task CRUD (title, description, status, etc.)
  - JWT-based auth (signup, login, logout)
  - OAuth2 (Google/AWS Cognito)

### Database
- **PostgreSQL** (local)
- **Amazon RDS** (production)

### Infrastructure
- **Docker** — containerized app
- **Terraform** — provision AWS resources (EC2, RDS, etc.)
- **CI/CD** — GitHub Actions for testing and deployment

### Monitoring
- **Development**: Prometheus + Grafana
- **Production**: AWS CloudWatch

---

## 🌎 Environments

| Feature         | Development         | Production           |
|-----------------|---------------------|-----------------------|
| Host            | Local machine        | AWS EC2               |
| OAuth2 Provider | Google OAuth2        | AWS Cognito           |
| Database        | PostgreSQL (Docker)  | Amazon RDS            |
| Monitoring      | Prometheus + Grafana | CloudWatch            |

---

## 🚀 Getting Started

1. Clone the repo  
   `git clone https://github.com/your-org/go-tasking.git`

2. Start dev environment  
   `docker-compose up --build`

3. Visit the frontend at  
   `http://localhost:5173`

---

## 📂 Project Structure

```bash
task-manager/
├── cmd/                # Entry point (main.go)
├── internal/           # Business logic
├── api/                # HTTP handlers and requests
├── config/             # Config loader
├── pkg/                # Utilities (db, jwt, oauth)
├── web/                # React frontend
├── migrations/         # DB migrations
├── scripts/            # Dev scripts
├── Dockerfile
├── docker-compose.yml
├── .github/workflows/  # GitHub Actions
└── README.md
```

---

## ✅ License

MIT License

