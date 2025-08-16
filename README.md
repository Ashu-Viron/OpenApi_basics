# OpenApi_basics

A minimal, hands-on example demonstrating how to integrate OpenAPI with a TypeScript + Hono backend deployed on Cloudflare Workers.
Just like FastAPI, this setup provides a centralized interface to explore, test, and document your API using Swagger UI, powered by the OpenAPI schema defined in spec.json.

You don’t need Postman or any external tool — simply run the app and test all your API endpoints directly in the browser through an interactive Swagger interface.

---

##  Table of Contents

- [Features](#features)  
- [Prerequisites](#prerequisites)  
- [Quick Start](#quick-start)  
- [Usage](#usage)  
- [OpenAPI Integration](#openapi-integration)  
- [Deployment](#deployment)  
- [Project Structure](#project-structure)  
- [Contributing](#contributing)  
- [License](#license)

---

##  Features

- Simple **Hono-based** TypeScript API deployed via **Cloudflare Workers**  
- Embedded **OpenAPI spec** (`spec.json`) illustrating request and response schemas  
- Demonstrates local development, spec-driven validation, and deployment flow

---

##  Prerequisites

- [Node.js](https://nodejs.org/) and npm/yarn  
- [Wrangler CLI](https://developers.cloudflare.com/workers/cli-wrangler/) for serverless deployment  
- (Optional) Familiarity with Hono, Cloudflare Workers, and OpenAPI

---

##  Quick Start

Clone the repo:

```bash
git clone https://github.com/Ashu-Viron/OpenApi_basics.git
cd OpenApi_basics
```
## Install dependencies
```bash
npm install
```

## Run locally in development mode
```bash
npm run dev
```
---
## Usage
Once your app is running,you can
- Acess the API endpoints (e.g. GET /users/{id})
- Explore and test the OpenAPI documentation via your preferred tools(Swagger UI)

## OpenAPI Integration
The project includes a static `spec.json` file defining the API in OpenAPI format. To use it:
- Open your API documentation tool (e.g., Swagger Editor, Redoc)
- Load or link the spec.json from the repository
- Interactively explore and test the API directly from the UI

## Deployment
Deploy to Cloudflare Workers with
```bash
npm run deploy
```

## Project Structure
```bash
├── README.md               # Overview & setup
├── package.json
├── tsconfig.json
├── wrangler.jsonc          # Cloudflare Worker configuration
├── spec.json               # OpenAPI schema for the project
├── src/
│   └── index.ts            # Core API logic with Hono routes
└── dist/                   # (Optional) Built assets
```
---
## Video
https://github.com/user-attachments/assets/cd8e2b44-deca-4fd4-81bb-43a470a5e517

---
## License
Distributed under the [MIT License](LICENSE). See the LICENSE file for more details.

