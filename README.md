# Veyra Production

Server-backed AI website builder.

## Features
- Email/password accounts
- Natural-language website generation through OpenAI Responses API
- Structured design-system generation
- AI-generated website imagery
- Conversational edits
- Persistent projects and usage limits
- Public publishing at `/s/<slug>`
- Optional Stripe subscriptions and billing portal

## Environment
Copy `.env.example` to `.env` locally or configure the same variables in your hosting provider. Never commit API keys.

Minimum required: `OPENAI_API_KEY`, `SESSION_SECRET`, `APP_URL`.

## Run
`npm install`
`npm start`

## Production
This build uses SQLite and local generated-image storage. Attach persistent storage in production, or replace these with managed database/object storage before scaling horizontally.
