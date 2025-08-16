# OpenApi_basics

A minimal, hands-on example demonstrating how to work with OpenAPI in a TypeScript setting—auto-generated documentation, deployment, and integration with APIs. Built with Hono on Cloudflare Workers and includes an OpenAPI spec (`spec.json`).

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
## License
Distributed under the [MIT License](LICENSE). See the LICENSE file for more details.

