# 🚛 Edward Moll — Frontend

> Official website for **Edward Moll Moving & Relocation Services** — built with React 19, TypeScript, Vite, and Tailwind CSS v4.

🌐 **Live Site:** [https://edwardmoll-frontend-nine.vercel.app](https://edwardmoll-frontend-nine.vercel.app)  
🔧 **Backend API:** [https://edwardmoll526.onrender.com](https://edwardmoll526.onrender.com)  
📖 **Swagger Docs:** [https://edwardmoll526.onrender.com/api](https://edwardmoll526.onrender.com/api)

---

## 📸 Tech Stack

| Technology | Version | Purpose |
|---|---|---|
| [React](https://react.dev/) | 19 | UI Framework |
| [TypeScript](https://www.typescriptlang.org/) | 6 | Type Safety |
| [Vite](https://vite.dev/) | 8 | Build Tool & Dev Server |
| [Tailwind CSS](https://tailwindcss.com/) | 4 | Styling |
| [shadcn/ui](https://ui.shadcn.com/) | latest | UI Components |
| [React Router](https://reactrouter.com/) | 7 | Client-side Routing |
| [Redux Toolkit](https://redux-toolkit.js.org/) | 2 | State Management |
| [React Hook Form](https://react-hook-form.com/) | 7 | Form Handling |
| [Zod](https://zod.dev/) | 4 | Schema Validation |
| [Framer Motion](https://www.framer.com/motion/) | 13 | Animations |
| [Recharts](https://recharts.org/) | 3 | Admin Charts |

---

## 📁 Project Structure

```
src/
├── pages/                  # Route-level pages
│   ├── Home.tsx
│   ├── About.tsx
│   ├── ServicesPage.tsx
│   ├── Gallery.tsx
│   ├── Contact.tsx
│   ├── Updates.tsx         # Blog/news page
│   ├── PostDetail.tsx
│   ├── Realtors.tsx
│   └── NotFound.tsx
├── pages/admin/            # Admin dashboard pages
│   ├── AdminLogin.tsx
│   ├── Dashboard.tsx
│   ├── ServicesManager.tsx
│   ├── GalleryManager.tsx
│   ├── PostsManager.tsx
│   └── InquiriesManager.tsx
├── components/             # Reusable UI components
│   ├── ui/                 # shadcn/ui base components
│   ├── layout/             # Navbar, Footer
│   ├── home/               # Home page sections
│   ├── about/              # About page sections
│   ├── contact/            # Contact form sections
│   └── common/             # Shared components
├── routes/
│   └── AppRoutes.tsx       # All route definitions
├── store/
│   └── authSlice.tsx       # Redux auth state
├── App.tsx
└── main.tsx
```

---

## ✨ Features

### Public Website
- 🏠 **Home** — Hero banner, services overview, reviews, crew gallery, CTA sections
- ℹ️ **About** — Company story, team, and values
- 🛠️ **Services** — Full service listings with details
- 🖼️ **Gallery** — Photo gallery of moves and crew
- 📰 **Updates/Blog** — Posts with comments, likes, and sharing
- 🤝 **Realtors** — Dedicated realtor partnership page
- 📬 **Contact** — Inquiry form with validation

### Admin Dashboard (Protected)
- 🔐 JWT-based login
- 📊 Dashboard with stats overview
- 🛠️ Manage Services (CRUD)
- 🖼️ Manage Gallery Images (CRUD)
- 📝 Manage Blog Posts (CRUD)
- 📨 View & manage Contact Inquiries

---

## 🔐 Admin Portal Access

Access the live Admin Login Portal here:

👉 **[https://edwardmoll-frontend.vercel.app/admin/login](https://edwardmoll-frontend.vercel.app/admin/login)**

### Login Credentials

| Field | Value |
|---|---|
| **Email** | `admin@gmail.com` |
| **Password** | `Admin@1234` |

> After signing in, you will have access to the **Admin Dashboard** where you can manage services, gallery images, blog posts, and contact inquiries.

---

## 🚀 Getting Started

### Prerequisites
- Node.js `>= 18`
- npm or yarn
- Backend API running (see [edwardmoll-backend](https://github.com/your-username/edwardmoll-backend))

### Installation

```bash
# Clone the repository
git clone https://github.com/your-username/edwardmoll-frontend.git
cd edwardmoll-frontend

# Install dependencies
npm install
```

### Environment Variables

Create a `.env` file in the root directory:

```env
# Backend API base URL
VITE_API_URL=http://localhost:3000
```

### Running the App

```bash
# Start development server
npm run dev

# Build for production
npm run build

# Preview production build
npm run preview

# Run linter
npm run lint
```

---

## 🌐 Deployment

This project is deployed on **Vercel**.

The `vercel.json` is already configured for client-side routing:

```json
{
  "rewrites": [{ "source": "/(.*)", "destination": "/" }]
}
```

### Deploy to Vercel

1. Push the code to GitHub
2. Go to [vercel.com](https://vercel.com) → Import your repository
3. Set the environment variable:
   - `VITE_API_URL` → your deployed backend URL
4. Click **Deploy**

---

## 🔗 Related

- 🔧 **Backend API:** [edwardmoll526.onrender.com](https://edwardmoll526.onrender.com) — NestJS + Prisma + PostgreSQL (deployed on Render)
- 📖 **Swagger Docs:** [edwardmoll526.onrender.com/api](https://edwardmoll526.onrender.com/api)

---

## 📄 License

This project is private and proprietary. All rights reserved © Edward Moll Moving & Relocation Services.
