# Product Requirements Document (PRD)

# DevPortfolio CMS

## 1. Ringkasan Produk

**Nama produk:** DevPortfolio CMS  
**Jenis produk:** Fullstack personal portfolio platform dengan admin dashboard  
**Target pengguna utama:** Fachri sebagai developer/admin  
**Target pengunjung:** Recruiter, calon klien, rekan developer, hiring manager, dan publik

DevPortfolio CMS adalah aplikasi portfolio modern berbasis **Next.js**, **NestJS**, **TypeScript**, **SQLite**, **Docker**, dan **CI/CD**. Aplikasi ini tidak hanya berfungsi sebagai website portfolio, tetapi juga sebagai studi kasus pengembangan software yang menonjolkan praktik **clean code**, **maintainable architecture**, **reusable component**, **readable codebase**, dokumentasi, testing, dan deployment modern.

Produk ini terdiri dari dua bagian utama:

1. **Public Portfolio Website**  
   Website publik untuk menampilkan profil, project, skill, pengalaman, blog, sertifikat, dan kontak.

2. **Admin Dashboard / CMS**  
   Panel admin untuk mengelola seluruh konten portfolio tanpa perlu mengubah kode secara manual.

---

## 2. Tujuan Produk

### 2.1 Tujuan Utama

Membangun project portfolio fullstack yang dapat digunakan sebagai:

- Portfolio pribadi profesional.
- Studi kasus kemampuan fullstack development.
- Latihan clean code dan software architecture.
- Bukti kemampuan membangun aplikasi production-like.
- Showcase kemampuan frontend, backend, database, DevOps, deployment, dan dokumentasi.

### 2.2 Tujuan Pembelajaran

Project ini harus membantu developer melatih:

- Clean code.
- Maintainable architecture.
- Reusable components.
- Readable file structure.
- Type safety dengan TypeScript.
- Separation of concerns.
- API design yang konsisten.
- Form validation yang rapi.
- Error handling yang jelas.
- Testing frontend dan backend.
- Dokumentasi teknis.
- Docker-based development.
- CI/CD workflow.
- Deployment frontend dan backend.

---

## 3. Problem Statement

Banyak portfolio developer hanya berupa halaman statis dan tidak benar-benar menunjukkan kemampuan engineering secara menyeluruh. Portfolio seperti itu sering tidak cukup untuk membuktikan kemampuan membangun aplikasi nyata.

Project ini dibuat untuk menjawab masalah tersebut dengan membangun portfolio yang memiliki:

- Frontend modern.
- Backend API.
- Database.
- Admin dashboard.
- Authentication.
- CRUD content management.
- Deployment pipeline.
- Documentation.
- Testing.
- Clean architecture.

Dengan begitu, portfolio tidak hanya menunjukkan hasil akhir, tetapi juga menunjukkan cara developer membangun software yang rapi, scalable, dan maintainable.

---

## 4. Target Pengguna

### 4.1 Admin / Owner

Admin adalah pemilik portfolio.

Kebutuhan admin:

- Login ke dashboard.
- Mengelola profil pribadi.
- Menambah, mengubah, dan menghapus project.
- Mengelola blog atau catatan teknis.
- Mengelola skill.
- Mengelola pengalaman kerja.
- Mengelola pendidikan.
- Mengelola sertifikat.
- Membaca pesan kontak.
- Mengatur tampilan dasar website.

### 4.2 Visitor

Visitor adalah orang yang melihat portfolio publik.

Kebutuhan visitor:

- Melihat profil developer dengan cepat.
- Melihat project unggulan.
- Membaca detail project.
- Melihat tech stack.
- Melihat pengalaman dan pendidikan.
- Membaca blog/catatan developer.
- Menghubungi developer.
- Mengakses GitHub, LinkedIn, CV, atau live demo.

---

## 5. Value Proposition

DevPortfolio CMS memberikan nilai utama sebagai berikut:

- **Untuk admin:** mudah mengelola konten portfolio tanpa edit kode.
- **Untuk visitor:** mudah memahami kemampuan, pengalaman, dan kualitas project developer.
- **Untuk recruiter:** bisa melihat bukti kemampuan fullstack secara nyata.
- **Untuk developer:** menjadi latihan membangun aplikasi bersih, reusable, maintainable, dan production-ready.

---

## 6. Scope Produk

### 6.1 In Scope

Fitur yang termasuk dalam versi utama:

- Public landing page.
- About page.
- Project listing.
- Project detail page.
- Skill section.
- Experience timeline.
- Education section.
- Certificate section.
- Blog listing.
- Blog detail page.
- Contact form.
- Admin login.
- Admin dashboard.
- CRUD profile.
- CRUD projects.
- CRUD blog posts.
- CRUD skills.
- CRUD experiences.
- CRUD education.
- CRUD certificates.
- Contact inbox.
- Site settings.
- API documentation.
- Docker setup.
- CI workflow.
- Frontend deployment.
- Backend deployment.

### 6.2 Out of Scope untuk MVP

Fitur yang tidak wajib untuk versi awal:

- Multi-user admin.
- Role-based permission kompleks.
- Payment system.
- Real-time chat.
- Advanced analytics.
- Comment system di blog.
- Newsletter system.
- Multi-language support.
- AI content generator.

Fitur tersebut dapat ditambahkan setelah MVP stabil.

---

## 7. Product Goals

