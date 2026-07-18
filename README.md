## Arkana | Social Campaign Managment System
Access the application: [https://arkana-portfolio.vercel.app](https://arkana-portfolio.vercel.app/)
</div>

Group: [Analice Carneiro](https://github.com/AnaliceCoimbra/), [Mariah Alice Pereira](https://github.com/alicelobwp), [Sofia Hernandes](https://github.com/sofiahernandes), [Victória Azevedo](https://github.com/viick04)  
Advisors: [Cristina Leite](https://www.linkedin.com/), [David Lemes](https://www.linkedin.com/in/dolemes/), [Francisco Escobar](https://www.linkedin.com/), [Leonardo Lugoboni](https://www.linkedin.com/), [Katia Bossi](https://www.linkedin.com/)
<br/><br/>

### Description

Arkana is a TypeScript-first full-stack web application developed for the **Lideranças Empáticas Project**, an initiative by **FECAP University Center** that combines social impact with entrepreneurial education through food and fundraising campaigns.
The platform streamlines the management of every donation campaign edition by providing tools for team administration, activity tracking, goal monitoring, contribution management, receipt validation, and performance analytics.
Designed prioritizing scalability and maintainability, the application leverages **Next.js**, **Express**, **Prisma**, **MySQL**, **JWT authentication**, **Cloudinary**, and a RESTful architecture, with deployment configured for **Vercel** and **Railway**.

### Tech Stack
- Language(s): TypeScript (primary), JavaScript (secondary)
- Framework/runtime: Next.js 15 (frontend, likely App Router) + Node.js + Express (backend) + Prisma ORM with MySQL
- Notable libraries: Next.js, React, Radix UI + Recharts (frontend); Express, Prisma, mysql2, multer/cloudinary (backend)

### Folders structure

```yaml
backend/              # Express + Prisma backend (TypeScript/JavaScript sources, routes, controllers, uploads)
  ├─ package.json
  ├─ .env.example
  ├─ prisma/          # Prisma schema & generated artifacts (persistence layer)
  └─ src/
     ├─ app.js        # Express app configuration (CORS, static /uploads, error handlers)
     ├─ server.js     # Server entry
     ├─ db.js         # DB connection (mysql2 pool)
     ├─ routes.js     # All HTTP routes (contributions, mentors, teams, users, receipts)
     ├─ controllers/  # Controller implementations (business endpoints)
     └─ uploads/      # Uploads handling (multer/cloudinary)
frontend/             # Next.js TypeScript frontend (app/, components/, hooks/, styles/)
  ├─ package.json
  ├─ next.config.mjs
  └─ app/             # Next app pages/components (UI, charts, forms)
entregas/             # Delivery documents & DB SQL (arkana-database.sql referenced)
README.md
LICENSE
tailwind.config.js
postcss.config.js
```

### How to run it locally

0. Pre-requisites: [Node.js](https://nodejs.org/) and [Yarn](https://classic.yarnpkg.com/lang/en/) ou `npm`

1. Clone and enter repo

```bash
git clone https://github.com/sofiahernandes/social-campaign-manager.git
cd social-campaign-manager
```

2. Install dependencies (root then frontend/backend if needed)

```bash
npm install 
# or
yarn install
```

3. Prepare the database (SQL available in the Markdown file [DATABASE.md](https://github.com/sofiahernandes/social-campaign-manager/blob/main/DATABASE.md) — run arkana-database.sql in your MySQL) 

4. Start development servers (run in both backend and frontend directories)
```bash
npm run dev 
# or
yarn run dev
```

### License

<a href="https://www.fecap.br">FECAP - Fundação de Comércio Álvares Penteado</a> - <a href="https://github.com/sofiahernandes/social-campaign-manager">Arkana</a> © 2025 by <a href="https://github.com/analicecoimbra">Analice Coimbra Carneiro</a>, <a href="https://github.com/alicelobwp">Mariah Alice Pimentel Lôbo Pereira</a>, <a href="https://github.com/sofiahernandes">Sofia Botechia Hernandes</a> and <a href="https://github.com/viick04">Victória Duarte Vieira Azevedo</a> is licensed under <a href="https://creativecommons.org/licenses/by-sa/4.0/">CC BY-SA 4.0</a> <img src="https://mirrors.creativecommons.org/presskit/icons/cc.svg" height="20" width="20" style="margin-left: 0.2em;"><img src="https://mirrors.creativecommons.org/presskit/icons/by.svg" height="20" width="20" style="margin-left: 0.2em;"><img src="https://mirrors.creativecommons.org/presskit/icons/sa.svg" height="20" width="20" style="margin-left: 0.2em;">
