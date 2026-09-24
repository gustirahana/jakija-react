# JakIja React LMS

A new React and NestJS implementation of an LMS inspired by the feature areas in [JakIja](https://github.com/johansantri/jakija). This repository is maintained by Gusti Rahana and is not the upstream JakIja repository.

## Purpose

This project is created for learning and educational purposes. It is a hands-on project for exploring how to build a learning management system with React and NestJS.

The upstream project is MIT licensed. This implementation follows its README attribution requirement and credits JakIja below.

## Repositories

- Main project: [gustirahana/jakija-react](https://github.com/gustirahana/jakija-react)
- Frontend: [gustirahana/lms-react-frontend](https://github.com/gustirahana/lms-react-frontend)
- Backend: [gustirahana/lms-backend](https://github.com/gustirahana/lms-backend)
- Upstream project: [johansantri/jakija](https://github.com/johansantri/jakija)

## Structure

```text
FE/   React + Vite learner web application
BE/   NestJS API
```

## Requirements

- Node.js 20 or newer
- npm

## Getting started

Install each app's dependencies and start the development servers in separate terminals:

```sh
cd FE && npm install && npm run dev
```

```sh
cd BE && npm install && npm run start:dev
```

The frontend reads API requests from `/api` and proxies them to `http://localhost:4000` during development. Configure `VITE_API_URL` when using a separately hosted backend.

## Attribution

Creator: JakIja — https://github.com/johansantri/jakija