### 7.1 Functional Goals

- Visitor dapat melihat portfolio dengan cepat dan nyaman.
- Admin dapat mengelola seluruh konten utama dari dashboard.
- Data project, blog, skill, pengalaman, pendidikan, dan sertifikat tersimpan di database.
- Contact form dapat menyimpan pesan visitor.
- API backend terdokumentasi dengan Swagger/OpenAPI.
- Website dapat di-deploy dan diakses online.

### 7.2 Engineering Goals

- Codebase mudah dibaca.
- Struktur folder konsisten.
- Komponen frontend reusable.
- Backend modular.
- DTO dan validation digunakan secara konsisten.
- TypeScript digunakan secara ketat.
- API response konsisten.
- Error handling jelas.
- Testing tersedia untuk logic penting.
- CI berjalan otomatis saat push atau pull request.
- Docker dapat menjalankan project secara lokal.

---

## 8. Success Metrics

Produk dianggap sukses jika:

- Public website dapat menampilkan semua konten portfolio.
- Admin dapat login dan mengelola konten utama.
- CRUD project berjalan lengkap.
- CRUD blog berjalan lengkap.
- Contact form dapat menyimpan pesan.
- Frontend berhasil deploy ke Vercel.
- Backend berhasil deploy ke platform backend.
- README menjelaskan setup, fitur, arsitektur, dan deployment.
- Tidak ada TypeScript error.
- Linting lolos.
- Build frontend dan backend berhasil.
- Minimal ada unit test untuk service backend penting.
- Minimal ada reusable component library internal di frontend.

---

## 9. Tech Stack

### 9.1 Frontend

- Next.js App Router.
- React.js.
- TypeScript.
- Tailwind CSS.
- shadcn/ui.
- React Icons.
- Lucide React.
- Framer Motion.
- React Hook Form.
- Zod.
- TanStack Query.
- Axios atau native fetch wrapper.
- next-themes.
- Sonner untuk toast.

### 9.2 Backend

- NestJS.
- TypeScript.
- Prisma ORM.
- SQLite untuk development/demo.
- JWT authentication.
- bcrypt untuk password hashing.
- class-validator.
- class-transformer.
- Swagger/OpenAPI.
- Helmet.
- CORS.
- ConfigModule.

### 9.3 DevOps

- Docker.
- Docker Compose.
- GitHub Actions.
- Vercel untuk frontend.
- Railway/Render/Fly.io/VPS untuk backend.

### 9.4 Testing

- Jest untuk backend.
- Supertest untuk API testing.
- Vitest untuk frontend utility testing.
- React Testing Library untuk component testing.
- Playwright sebagai opsional untuk e2e testing.

---

## 10. Product Architecture

### 10.1 High-Level Architecture

```txt
Visitor/Admin
    |
    v
Next.js Frontend
    |
    v
NestJS REST API
    |
    v
Prisma ORM
    |
    v
SQLite Database
```

### 10.2 Public Website Flow

```txt
Visitor membuka website
Visitor melihat halaman portfolio
Frontend mengambil data dari API
API mengambil data dari database
Data ditampilkan ke UI
```

### 10.3 Admin Flow

```txt
Admin membuka /admin/login
Admin login dengan email dan password
Backend validasi credential
Backend mengembalikan JWT
Frontend menyimpan token dengan aman
Admin mengakses dashboard
Admin melakukan CRUD content
Frontend mengirim request ke API
Backend memvalidasi request
Database diperbarui
Public website menampilkan data terbaru
```

---

## 11. User Stories

### 11.1 Public Visitor

#### US-001 — View Landing Page

Sebagai visitor, saya ingin melihat halaman utama portfolio agar saya cepat memahami siapa developer ini dan apa keahliannya.

Acceptance criteria:

- Visitor dapat melihat hero section.
- Visitor dapat melihat nama, role, dan deskripsi singkat.
- Visitor dapat membuka link GitHub, LinkedIn, dan CV.
- Visitor dapat menuju halaman projects dan contact.

#### US-002 — View Projects

Sebagai visitor, saya ingin melihat daftar project agar saya dapat menilai kemampuan developer.

Acceptance criteria:

- Visitor dapat melihat daftar project.
- Visitor dapat melihat tech stack setiap project.
- Visitor dapat membuka detail project.
- Visitor dapat membuka GitHub URL jika tersedia.
- Visitor dapat membuka live demo jika tersedia.

#### US-003 — View Project Detail

Sebagai visitor, saya ingin membaca detail project agar saya memahami masalah, solusi, dan teknologi yang digunakan.

Acceptance criteria:

- Halaman detail project menampilkan title, description, content, thumbnail, tech stack, GitHub URL, live URL, dan status.
- Jika project tidak ditemukan, tampilkan halaman not found yang rapi.

#### US-004 — View Skills

Sebagai visitor, saya ingin melihat skill developer berdasarkan kategori agar mudah memahami kemampuan teknisnya.

Acceptance criteria:

- Skill dikelompokkan berdasarkan kategori.
- Skill dapat memiliki icon dan level.
- Tampilan responsive.

#### US-005 — Send Contact Message

Sebagai visitor, saya ingin mengirim pesan melalui form kontak agar dapat menghubungi developer.

Acceptance criteria:

- Form memiliki field name, email, subject, message.
- Form divalidasi di frontend dan backend.
- Pesan tersimpan di database.
- Visitor menerima success message setelah submit.
- Jika gagal, tampilkan error message yang jelas.

