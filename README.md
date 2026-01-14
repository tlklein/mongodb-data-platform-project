# Enterprise Data Platform Project

![Screenshot 2024-12-24 at 10 24 06 PM](398512429-b71af6f2-089b-4e80-9f96-f426f7773ac3.png)

## Project Overview

This project is a full-stack data platform (MEVN) that models how Community Health Workers (CHWs) manage events, client data, and service sign-ups. This iteration refactors a prototype into a maintainable, production-minded application with role-based access, dynamic service management, and interactive visualizations.

This project transformed an academic prototype into a production-ready data platform by addressing maintainability, security, and real-world usability gaps. The frontend was refactored to the Vue Composition API to improve code organization and extensibility, while secure authentication with role-based access control enabled differentiated Viewer and Editor workflows. Static service data was replaced with fully dynamic CRUD-backed APIs, and interactive dashboard visualizations were added to surface actionable client and event metrics. 

The result is a more maintainable, extensible, and analytics-driven application aligned with real-world Community Health Worker workflows. 

## Tech Stack

Frontend
- Vue.js 3 - Modern reactive UI framework using the Composition API
- Vite - Fast build tooling and local development server
- Tailwind CSS - Utility-first styling for rapid, consistent UI development
- Pinia - Lightweight, scalable state management
- Vuelidate - Declarative form validation for complex user inputs


Backend
- Node.js - JavaScript runtime for server-side logic
- Express.js - RESTful API framework for routing and middleware
- MongoDB - NoSQL document database for flexible data modeling
- Mongoose - ODM for schema enforcement, validation, and query abstraction


Architecture & Practices
- RESTful API design with clear separation of frontend and backend concerns
- Role-based access patterns enforced at the API and UI layers
- Modular component and service structure to improve maintainability and extensibility

## Repo Structure
```text
├── backend/                         # Node.js / Express backend (API + auth + data layer)
│   ├── auth/                        # Authentication & authorization logic
│   │   └── authMiddleWare.js        # Middleware enforcing authentication and role-based access
│   ├── models/                     # Database schema definitions
│   │   └── models.js               # Mongoose models for users, clients, events, services, orgs
│   ├── routes/                     # REST API route handlers
│   │   ├── clients.js              # CRUD endpoints for client records
│   │   ├── events.js               # Event scheduling and management APIs
│   │   ├── org.js                  # Organization-level configuration and metadata
│   │   ├── services.js             # Service catalog CRUD endpoints
│   │   └── users.js                # User management and role handling
│   ├── app.js                      # Express app entry point and middleware wiring
│   ├── create_hash.js              # Utility for generating hashed passwords (auth setup)
│   ├── package.json                # Backend dependencies and scripts
│   └── README.md                   # Backend-specific documentation
├── frontend/                       # Vue 3 frontend application
│   ├── public/                     # Static assets served directly
│   │   └── favicon.ico             # Application favicon
│   ├── src/                        # Frontend source code
│   │   ├── api/                    # API abstraction layer
│   │   │   └── api.js              # Centralized HTTP client for backend communication
│   │   ├── assets/                 # Static frontend assets
│   │   │   └── DanPersona.svg      # Branding / UI illustration asset
│   │   ├── components/             # Reusable UI components
│   │   │   ├── barChart.vue        # Dashboard bar chart visualization
│   │   │   └── donutZipChart.vue   # Donut chart for client distribution metrics
│   │   ├── router/                 # Client-side routing
│   │   │   └── index.js            # Vue Router configuration and route guards
│   │   ├── store/                  # State management (Pinia)
│   │   │   └── loggedInUser.js     # Authenticated user state and role context
│   │   ├── views/                  # Page-level components (routes)
│   │   │   ├── clientdetails.vue   # Client detail view
│   │   │   ├── clientform.vue      # Create/edit client workflow
│   │   │   ├── ConfirmationDialog.vue # Reusable confirmation modal
│   │   │   ├── eventDetials.vue    # Event detail view
│   │   │   ├── eventform.vue       # Create/edit event workflow
│   │   │   ├── findclient.vue      # Client search and discovery
│   │   │   ├── findevents.vue      # Event search and filtering
│   │   │   ├── findservice.vue     # Service lookup interface
│   │   │   ├── home.vue            # Dashboard / landing page
│   │   │   ├── login.vue           # Authentication entry point
│   │   │   ├── servicedetails.vue  # Service detail view
│   │   │   └── serviceform.vue     # Create/edit service workflow
│   ├── App.vue                     # Root Vue component
│   ├── index.css                   # Global styles (Tailwind base/custom overrides)
│   └── README.md                   # Frontend-specific documentation
├── documentation/                  # Project documentation and planning artifacts
│   ├── Functional Specification Document.pdf  # Formal functional requirements
│   └── Project_Timeline_Group_8.xlsx           # Project timeline and milestone tracking
├── 398512429-b71af6f2-089b-4e80-9f96-f426f7773ac3.png  # Architecture/UI reference image
├── package-lock.json               # Dependency lockfile (root)
├── package.json                    # Root-level scripts and shared tooling
└── README.md # Project summary         
```

## Project Setup

### Backend
```bash
cd backend
# follow backend/README for env vars and run instructions
npm install
npm run dev
```

### Frontend
```bash
cd frontend
# follow frontend/README for env vars and run instructions
npm install
npm run dev
```

Refer to the backend/README.md and frontend/README.md for environment variables, database setup, and seed scripts.
