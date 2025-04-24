# 🥞 Scaling Pancake

> A fully automated CI/CD pipeline using **Docker**, **Python**, and **GitHub Actions** — designed to streamline testing, building, and deploying modern Python applications with DevOps best practices.

---

## 📐 Project Architecture

This project follows a clean and scalable structure, designed for modularity and ease of automation:

```
📦 scaling-pancake/
├── .github/workflows/       # GitHub Actions workflow for CI/CD
├── app/                     # Main application code
│   └── main.py              # Application entry point
├── tests/                   # Automated tests using Pytest
│   └── test_main.py         
├── Dockerfile               # Docker container definition
├── requirements.txt         # Project dependencies
└── README.md                # Project documentation
```

This layout promotes testability, consistency, and smooth DevOps integration.

---

## 🐳 Docker Containers

The included `Dockerfile` builds a lightweight Python environment tailored for:

- **Reproducibility**: Same environment across dev, test, and production.
- **Automated testing**: Runs unit tests at build time.
- **Portability**: Runs anywhere with Docker installed.

### Run Locally with Docker:

```bash
docker build -t scaling-pancake .
docker run --rm scaling-pancake
```

This ensures your local tests mirror production conditions exactly.

---

## ⚙️ CI/CD with GitHub Actions

This project uses **GitHub Actions** to fully automate its continuous integration and delivery pipeline.

### Workflow:

1. Code is pushed to the main branch.
2. GitHub Actions runs:
   - Dependency installation
   - Automated tests (`pytest`)
   - Docker build validation
3. If all tests pass, the project is ready for deployment.

This enables fast feedback and reliable delivery cycles.

---

## 🧠 DevOps Culture

This repository embraces core **DevOps** principles:

- **Continuous Integration (CI)**: Every push triggers automated testing.
- **Continuous Delivery (CD)**: Tested builds are deployment-ready.
- **Infrastructure as Code**: Environments defined through Docker and GitHub Actions.
- **Automated Feedback**: PRs and commits receive immediate test results.

The result: fewer bugs in production and shorter development cycles.

---

## 🐍 Python in the Project

Python serves as the backbone of this project due to its:

- Clean and readable syntax for scripting
- Rich ecosystem for testing (e.g. `pytest`)
- Rapid prototyping and integration capabilities

`main.py` represents the core application logic, and all functionality is covered by test cases under `tests/`.

---

## 🚀 Running Locally

```bash
# Clone the repository
git clone https://github.com/petersonchiquetto/scaling-pancake.git
cd scaling-pancake

# Install dependencies (if not using Docker)
pip install -r requirements.txt

# Run the app
python app/main.py

# Run tests
pytest
```

---

## 📄 License

This project is licensed under the MIT License. See the [LICENSE](https://github.com/petersonchiquetto/scaling-pancake/blob/main/LICENSE) file for more information.

---
