# JakIja React LMS

A React and NestJS learning management system inspired by feature areas in [JakIja](https://github.com/johansantri/jakija). This is a new implementation maintained by Gusti Rahana, not the upstream JakIja repository.

## Purpose

This project is for learning and educational purposes. It is a hands-on project for exploring how to build a learning management system with React, NestJS, and Supabase.

The upstream project is MIT licensed. This implementation follows its README attribution requirement and credits JakIja below.

## Repositories

- Project index: [gustirahana/jakija-react](https://github.com/gustirahana/jakija-react)
- Frontend: [gustirahana/lms-react-frontend](https://github.com/gustirahana/lms-react-frontend)
- Backend: [gustirahana/lms-backend](https://github.com/gustirahana/lms-backend)
- Upstream project: [johansantri/jakija](https://github.com/johansantri/jakija)

The frontend and backend are maintained in their own repositories. This repository is the project index and does not contain the application source as a monorepo.

## Architecture

- Frontend: React + Vite learner application
- Backend: NestJS API
- Authentication and database: Supabase Auth and Postgres
- Browser sessions: server-issued HttpOnly cookies
- Live updates: authorization-aware Socket.IO namespaces and course rooms

## Local development

Clone the frontend and backend repositories separately:

~~~sh
git clone https://github.com/gustirahana/lms-react-frontend.git
git clone https://github.com/gustirahana/lms-backend.git
~~~

Configure and start the backend first. Follow its README to set up Supabase credentials, apply the database migration, and generate the session encryption key:

~~~sh
cd lms-backend
cp .env.example .env
npm ci
npm run start:dev
~~~

In another terminal, start the frontend:

~~~sh
cd lms-react-frontend
cp .env.example .env.local
npm ci
npm run dev
~~~

The frontend uses the same-origin /api path by default. For local development, Vite proxies API and Socket.IO requests to http://localhost:4000.

See the [frontend README](https://github.com/gustirahana/lms-react-frontend#readme) and [backend README](https://github.com/gustirahana/lms-backend#readme) for environment configuration, verification commands, and deployment prerequisites.

## Attribution

Creator: JakIja — https://github.com/johansantri/jakija