### 11.2 Admin User Stories

#### US-006 — Admin Login

Sebagai admin, saya ingin login agar dapat mengelola konten portfolio.

Acceptance criteria:

- Admin dapat memasukkan email dan password.
- Backend memvalidasi credential.
- Jika berhasil, admin diarahkan ke dashboard.
- Jika gagal, tampilkan error message.
- Route admin dilindungi dari visitor yang belum login.

#### US-007 — Manage Projects

Sebagai admin, saya ingin membuat, mengedit, menghapus, dan mempublish project agar portfolio selalu update.

Acceptance criteria:

- Admin dapat melihat list project.
- Admin dapat membuat project baru.
- Admin dapat mengedit project.
- Admin dapat menghapus project.
- Admin dapat mengubah status draft/published/archived.
- Admin dapat menandai project sebagai featured.

#### US-008 — Manage Blog Posts

Sebagai admin, saya ingin membuat dan mengelola blog agar dapat membagikan catatan teknis.

Acceptance criteria:

- Admin dapat melihat list blog.
- Admin dapat membuat blog post.
- Admin dapat mengedit blog post.
- Admin dapat menghapus blog post.
- Admin dapat mengatur status draft/published.
- Admin dapat menambahkan tags.

#### US-009 — Manage Profile

Sebagai admin, saya ingin mengubah data profil agar informasi publik selalu akurat.

Acceptance criteria:

- Admin dapat mengedit nama, title, bio, email, location, avatar URL, CV URL, dan social links.
- Perubahan tampil di public website.

#### US-010 — Manage Contact Messages

Sebagai admin, saya ingin melihat pesan masuk agar dapat merespons visitor.

Acceptance criteria:

- Admin dapat melihat daftar pesan.
- Admin dapat membaca detail pesan.
- Admin dapat menandai pesan sebagai read/unread.
- Admin dapat mengarsipkan pesan.
- Admin dapat menghapus pesan.

---

## 12. Functional Requirements

### 12.1 Public Website

#### FR-001 — Landing Page

Halaman utama harus menampilkan:

- Navbar.
- Hero section.
- Short intro.
- Featured projects.
- Tech stack preview.
- Experience preview.
- Latest blog posts.
- Contact CTA.
- Footer.

#### FR-002 — About Page

Halaman about harus menampilkan:

- Full bio.
- Profile image.
- Tech stack summary.
- Experience summary.
- Education summary.
- Download CV button.

#### FR-003 — Projects Page

Halaman projects harus mendukung:

- List project.
- Search project.
- Filter berdasarkan category.
- Filter berdasarkan tech stack.
- Featured badge.
- Empty state jika tidak ada data.

#### FR-004 — Project Detail Page

Halaman detail project harus menampilkan:

- Title.
- Description.
- Full content.
- Thumbnail.
- Tech stack.
- Problem statement.
- Solution.
- Features.
- GitHub link.
- Live demo link.
- Related projects opsional.

#### FR-005 — Blog Page

Halaman blog harus mendukung:

- List blog post.
- Search post.
- Filter by tag.
- Published posts only untuk visitor.

#### FR-006 — Blog Detail Page

Halaman detail blog harus menampilkan:

- Title.
- Excerpt.
- Content.
- Cover image.
- Tags.
- Published date.

#### FR-007 — Contact Page

Halaman contact harus memiliki:

- Contact form.
- Social links.
- Email address.
- Success and error state.

### 12.2 Admin Dashboard

#### FR-008 — Admin Login

Admin harus dapat login menggunakan email dan password.

#### FR-009 — Protected Admin Route

Semua route `/admin/*` selain `/admin/login` harus hanya dapat diakses oleh admin yang sudah login.

#### FR-010 — Dashboard Overview

Dashboard harus menampilkan:

- Total projects.
- Total posts.
- Total skills.
- Total experiences.
- Total messages.
- Total unread messages.
- Latest messages.
- Latest projects.

#### FR-011 — Project Management

Admin harus dapat:

- Create project.
- Read project list.
- Update project.
- Delete project.
- Publish/unpublish project.
- Set featured project.

#### FR-012 — Blog Management

Admin harus dapat:

- Create post.
- Read post list.
- Update post.
- Delete post.
- Publish/unpublish post.

#### FR-013 — Skill Management

Admin harus dapat:

- Create skill.
- Read skill list.
- Update skill.
- Delete skill.
- Reorder skill.

#### FR-014 — Experience Management

Admin harus dapat:

- Create experience.
- Read experience list.
- Update experience.
- Delete experience.
- Set current position.

#### FR-015 — Education Management

Admin harus dapat:

- Create education record.
- Read education list.
- Update education record.
- Delete education record.

#### FR-016 — Certificate Management

Admin harus dapat:

- Create certificate.
- Read certificate list.
- Update certificate.
- Delete certificate.

#### FR-017 — Contact Inbox

Admin harus dapat:

- Read contact messages.
- Mark as read.
- Mark as unread.
- Archive message.
- Delete message.

#### FR-018 — Site Settings

Admin harus dapat mengatur:

- Site name.
- Site description.
- Hero title.
- Hero subtitle.
- Logo text.
- Primary color.
- Toggle blog section.
- Toggle contact section.
- Toggle resume section.

---

