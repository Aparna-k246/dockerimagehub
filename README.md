# 🌍 Flask Hello World - Dockerized App

A minimal 🧪 **Flask web app** that returns "Hello World!" — containerized with **Docker** and ready for CI/CD workflows!

---

## 🚀 Tech Stack

- 🐍 Python
- 🌐 Flask
- 🐳 Docker
- 🤖 GitHub Actions (Optional for CI/CD)

---

## 📝 Source Code

```python
from flask import Flask

app = Flask(__name__)

@app.route("/")
def home():
    return "Hello World!"

if __name__ == "__main__":
    app.run(host="0.0.0.0", port=5000)
```

---

## 📁 File Structure

```bash
.
├── app.py              # Flask app
├── Dockerfile          # Docker image instructions
├── requirements.txt    # Flask dependency
├── test_app.py         # Optional - unit test
└── README.md           # Project overview
```

---

## 🐳 Docker Instructions

### 🔧 Build Docker Image

```bash
docker build -t flask-hello-app .
```

### ▶️ Run the App

```bash
docker run -p 5000:5000 flask-hello-app
```

Then visit: [http://localhost:5000](http://localhost:5000)

---

## ✅ Example Output

```bash
$ curl http://localhost:5000
Hello World!
```

---

## 🔁 Optional CI/CD Workflow

You can add `.github/workflows/flask-ci.yml` to automate testing & docker build on push.

---

## 💼 For Recruiters & Interviewers

This mini project demonstrates:

- Dockerizing a Python Flask app
- Exposing endpoints via container
- CI/CD readiness via GitHub Actions
- Basics of containerized microservices

---

## 🤝 Connect with Me

- 🔗 [LinkedIn](https://www.linkedin.com/in/aparna-k-628005167/)
- 💻 [GitHub](https://github.com/Aparna-k246)

---

## 📝 License

MIT License – free to use, share & modify.
