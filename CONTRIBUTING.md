# Contributing to Salon API

## Getting Started
1. Fork the repository
2. Clone your fork: `git clone https://github.com/your-username/salon-api`
3. Install dependencies: `npm install`
4. Copy environment variables: `cp .env.example .env`
5. Create a feature branch: `git checkout -b feature/your-feature`
6. Make your changes
7. Push and open a Pull Request against `develop`

## Branch Strategy
- `main` → production, never push directly
- `staging` → pre-production testing
- `develop` → active development
- `feature/` → new features
- `fix/` → bug fixes
- `hotfix/` → urgent production fixes

## Commit Convention
Write commits in English, imperative mood:
✅ Add booking endpoint
✅ Fix authentication bug
❌ added stuff
❌ fixed things

## Pull Request Rules
- Always target `develop` branch
- Fill out the PR template completely
- All Cubic review comments must be resolved
- PR title must be clear and descriptive

## Code Standards
- TypeScript only
- ESLint must pass: `npm run lint`
- Prettier formatting: `npm run format`
- Never commit `.env` files
- Never commit secrets or API keys

## Database Changes
- All database changes must go through Prisma migrations
- Never modify the database directly
- Run migrations: `npx prisma migrate dev`
- Update schema documentation in Notion after changes

## API Standards
- All endpoints must be versioned: `/v1/`
- All endpoints must be documented with Swagger decorators
- Follow RESTful conventions

## Reporting Bugs
Use the Bug Report issue template on GitHub.

## Suggesting Features
Use the Feature Request issue template on GitHub.

## Questions?
Open a GitHub Discussion or reach out via email.