## 13. Non-Functional Requirements

### 13.1 Performance

- Landing page initial load harus cepat.
- Images harus dioptimasi.
- API response untuk list data sederhana harus cepat.
- Frontend harus menggunakan caching strategy untuk data yang jarang berubah.
- Hindari unnecessary re-render.

### 13.2 Security

- Password harus di-hash menggunakan bcrypt.
- JWT secret disimpan di environment variable.
- Endpoint admin harus dilindungi guard.
- Validasi input dilakukan di frontend dan backend.
- CORS hanya mengizinkan origin yang diperlukan.
- Gunakan Helmet di backend.
- Jangan expose sensitive env ke frontend.
- Error message tidak boleh membocorkan detail internal.

### 13.3 Maintainability

- Struktur folder harus konsisten.
- Naming harus jelas.
- Business logic tidak dicampur dengan UI.
- API service dipisahkan dari component.
- Validation schema dipisahkan dari component.
- Reusable component dipakai untuk UI yang berulang.
- Hindari duplicated code.
- Setiap module backend punya controller, service, DTO, entity/model mapping jika diperlukan.

### 13.4 Readability

- Gunakan nama variable dan function yang deskriptif.
- Hindari function terlalu panjang.
- Hindari nested conditional berlebihan.
- Gunakan early return jika lebih mudah dibaca.
- Gunakan type/interface yang jelas.
- Tambahkan comment hanya untuk logic yang memang butuh penjelasan.

### 13.5 Reusability

- Button, Input, Card, SectionHeader, PageHeader, EmptyState, LoadingState dibuat reusable.
- Admin table dibuat reusable.
- Form field dibuat reusable.
- API client dibuat reusable.
- Custom hook dibuat untuk data fetching yang sering dipakai.

### 13.6 Reliability

- Form harus menangani loading, success, dan error state.
- API harus memberikan response konsisten.
- Delete action harus menggunakan confirmation dialog.
- Jika data kosong, tampilkan empty state.
- Jika API error, tampilkan feedback yang jelas.

### 13.7 Accessibility

- Gunakan semantic HTML.
- Button harus punya label jelas.
- Form input harus punya label.
- Kontras warna harus cukup.
- Navigasi keyboard harus diperhatikan.
- Modal/dialog harus accessible.

### 13.8 Responsiveness

- Website harus nyaman di desktop, tablet, dan mobile.
- Admin dashboard minimal usable di tablet dan desktop.
- Public website wajib mobile-friendly.

---

## 14. Clean Code Requirements

### 14.1 General Rules

- Satu file sebaiknya punya satu tanggung jawab utama.
- Function harus kecil dan fokus.
- Hindari magic string; gunakan constant atau enum.
- Hindari duplicated logic.
- Hindari component yang terlalu besar.
- Gunakan composition daripada props yang terlalu banyak.
- Gunakan strict TypeScript.
- Gunakan formatter dan linter.

### 14.2 Frontend Clean Code Rules

- Component UI tidak boleh langsung berisi business logic kompleks.
- Data fetching diletakkan di service atau hook.
- Form schema diletakkan di file terpisah.
- Type diletakkan di folder `types` atau dekat feature terkait.
- Gunakan feature-based folder structure.
- Gunakan reusable layout component.
- Hindari inline object/function yang tidak perlu jika menyebabkan re-render.

### 14.3 Backend Clean Code Rules

- Controller hanya menangani request dan response flow.
- Service menangani business logic.
- DTO menangani validasi input.
- Prisma query dikelola di service atau repository layer.
- Guard digunakan untuk authentication.
- Interceptor/filter digunakan untuk response/error handling jika diperlukan.
- Module harus dipisahkan berdasarkan domain.

### 14.4 Naming Convention

Frontend:

```txt
components/ui/button.tsx
components/common/page-header.tsx
features/projects/components/project-card.tsx
features/projects/services/project.service.ts
features/projects/types/project.type.ts
features/projects/schemas/project.schema.ts
```

Backend:

```txt
projects.controller.ts
projects.service.ts
projects.module.ts
dto/create-project.dto.ts
dto/update-project.dto.ts
```

---

## 15. Frontend Architecture

### 15.1 Recommended Folder Structure

```txt
apps/web/
├── app/
│   ├── (public)/
│   │   ├── page.tsx
│   │   ├── about/
│   │   ├── projects/
│   │   ├── blog/
│   │   └── contact/
│   ├── admin/
│   │   ├── login/
│   │   ├── page.tsx
│   │   ├── projects/
│   │   ├── posts/
│   │   ├── skills/
│   │   ├── experiences/
│   │   ├── education/
│   │   ├── certificates/
│   │   ├── messages/
│   │   └── settings/
│   ├── layout.tsx
│   └── globals.css
│
├── components/
│   ├── ui/
│   ├── common/
│   ├── layout/
│   └── admin/
│
├── features/
│   ├── auth/
│   ├── profile/
│   ├── projects/
│   ├── posts/
│   ├── skills/
│   ├── experiences/
│   ├── education/
│   ├── certificates/
│   ├── messages/
│   └── settings/
│
├── hooks/
├── lib/
├── services/
├── types/
└── constants/
```

### 15.2 Component Layers

#### UI Components

Komponen dasar yang tidak tahu business logic.

Contoh:

- Button.
- Input.
- Textarea.
- Select.
- Badge.
- Card.
- Dialog.

