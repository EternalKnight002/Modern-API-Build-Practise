# 🚀 Modern API Build Practice

A high-performance laboratory for mastering backend engineering. This repository tracks my journey from building basic REST APIs to deploying scalable, secure, and containerized microservices.

## 🛠️ Tech Stack Evolution
As I progress, I am integrating the following technologies into my builds:
* **Runtime & Framework:** Node.js, Express.js
* [cite_start]**Databases:** PostgreSQL (via `pg` & Prisma ORM) [cite: 1]
* **Communication:** REST & GraphQL
* [cite_start]**DevOps & Infrastructure:** Docker, Docker Compose, Kubernetes, AWS [cite: 1]
* **Security:** JWT Authentication, Bcrypt, and Middleware-driven protection

---

## 🚀 Getting Started

### Prerequisites
* [Docker Desktop](https://www.docker.com/products/docker-desktop/) installed.
* [VS Code REST Client](https://marketplace.visualstudio.com/items?itemName=humao.rest-client) (for testing endpoints).

### Running a Project
1.  **Navigate to a specific API folder:**
    ```bash
    cd API1
    ```
2.  **Spin up the infrastructure:**
    ```bash
    docker-compose up --build
    ```
3.  **Initialize the Environment:**
    * For `API1`, use the `apitest.rest` file to run the `GET /setup` request to initialize the PostgreSQL tables.
    * For later projects, this will include running Prisma migrations: `npx prisma migrate dev`.

---

## 🧪 Testing & Debugging
Each project folder contains an `apitest.rest` file configured for its specific environment. 

* **REST API:** Use the `apitest.rest` file to trigger requests directly from VS Code.
* [cite_start]**Docker Health:** Run `docker ps` to ensure your app (Port 3000) and DB (Port 5432) are healthy and mapped correctly[cite: 2, 4].

---

## 🗺️ Learning Roadmap & Milestones

### Phase 1: Foundations
- [x] [cite_start]CRUD with Node.js & PostgreSQL [cite: 1]
- [x] [cite_start]Containerization with Docker & Docker Compose [cite: 2, 4]
- [x] Environment abstraction and `.gitignore` safety

### Phase 2: Modern Tooling
- [ ] Transitioning to **Prisma ORM** for type-safe DB queries.
- [ ] Implementing **GraphQL** for flexible data fetching.
- [ ] Centralized **Authentication (JWT)** and password hashing.

### Phase 3: Cloud & Orchestration
- [ ] Deploying to **AWS** (EC2/ECS/RDS).
- [ ] Container orchestration using **Kubernetes (K8s)**.
- [ ] Implementing CI/CD pipelines for automated testing and deployment.

---
## LICENSE

All the API's within this project are licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
##

*Created by EternalKnight002 — Built to learn, optimized for scale.*