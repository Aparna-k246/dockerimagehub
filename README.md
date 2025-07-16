# 🐳 DockerImageHub - CI/CD FastAPI Template

A minimal ⚡ FastAPI project, fully containerized with **Docker**, integrated with **CI/CD workflows via GitHub Actions**, and supported by **unit tests** — perfect for scalable microservice deployment and DevOps readiness! 🧑‍💻

---

## 🚀 Tech Stack

- 🐍 **Python 3.10+**
- ⚡ **FastAPI**
- 🧪 **Pytest**
- 🐳 **Docker**
- 🤖 **CI/CD**: GitHub Actions
- 🔬 **Unit Testing**

---

## 🔧 Workflows

📁 `.github/workflows/cicd.yml`  
CI/CD workflow runs:

- ✅ Lint check
- 🧪 Unit test via `pytest`
- 🐳 Docker build

```yaml
# Sample steps (see full in repo)
- name: Test with pytest
  run: |
    pytest test_app.py
- name: Build Docker image
  run: |
    docker build -t dockerimagehub:latest .
```

---

## 📦 Folder Structure

```bash
dockerimagehub/
├── .github/
│   └── workflows/
│       └── cicd.yml         # CI/CD Workflow
├── .gitignore
├── app.py                   # FastAPI Application
├── Dockerfile               # Docker Setup
├── requirements.txt         # Project Dependencies
├── test_app.py              # Unit Tests
└── README.md                # Project Overview
```

---

## 🧪 Running the Project

### 🖥️ Locally

```bash
pip install -r requirements.txt
uvicorn app:app --reload
```

### 🐳 Docker

```bash
docker build -t dockerimagehub .
docker run -p 8000:8000 dockerimagehub
```

---

## ✅ Example API Response

```bash
GET http://localhost:8000/

{
  "message": "Hello, Dockerized FastAPI!"
}
```

---

## 🔁 CI/CD Automation

Every push triggers:

1. ✅ **Code lint & test**
2. 🐳 **Docker build validation**
3. 💥 Ideal for container-based deployment pipelines

---

## 💼 For Recruiters & Interviewers

📌 This repository demonstrates:

- Proficiency with **FastAPI**
- Strong understanding of **CI/CD pipelines**
- Experience with **Docker containers**
- Writing & running **automated unit tests**
- Building **clean, production-ready APIs**

⭐ Ideal for **backend**, **DevOps**, or **platform engineering** roles.

---

## 📸 UI or Terminal Screenshot (Optional)

> _You can add a screenshot here showing terminal running FastAPI in Docker or GitHub Actions run badge!_

---

## 🤝 Let's Connect!

- 🔗 [LinkedIn](https://www.linkedin.com/in/aparna-k-628005167/)
- 💻 [GitHub](https://github.com/Aparna-k246)

---

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