#### Common Components

Komponen umum yang reusable lintas halaman.

Contoh:

- PageHeader.
- SectionHeader.
- EmptyState.
- LoadingState.
- ErrorState.
- ConfirmDialog.

#### Feature Components

Komponen yang spesifik ke domain.

Contoh:

- ProjectCard.
- ProjectForm.
- PostForm.
- SkillForm.
- MessageDetail.

#### Layout Components

Komponen struktur halaman.

Contoh:

- PublicNavbar.
- PublicFooter.
- AdminSidebar.
- AdminTopbar.
- AdminShell.

---

## 16. Backend Architecture

### 16.1 Recommended Folder Structure

```txt
apps/api/src/
├── auth/
│   ├── auth.controller.ts
│   ├── auth.service.ts
│   ├── auth.module.ts
│   ├── guards/
│   ├── strategies/
│   └── dto/
│
├── users/
├── profile/
├── projects/
├── posts/
├── skills/
├── experiences/
├── education/
├── certificates/
├── messages/
├── settings/
│
├── common/
│   ├── decorators/
│   ├── filters/
│   ├── guards/
│   ├── interceptors/
│   ├── pipes/
│   ├── types/
│   └── utils/
│
├── prisma/
│   ├── prisma.module.ts
│   └── prisma.service.ts
│
├── config/
├── app.module.ts
└── main.ts
```

### 16.2 Backend Module Pattern

Setiap domain module minimal memiliki:

```txt
module-name/
├── dto/
│   ├── create-module.dto.ts
│   └── update-module.dto.ts
├── module-name.controller.ts
├── module-name.service.ts
└── module-name.module.ts
```

### 16.3 API Response Standard

Gunakan response format konsisten:

```json
{
  "success": true,
  "message": "Project created successfully",
  "data": {}
}
```

Untuk error:

```json
{
  "success": false,
  "message": "Validation failed",
  "errors": []
}
```

---

## 17. Database Design

### 17.1 User

```prisma
model User {
  id        String   @id @default(cuid())
  name      String
  email     String   @unique
  password  String
  role      String   @default("admin")
  createdAt DateTime @default(now())
  updatedAt DateTime @updatedAt
}
```

### 17.2 Profile

```prisma
model Profile {
  id           String   @id @default(cuid())
  name         String
  username     String?
  title        String
  shortBio     String
  longBio      String?
  email        String
  phone        String?
  location     String?
  avatarUrl    String?
  cvUrl        String?
  githubUrl    String?
  linkedinUrl  String?
  instagramUrl String?
  websiteUrl   String?
  createdAt    DateTime @default(now())
  updatedAt    DateTime @updatedAt
}
```

### 17.3 Project

```prisma
model Project {
  id               String   @id @default(cuid())
  title            String
  slug             String   @unique
  description      String
  content          String?
  thumbnail        String?
  category         String
  techStack        String
  githubUrl        String?
  liveUrl          String?
  documentationUrl String?
  status           String   @default("draft")
  featured         Boolean  @default(false)
  createdAt        DateTime @default(now())
  updatedAt        DateTime @updatedAt
}
```

### 17.4 BlogPost

```prisma
model BlogPost {
  id         String   @id @default(cuid())
  title      String
  slug       String   @unique
  excerpt    String?
  content    String
  coverImage String?
  tags       String?
  status     String   @default("draft")
  createdAt  DateTime @default(now())
  updatedAt  DateTime @updatedAt
}
```

### 17.5 Skill

```prisma
model Skill {
  id        String   @id @default(cuid())
  name      String
  category  String
  icon      String?
  level     Int?
  order     Int      @default(0)
  createdAt DateTime @default(now())
  updatedAt DateTime @updatedAt
}
```

### 17.6 Experience

```prisma
model Experience {
  id          String   @id @default(cuid())
  company     String
  position    String
  location    String?
  startDate   DateTime
  endDate     DateTime?
  isCurrent   Boolean  @default(false)
  description String
  techStack   String?
  createdAt   DateTime @default(now())
  updatedAt   DateTime @updatedAt
}
```

### 17.7 Education

```prisma
model Education {
  id          String   @id @default(cuid())
  school      String
  major       String
  degree      String?
  startYear   String
  endYear     String?
  description String?
  createdAt   DateTime @default(now())
  updatedAt   DateTime @updatedAt
}
```

### 17.8 Certificate

```prisma
model Certificate {
  id            String   @id @default(cuid())
  title         String
  issuer        String
  issueDate     DateTime
  credentialUrl String?
  imageUrl      String?
  createdAt     DateTime @default(now())
  updatedAt     DateTime @updatedAt
}
```

### 17.9 ContactMessage

```prisma
model ContactMessage {
  id        String   @id @default(cuid())
  name      String
  email     String
  subject   String
  message   String
  status    String   @default("unread")
  createdAt DateTime @default(now())
  updatedAt DateTime @updatedAt
}
```

### 17.10 SiteSetting

```prisma
model SiteSetting {
  id              String   @id @default(cuid())
  siteName        String
  siteDescription String?
  heroTitle       String?
  heroSubtitle    String?
  logoText        String?
  primaryColor    String?
  enableBlog      Boolean  @default(true)
  enableContact   Boolean  @default(true)
  enableResume    Boolean  @default(true)
  createdAt       DateTime @default(now())
  updatedAt       DateTime @updatedAt
}
```

