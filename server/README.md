# API server

Express modular monolith. Part of [Fidelyra](../README.md).

> **Structure only.** The source code is private. Source files here are intentionally empty so you can see how the project is organized. Commands describe the private codebase.

## Responsibilities

- Merchants, branches, terminals and staff
- Loyalty programs, rewards and ledger
- Checkout with rotating QR challenges
- Circles, referrals, reviews and discovery
- Socket.IO with Redis adapter
- OpenAPI document

## Main dependencies

`@socket.io/redis-adapter`, `bcrypt`, `cors`, `dotenv`, `express`, `express-rate-limit`, `helmet`, `ioredis`, `joi`, `jsonwebtoken`, `pino`, `pino-http`, `pg`, `rate-limit-redis`, `sequelize`, `socket.io`, `swagger-ui-express`, `uuid`

## Structure

```text
src/                              2 files
src/config/                       6 files
src/database/                     5 files
src/docs/                         1 file
src/jobs/                         1 file
src/middleware/                   7 files
src/modules/                      101 files
src/tests/                        1 file
src/utils/                        6 files
```

## Commands

```bash
npm install
npm run dev
npm start
npm run db:migrate
npm run db:seed
npm test
npm run lint
```
