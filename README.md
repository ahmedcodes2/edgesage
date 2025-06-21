# EdgeSage

**EdgeSage** is a cloud-native, event-driven user analytics and personalization platform. It enables websites and applications to track user behavior and serve dynamic, personalized experiences — all powered by edge computing and scalable architecture.

> Think of it as your own lightweight alternative to Google Analytics, tailored for modern, privacy-aware, and performance-critical environments.

---

## 🌐 Architecture Overview

EdgeSage is built on a modular, microservice-inspired architecture and currently includes:

- **TurboRepo** for monorepo management
- **Next.js** for the frontend and admin dashboard
- **Node.js (Express)** for backend services
- **AWS Lambda + Kinesis** for scalable, serverless ingestion
- **PostgreSQL + Redis** (planned) for data persistence and caching

---

## 📦 Modules

- `apps/sdk` – Lightweight JavaScript SDK for integration
- `apps/ingestion-api` – Receives user activity and pushes to event stream
- `apps/config-api` – Serves dynamic config for personalization
- `apps/admin-panel` – Dashboard to manage user accounts, keys, and analytics

---

## 🚀 Goals

- Near real-time user event ingestion
- Customization APIs to deliver tailored site behavior
- Plug-and-play SDK for third-party sites
- Scalable backend with future support for machine learning-based personalization

---

## 📚 Tech Stack

| Area         | Tech         |
|--------------|--------------|
| Frontend     | Next.js      |
| Backend APIs | Node.js + Express |
| Monorepo     | TurboRepo    |
| Event System | AWS Kinesis (planned) |
| Infra as Code | Terraform (planned) |

---

## 🛠️ Getting Started

1. Clone this repo
2. Run `npm install` at the root
3. Start individual apps using Turbo:

```bash
npx turbo run dev
