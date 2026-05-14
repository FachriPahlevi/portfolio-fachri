# dev-portfolio-cms

Fullstack portfolio CMS untuk latihan clean code, maintainable code, reusable component, dan readable project structure.

## Tech Stack

- Frontend: Next.js App Router, React, TypeScript, Tailwind CSS, shadcn/ui, React Icons
- Backend: NestJS, TypeScript
- Database: SQLite dengan Prisma
- DevOps: Docker dan Docker Compose
- Deployment target: frontend ke Vercel, backend ke Railway/Render/VPS

## Port

- Frontend: `http://localhost:3000`
- Backend: `http://localhost:3001`
- Prisma Studio: `http://localhost:5555`

## Struktur Project

```text
dev-portfolio-cms/
├── frontend/
├── backend/
├── docker/
├── docs/
├── docker-compose.yml
├── README.md
└── .gitignore
```

## Run Frontend Manual

```bash
cd frontend
npm install
npm run dev
```

Frontend berjalan di `http://localhost:3000`.

## Run Backend Manual

```bash
cd backend
npm install
cp .env.example .env
npm run prisma:generate
npm run prisma:migrate
npm run start:dev
```

Backend berjalan di `http://localhost:3001`.

Gunakan environment berikut saat development lokal:

```env
FRONTEND_URL=http://localhost:3000
DATABASE_URL=file:./dev.db
JWT_SECRET=dev-secret
JWT_EXPIRES_IN=1d
```

## Run dengan Docker

```bash
docker compose up --build
```

Service yang tersedia:

- Frontend: `http://localhost:3000`
- Backend: `http://localhost:3001`

Untuk menjalankan migration di container backend:

```bash
docker compose exec backend npm run prisma:migrate
```

Untuk membuka Prisma Studio:

```bash
cd backend
npm run prisma:studio
```

## GitHub Actions

CI berjalan saat `push` ke `main` dan saat `pull_request` ke `main`.

Workflow mengecek:

- Frontend: `npm ci`, `npm run lint`, `npm run build`
- Backend: `npm ci`, Prisma validate/generate, `npm run lint:check`, `npm run test`, `npm run build`
- Docker: `docker compose config`
