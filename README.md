# Vinith Ramaswamy

Full-stack software engineer. For the past 15 months I have been the sole engineer and operator of
[JustBook](https://justbookapp.com), a multi-tenant booking and operations platform for appointment
businesses that went live in August 2026.

B.S. Computer Science and B.S. Data Science, University of Wisconsin–Madison, May 2026.
Johns Creek, GA. Open to backend and full-stack roles, in person.
[LinkedIn](https://www.linkedin.com/in/vinith-ramaswamy-6a5964200) · vinithramaswamy@gmail.com

## JustBook, by the numbers

The repositories are private: JustBook is a live commercial product with customer data
flows, Stripe and Twilio integrations, and legal documents, so the code stays confidential. The
contribution graph on this profile is that work. Here is what is in it, as of September 2026.

| | |
|---|---|
| Application code | ~340K lines: Python (Flask, SQLAlchemy) and React 19 |
| API | 632 REST endpoints across 52 Flask blueprints |
| Database | 127-table PostgreSQL 16 schema, 129 Alembic migrations |
| Tests | 5,400+: 3,471 pytest, 1,729 Vitest, 255 Playwright E2E (desktop, iOS, Android) |
| CI guards | 19 custom checks that fail the build: unguarded routes, error-contract violations, doc drift, secrets in logs |
| Payments | Stripe Subscriptions, Connect direct charges, Terminal with Tap to Pay on iPhone and Android |
| Mobile | JustBook app shipped on iOS and Android (Capacitor): Tap to Pay, push (APNs/FCM), passkeys, barcode scanning |
| Infrastructure | Render (API, worker, cron), Cloudflare Workers, AWS S3, Redis, Sentry, staging mirror, daily off-platform backups |
| Messaging | ZeptoMail, Postmark, Twilio SMS, WhatsApp (34 Meta-approved templates) |
| Security | Server-enforced tenant and branch scoping, RBAC, JWT + TOTP + WebAuthn passkeys, rate limiting, audit log, GDPR privacy-request register |
| History | 2,400+ commits, May 2025 to present, one author |

## How it was built

Most of the code was written with AI coding agents (Claude Code) running concurrently on one
shared tree. What made that work was not the agents; it was the rules around them: a 640-line
engineering-standards document, 76 dated architecture decisions, and machine-checked invariants
that fail the build when a route ships without a guard, a doc drifts from the code it describes,
or an error response leaks internals. I own every architecture decision in that document.

## What I can show

- **[justbookapp.com](https://justbookapp.com)**: the product, the public docs, and the example
  booking pages.
- **Coming soon**: a self-contained tool extracted from JustBook, published with tests.
- **[neurosolis-preview](https://github.com/vramaswamy4/neurosolis-preview)**: a static site
  built for a biotech founding team (contract, 2026).

Older public repositories here are coursework and tutorial exercises from 2021 and are archived.
