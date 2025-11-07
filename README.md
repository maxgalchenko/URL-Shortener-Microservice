# URL Shortener Microservice

<div align="center">

![Node.js](https://img.shields.io/badge/Node.js-12.x-339933?logo=node.js&logoColor=white)
![Express](https://img.shields.io/badge/Express-4.x-black?logo=express&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-Database-47A248?logo=mongodb&logoColor=white)
![Mongoose](https://img.shields.io/badge/Mongoose-ORM-880000)

</div>

## Overview

A simple URL shortener API built for the freeCodeCamp APIs & Microservices curriculum. It lets users create short URLs and redirects short codes to their original destinations using a MongoDB backend.

## Key Features

- Create short URLs via `POST /api/shorturl/new`
- Redirect to original URLs via `GET /api/shorturl/:shorturl`
- Utility endpoints to view count and clear data

## Tech Stack

Node.js 12, Express 4, MongoDB, Mongoose 5, JavaScript

## Architecture

Express server with REST endpoints; MongoDB via Mongoose with a `shorturl` model holding `original_url` and an incremental `short_url` id. Serves a static client from the `build/` directory for a minimal landing page.

## Performance & Accessibility

Lightweight API with minimal middleware and static asset serving; accessibility is not applicable beyond the static landing page.

## Quality

- Linting: None • Formatting: None
- Type safety: JavaScript (no TypeScript)
- Tests: None
- CI: None • Coverage: N/A

## Prerequisites

- Node.js: `12.18.3`
- MongoDB: connection URI

## Installation

```bash
git clone https://github.com/maxgalchenko/URL-Shortener-Microservice.git
cd URL-Shortener-Microservice
npm install
```

## Environment Variables

```env
MONGO_URL=mongodb://localhost:27017/url-shortener
PORT=8080
```

## Quick Start

```bash
npm run dev
# Production
npm run build
npm start
```

Open http://localhost:8080

## Available Scripts

- `npm run dev` – Start the server in development with nodemon.
- `npm run build` – Not available.
- `npm test` – Not available.
- `npm start` – Start the server.

---

<div align="center">

Built with ❤️ by [Maksym Galchenko](https://github.com/maxgalchenko)

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?style=for-the-badge&logo=linkedin)](https://www.linkedin.com/in/galchenko-max/)
[![Portfolio](https://img.shields.io/badge/Portfolio-Visit-green?style=for-the-badge&logo=web)](https://portfolio-green-six-29.vercel.app/)
[![Email](https://img.shields.io/badge/Email-Contact-red?style=for-the-badge&logo=gmail)](mailto:galchenko.maksym@gmail.com)
![License](https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge)

</div>
