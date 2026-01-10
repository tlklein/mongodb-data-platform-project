
# Enterprise Data Platform Project

![Screenshot 2024-12-24 at 10 24 06 PM](398512429-b71af6f2-089b-4e80-9f96-f426f7773ac3.png)

## Project Overview

A full-stack data platform (MEVN) that models how Community Health Workers (CHWs) manage events, client data, and service sign-ups. This iteration refactors a prototype into a maintainable, production-minded application with role-based access, dynamic service management, and interactive visualizations.

### Problem

Prototype code lacked maintainability, feature extensibility, and production-ready data flows. The app needed secure user access, dynamic service management, and dashboard analytics to be useful for real-world CHW workflows.

### Solution

Refactored the frontend to **Vue Composition API**, implemented secure authentication and role-based access, converted hardcoded services into CRUD-backed endpoints, and added dashboard visualizations that surface actionable metrics.

### Tech Stack

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


### Result / Key Achievements

- Implemented secure login with role-based UI (Viewer / Editor).  
- Replaced static service data with full CRUD API and real-time updates.  
- Added dashboard visualizations that expose client distribution and event metrics.  
- Improved code maintainability and developer ergonomics via Composition API refactor.

## Scope & Features (high-level)

- Auth & Access: Hashed password storage, session handling, and role-based UI control.  
- Service Management: CRUD endpoints for event services, dynamic front-end forms.  
- Dashboard: Chart components (Pie/Doughnut) showing client distribution by zip code and other KPIs.  
- Maintainability: Composition API refactor, modular components, and clearer API contracts.

## Deliverables

Functional
- Secure authentication & authorization  
- CRUD service management APIs  
- Interactive dashboard visualizations

UI
- User-friendly login & navigation  
- Service management pages and responsive chart components

Documentation
- Use case and user-flow diagrams  
- Development timeline and milestone notes  
- Backend & frontend README with run instructions

All deliverables can be found in the 'Documentation' Folder. All deliverables are completed in the 'Functional Specification Document', with a project timeline in the same folder. 

## Team

- Joanna Macedo - Contributor  
- Trinity Klein - Contributor  
- Maria Abejide - Contributor  

(Previous contributors: Jeremy Griffith, Edwin Charly, Elliot Farmer Garcia, Agatha Molski, Chris Blanco)

## Project Setup

### Backend (Node/Express)
```bash
cd backend
# follow backend/README for env vars and run instructions
npm install
npm run dev
```

### Frontend (Vue 3)
```bash
cd frontend
# follow frontend/README for env vars and run instructions
npm install
npm run dev
```

Refer to the backend/README.md and frontend/README.md for environment variables, database setup, and seed scripts.