---

## 18. API Requirements

### 18.1 Auth API

```txt
POST /auth/login
GET  /auth/me
POST /auth/logout
```

### 18.2 Profile API

```txt
GET   /profile
PATCH /profile
```

### 18.3 Projects API

```txt
GET    /projects
GET    /projects/featured
GET    /projects/:slug
POST   /projects
PATCH  /projects/:id
DELETE /projects/:id
```

Public access:

- GET `/projects`
- GET `/projects/featured`
- GET `/projects/:slug`

Admin access:

- POST `/projects`
- PATCH `/projects/:id`
- DELETE `/projects/:id`

### 18.4 Posts API

```txt
GET    /posts
GET    /posts/:slug
POST   /posts
PATCH  /posts/:id
DELETE /posts/:id
```

### 18.5 Skills API

```txt
GET    /skills
POST   /skills
PATCH  /skills/:id
DELETE /skills/:id
```

### 18.6 Experiences API

```txt
GET    /experiences
POST   /experiences
PATCH  /experiences/:id
DELETE /experiences/:id
```

### 18.7 Education API

```txt
GET    /education
POST   /education
PATCH  /education/:id
DELETE /education/:id
```

### 18.8 Certificates API

```txt
GET    /certificates
POST   /certificates
PATCH  /certificates/:id
DELETE /certificates/:id
```

### 18.9 Contact Messages API

```txt
POST   /contact/messages
GET    /contact/messages
GET    /contact/messages/:id
PATCH  /contact/messages/:id/status
DELETE /contact/messages/:id
```

### 18.10 Settings API

```txt
GET   /settings
PATCH /settings
```

---

## 19. UI/UX Requirements

### 19.1 Visual Direction

Style utama:

- Modern tech.
- Dark mode first.
- Clean SaaS look.
- Bento grid.
- Soft glow.
- Monospace accent.
- Minimal but expressive.
- Developer dashboard feel.

### 19.2 Public Website Layout

Homepage sections:

```txt
Navbar
Hero
Featured Projects
Tech Stack
Experience Timeline
Latest Blog Posts
Contact CTA
Footer
```

### 19.3 Admin Dashboard Layout

Admin layout:

```txt
Sidebar
Topbar
Page Header
Stats Cards
Data Table
Form Dialog / Form Page
Toast Notification
Confirm Delete Dialog
```

### 19.4 Required UI States

Setiap page dan form harus menangani:

- Loading state.
- Empty state.
- Error state.
- Success state.
- Disabled state.
- Validation state.

---

## 20. Admin Dashboard Requirements

### 20.1 Sidebar Menu

Sidebar admin harus memiliki menu:

```txt
Dashboard
Profile
Projects
Blog
Skills
Experience
Education
Certificates
Messages
Settings
Logout
```

### 20.2 Data Table Pattern

Setiap halaman list admin harus memiliki:

- Table.
- Search.
- Filter jika relevan.
- Pagination jika data banyak.
- Action menu.
- Edit action.
- Delete action.
- Empty state.

### 20.3 Form Pattern

Setiap form admin harus memiliki:

- Label yang jelas.
- Validation message.
- Submit button.
- Cancel button.
- Loading state saat submit.
- Toast success/error.

---

## 21. Authentication Requirements

### 21.1 Login

Input:

- Email.
- Password.

Validation:

- Email harus valid.
- Password wajib diisi.

Response success:

- Access token.
- User data.

Response failed:

- Error message umum seperti `Invalid email or password`.

### 21.2 Token Handling

- Token digunakan untuk request admin API.
- Token tidak boleh disimpan sembarangan jika ada risiko XSS.
- Untuk MVP, token dapat disimpan di httpOnly cookie jika memungkinkan.
- Alternatif sementara: memory/localStorage dengan mitigasi dan catatan teknis di README.

### 21.3 Route Protection

- Admin route dicek sebelum render halaman admin.
- Jika belum login, redirect ke `/admin/login`.
- Jika token invalid, logout otomatis.

---

## 22. Validation Requirements

Validation harus ada di dua sisi:

1. Frontend menggunakan Zod.
2. Backend menggunakan class-validator.

Contoh rule project:

- Title wajib diisi.
- Slug wajib diisi dan unique.
- Description wajib diisi.
- Category wajib diisi.
- Status hanya boleh draft, published, archived.
- URL harus valid jika diisi.

Contoh rule contact:

- Name wajib diisi minimal 2 karakter.
- Email wajib valid.
- Subject wajib diisi.
- Message minimal 10 karakter.

---

## 23. Error Handling Requirements

Frontend harus menangani:

- Network error.
- Validation error.
- Unauthorized error.
- Not found error.
- Server error.

Backend harus menangani:

- Validation exception.
- Unauthorized exception.
- Forbidden exception.
- Not found exception.
- Conflict exception untuk duplicate slug/email.
- Internal server error.

Error response harus konsisten.

---

## 24. Testing Requirements

### 24.1 Backend Testing

Minimal test:

- Auth service login success.
- Auth service login failed.
- Project service create project.
- Project service update project.
- Project service delete project.
- Contact message service create message.

### 24.2 Frontend Testing

Minimal test:

- ProjectCard render correctly.
- Contact form validation.
- Login form validation.
- EmptyState render.
- Utility function test.

### 24.3 E2E Testing Optional

