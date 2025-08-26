# Polling App

A modern **Polling Application** built with **Next.js 14, Supabase, and shadcn/ui**, designed to explore how **AI-assisted development** can accelerate feature implementation.  

This project demonstrates a complete **authentication flow** (login, registration, session management) as the foundation of a larger polling platform.  

---

## Purpose

The Polling App is being developed as part of the **ALX AI Software Engineering program** to showcase:  

- How **AI tools** (like ChatGPT) can assist in structuring, coding, and documenting projects.  
- How to integrate **Supabase authentication** into a Next.js app.  
- How to build **clean UI components** using **shadcn/ui**.  
- How to follow **best practices** in commits, folder structure, and project documentation.  

---

## Features

- **Authentication Flow** (Login & Register with Supabase).  
- **Clean UI with shadcn/ui** (reusable Button, Input, Label, Card).  
- **Next.js 14 App Router** for modern React-based routing.  
- **Supabase Auth Context** to manage user sessions globally.  
- **AI-Assisted Development**: Used for folder scaffolding, UI code generation, Supabase config, and commit message drafting.  

---

## Tech Stack

- **Framework**: Next.js 14 (with TypeScript, App Router)  
- **Authentication & Database**: Supabase  
- **UI Components**: shadcn/ui + Tailwind CSS  
- **AI Assistance**: ChatGPT (used for code scaffolding, component generation, and commit automation)  

---

## Setup & Installation

Follow these steps to run the project locally:  

### Clone the repository

```bash
git clone https://github.com/your-username/polling-app.git
cd polling-app

---

- Install dependencies

```bash
npm install

- Configure Supabase

Create a project on Supabase

Get your Project URL and Anon Key from Project Settings > API.

Create a .env.local file in the root of the project and add:

```env
NEXT_PUBLIC_SUPABASE_URL=your-project-url
NEXT_PUBLIC_SUPABASE_ANON_KEY=your-anon-key

- Run the project

```bash
npm run dev


Visit: http://localhost:3000

## Project Structure

```bash
src/
  lib/
    supabaseClient.ts     # Supabase client setup
    auth-context.tsx      # Authentication context provider
  components/
    ui/                   # shadcn/ui components
      button.tsx
      input.tsx
      label.tsx
      card.tsx
    LoginForm.tsx         # Login form
    RegisterForm.tsx      # Registration form
  app/
    auth/
      login/page.tsx      # Login page
      register/page.tsx   # Register page
    layout.tsx            # Root layout with AuthProvider

## AI-Assisted Development

AI tools (ChatGPT + inline completions) were used in the following ways:

- Folder & File Scaffolding: Suggested the optimal folder structure (/auth/login, /auth/register, /components/...).

- Code Generation: Produced JSX layouts for LoginForm.tsx and RegisterForm.tsx with Supabase integration.

- Supabase Setup: Guided .env.local, supabaseClient.ts, and auth-context.tsx.

- UI Components: Suggested imports and usage of shadcn/ui (Button, Input, Label).

- Commit Messages: Drafted clear, semantic commit messages (e.g., feat: add Supabase client setup).

- Documentation: Helped generate this comprehensive README.

## Example Usage

- Navigate to /auth/register → Register a new account.

- Navigate to /auth/login → Login with the registered credentials.

- Session state is automatically tracked with AuthProvider.

## Screenshots (to be added)

- Add screenshots of login/register forms and AI prompts used in development.

## Commit Convention

All commits follow Conventional Commits:

- feat: → New feature (e.g., feat: add login form with Supabase integration).

- chore: → Build/maintenance tasks (e.g., chore: scaffold Next.js project).

- style: → UI/UX updates (e.g., style: improve login form with shadcn/ui).

## Next Steps

- Add poll creation & voting features.

- Implement protected routes (only logged-in users can vote).

- Extend UI with charts for results visualization.

- Deploy on Vercel.

## Contributors

- Bethel Amadi (Lead Developer, AI Product Architect)

- AI Assistant (ChatGPT) (Code scaffolding, documentation, commit drafting)
