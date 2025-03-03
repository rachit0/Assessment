# Assessment
Backend,Frontend,Shared-ORM
# Full Stack Assessment Project

This project is a **Full Stack Application** using:
- **Backend:** NestJS + Sequelize + MySQL
- **Frontend:** React.js
- **Shared ORM Library:** Sequelize models for database management

---
Follow these steps to set up and run the project.

###  1. Clone the Repository
```sh
git clone https://github.com/rachit0/Assessment.git
cd Assessment
```  for running the project 1. cd shared-orm -> npm run build
  2. cd backend -> npm run start:dev
  3. cd frontend -> npm start
```


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

![Screenshot (27)](https://github.com/user-attachments/assets/3f1020bd-3875-445c-a67e-f460d08a40d3)


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

![Screenshot (26)](https://github.com/user-attachments/assets/ba8becb2-c71f-4da4-9d8e-9d0be2d027fe)


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

![Screenshot (25)](https://github.com/user-attachments/assets/ef368b18-0440-4c69-a76c-55ab0d930174)




