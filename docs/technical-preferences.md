# Tech Stack Preferences

This document outlines my preferred technologies, tools, and practices when building and deploying full-stack applications.

---

## Backend
- **Language:** Python 3.11+
- **Framework:** Flask 2.3+
- **ORM:** SQLAlchemy
- **Database:** MySQL
- **API Design:** RESTful services (JSON-first)

---

## Frontend
- **Framework/Library:** React with TypeScript
- **UI Framework:** Bootstrap 5.3+
- **Testing:**  
  - **Unit Testing:** Jest  
  - **End-to-End Testing:** Cypress 13+ with **Gherkin pattern**

---

## Development & Deployment
- **Local Development:** Docker Compose
- **Deployment Environment:** AWS Containers (ECS or Fargate)
- **CI/CD:** Containerized workflows with automated testing before deploy

---

## Security
- **Encryption:** TLS 1.3, AES-256
- **Authentication:** OAuth 2.0 / JWT
- **Passwordless Authentication:** Always prefer **magic link pattern** over traditional passwords
- **Local Testing for Magic Links:** MailHog

---

## Additional Notes
- Emphasis on maintainability, test coverage, and clear API contracts.
- Consistent use of TypeScript interfaces and Python dataclasses for type safety.
- Prefer containerization across all environments for reproducibility.

---