Skenario e2e:

- Visitor membuka homepage.
- Visitor mengirim contact message.
- Admin login.
- Admin membuat project.
- Project muncul di public website.

---

## 25. CI/CD Requirements

GitHub Actions harus menjalankan:

- Install dependencies.
- Lint frontend.
- Build frontend.
- Lint backend.
- Generate Prisma client.
- Test backend.
- Build backend.

Contoh workflow job:

```txt
web-ci
api-ci
```

Build harus gagal jika:

- Ada TypeScript error.
- Lint error.
- Test gagal.
- Build gagal.

---

## 26. Docker Requirements

Docker Compose harus dapat menjalankan:

- Frontend app.
- Backend app.
- SQLite volume/file persistence untuk development.

Command yang diharapkan:

```bash
docker compose up --build
```

Service:

```txt
web
api
```

---

## 27. Environment Variables

### 27.1 Frontend

```env
NEXT_PUBLIC_API_URL=http://localhost:3001
```

### 27.2 Backend

```env
PORT=3001
DATABASE_URL="file:./dev.db"
JWT_SECRET="your-secret"
JWT_EXPIRES_IN="1d"
FRONTEND_URL="http://localhost:3000"
```

---

## 28. Deployment Requirements

### 28.1 Frontend Deployment

Frontend deploy ke Vercel.

Requirement:

- Root directory: `apps/web`.
- Environment variable `NEXT_PUBLIC_API_URL` diisi dengan URL backend production.
- Build berhasil tanpa error.

### 28.2 Backend Deployment

Backend deploy ke Railway, Render, Fly.io, atau VPS.

Requirement:

- Environment variable production tersedia.
- Prisma generate berjalan.
- Database tersedia.
- API dapat diakses frontend.
- CORS mengizinkan domain frontend.

### 28.3 Database Deployment Note

SQLite cocok untuk development dan demo sederhana. Untuk production yang lebih stabil, siapkan opsi migrasi ke PostgreSQL.

---

## 29. Documentation Requirements

README harus memiliki:

- Project overview.
- Features.
- Tech stack.
- Architecture diagram.
- Folder structure.
- Database schema summary.
- API documentation link.
- Installation guide.
- Environment variables.
- Docker guide.
- Testing guide.
- Deployment guide.
- Screenshots.
- Commit convention.

Dokumentasi tambahan:

```txt
docs/
├── architecture.md
├── api.md
├── database.md
├── deployment.md
├── clean-code-guidelines.md
└── contribution.md
```

---

## 30. Coding Standards

### 30.1 TypeScript

- Enable strict mode.
- Avoid `any` unless benar-benar diperlukan.
- Gunakan explicit type untuk public function.
- Gunakan union type untuk status.
- Gunakan interface/type untuk API response.

### 30.2 Formatting

- Gunakan Prettier.
- Gunakan ESLint.
- Format otomatis sebelum commit.

### 30.3 Commit Convention

Gunakan Conventional Commits.

Contoh:

```txt
feat: add project management dashboard
fix: handle invalid login credentials
refactor: simplify project form validation
chore: add docker compose setup
docs: update deployment guide
test: add project service unit tests
```

---

## 31. Reusable Component Requirements

Minimal reusable components:

```txt
PageHeader
SectionHeader
Container
EmptyState
LoadingState
ErrorState
ConfirmDialog
DataTable
StatusBadge
TechStackBadge
FormInput
FormTextarea
FormSelect
FormSwitch
SubmitButton
ProjectCard
PostCard
ExperienceTimeline
```

Setiap reusable component harus:

- Punya props yang jelas.
- Tidak terlalu spesifik kecuali memang feature component.
- Tidak menyimpan logic yang tidak relevan.
- Mudah dipakai ulang di halaman lain.

---

## 32. Feature Breakdown by Phase

### 32.1 Phase 1 — Project Foundation

Deliverables:

- Monorepo setup.
- Next.js setup.
- NestJS setup.
- TypeScript strict setup.
- Tailwind setup.
- shadcn/ui setup.
- Prisma setup.
- SQLite setup.
- Basic README.

Acceptance criteria:

- Frontend bisa run lokal.
- Backend bisa run lokal.
- Database bisa migrate.
- Lint dan build berjalan.

### 32.2 Phase 2 — Public Website MVP

Deliverables:

- Landing page.
- About page.
- Projects page.
- Project detail page.
- Contact page.
- Responsive layout.
- Dark mode.

Acceptance criteria:

- Visitor dapat membuka semua halaman utama.
- UI responsive.
- Data dapat berasal dari seed/database.

### 32.3 Phase 3 — Backend API MVP

Deliverables:

- Profile API.
- Projects API.
- Skills API.
- Experiences API.
- Contact API.
- Swagger docs.

Acceptance criteria:

- API CRUD berjalan.
- DTO validation aktif.
- Swagger dapat dibuka.
- Response konsisten.

### 32.4 Phase 4 — Admin Dashboard MVP

Deliverables:

- Admin login.
- Protected route.
- Admin layout.
- Dashboard overview.
- CRUD projects.
- Contact inbox.

Acceptance criteria:

- Admin dapat login.
- Admin dapat membuat/edit/hapus project.
- Admin dapat membaca contact message.
- Unauthorized user tidak bisa masuk dashboard.

### 32.5 Phase 5 — Content CMS Expansion

Deliverables:

