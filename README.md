# Assessment
Backend,Frontend,Shared-ORM
# Full Stack Assessment Project

This project is a **Full Stack Application** using:
- **Backend:** NestJS + Sequelize + MySQL
- **Frontend:** React.js
- **Shared ORM Library:** Sequelize models for database management

---
for running the project 1. cd shared-orm -> npm run build
2. cd backend -> npm run start:dev
3. cd frontend -> npm start


## 📁 Project Structure

# Shared ORM Library
This library provides shared entities, migrations, and database connection logic for the MyStore application.

## Setup
1. Install dependencies: `npm install`
2. Configure database credentials in `src/database/database-connection.ts`.
3. Run migrations: `npm run migrate`

## Prerequisites
- MySQL installed and running
- Node.js v18+
  
shared-orm/
├── src/
│   ├── models/
│   │   ├── product.js
│   │   └── category.js
│   ├── migrations/
│   │   └── 20250302123456-create-tables.js
│   └── database/
│       └── database-connection.js
├── package.json
└── README.md

# Backend
REST API for MyStore using NestJS and Sequelize.

## Setup
1. Install dependencies: `npm install`
2. Ensure the shared-orm library is built and linked.
3. Start the server: `npm run start:dev`

## Endpoint
- GET /products: Returns a JSON array of products with category details.

backend/
├── src/
│   ├── products/
│   │   ├── products.module.ts
│   │   ├── products.service.ts
│   │   └── products.controller.ts
│   ├── app.module.ts
│   └── main.ts
├── package.json
└── README.md

# Frontend
React app to display products from the MyStore API.

## Setup
1. Install dependencies: `npm install`
2. Start the app: `npm start`
3. Ensure the backend is running at http://localhost:3000.

frontend/
├── src/
│   ├── components/
│   │   └── ProductList.js
│   ├── App.js
│   └── index.js
├── package.json
└── README.md