- CRUD blog.
- CRUD skills.
- CRUD experiences.
- CRUD education.
- CRUD certificates.
- Site settings.
- Profile settings.

Acceptance criteria:

- Semua konten utama dapat dikelola dari admin.
- Perubahan tampil di public website.

### 32.6 Phase 6 — DevOps and Quality

Deliverables:

- Dockerfile web.
- Dockerfile api.
- Docker Compose.
- GitHub Actions CI.
- Unit tests.
- Deployment frontend.
- Deployment backend.
- Documentation update.

Acceptance criteria:

- `docker compose up --build` berhasil.
- CI berjalan saat push/PR.
- Frontend online.
- Backend online.
- README lengkap.

---

## 33. MVP Definition

MVP dianggap selesai jika memiliki:

- Public homepage.
- Projects page.
- Project detail page.
- Contact page.
- Admin login.
- Admin dashboard.
- CRUD projects.
- Contact inbox.
- NestJS API.
- SQLite database.
- Prisma ORM.
- Docker Compose.
- CI build check.
- Deployment frontend.
- Deployment backend.
- README lengkap.

---

## 34. Future Enhancements

Fitur lanjutan:

- Multi-language support.
- Advanced analytics.
- Page view tracking.
- Media upload dengan Cloudinary/Supabase Storage.
- Blog markdown editor yang lebih lengkap.
- Newsletter subscription.
- Public changelog.
- Command palette.
- Terminal-style intro.
- Project case study template.
- GitHub API integration untuk mengambil repo otomatis.
- AI-assisted blog draft.
- Role-based access control.
- PostgreSQL migration.

---

## 35. Risks and Mitigations

### 35.1 Scope Terlalu Besar

Risk:

- Project terlalu banyak fitur dan tidak selesai.

Mitigation:

- Kerjakan per phase.
- Prioritaskan MVP.
- Jangan mulai fitur advanced sebelum CRUD utama selesai.

### 35.2 Codebase Berantakan

Risk:

- Terlalu cepat menambah fitur tanpa struktur.

Mitigation:

- Gunakan folder structure sejak awal.
- Pisahkan feature, component, service, schema, dan type.
- Refactor setiap selesai satu phase.

### 35.3 SQLite Tidak Cocok untuk Production

Risk:

- SQLite kurang ideal untuk production serverless atau multi-instance.

Mitigation:

- Gunakan SQLite untuk development/demo.
- Siapkan dokumentasi migrasi ke PostgreSQL.

### 35.4 Admin Auth Kurang Aman

Risk:

- Token handling tidak aman.

Mitigation:

- Gunakan httpOnly cookie jika memungkinkan.
- Validasi route backend dengan guard.
- Jangan expose secret.

---

## 36. Definition of Done

Sebuah fitur dianggap selesai jika:

- Requirement terpenuhi.
- UI responsive.
- Loading, error, empty, dan success state tersedia.
- Form validation tersedia jika fitur memakai form.
- API validation tersedia.
- Tidak ada TypeScript error.
- Tidak ada lint error.
- Minimal ada test untuk logic penting.
- Dokumentasi singkat tersedia jika diperlukan.
- Code sudah readable dan tidak duplicate.

---

## 37. Development Principles

Project ini harus selalu mengikuti prinsip:

```txt
Clean over clever.
Readable over short.
Reusable but not over-engineered.
Consistent over personal style.
Simple first, scalable later.
```

Artinya:

- Jangan membuat abstraction terlalu cepat.
- Jangan membuat component reusable sebelum ada pola yang jelas.
- Refactor saat duplication mulai terlihat.
- Gunakan nama yang jelas meskipun lebih panjang.
- Pisahkan logic berdasarkan domain.
- Prioritaskan code yang mudah dibaca oleh developer lain.

---

## 38. Final Product Positioning

Project ini dapat diposisikan sebagai:

> A modern fullstack portfolio CMS built with Next.js, NestJS, TypeScript, SQLite, Prisma, Docker, and CI/CD, focused on clean code, maintainable architecture, reusable components, and production-like development workflow.

GitHub description:

```txt
A fullstack developer portfolio CMS with admin dashboard, built using Next.js, NestJS, TypeScript, SQLite, Prisma, Docker, and GitHub Actions.
```

Recommended repository name:

```txt
dev-portfolio-cms
```

---

## 39. Recommended First Milestone

Milestone pertama yang paling realistis:

```txt
Milestone 1: Foundation and Public Portfolio MVP
```

Tasks:

- Initialize monorepo.
- Setup Next.js.
- Setup NestJS.
- Setup Prisma + SQLite.
- Setup Tailwind + shadcn/ui.
- Create public layout.
- Create homepage.
- Create projects page.
- Create projects API.
- Seed initial project data.
- Connect frontend to API.
- Write README setup guide.

Goal milestone:

- Portfolio public sudah bisa menampilkan data project dari backend.

---

## 40. Summary

DevPortfolio CMS adalah project portfolio fullstack yang dirancang untuk menjadi bukti kemampuan teknis sekaligus latihan engineering discipline. Fokus utamanya bukan hanya membuat tampilan menarik, tetapi membangun aplikasi yang rapi, maintainable, reusable, readable, terdokumentasi, dapat diuji, dan dapat di-deploy.

Dengan PRD ini, pengembangan dapat dilakukan secara bertahap, jelas, dan terukur.
