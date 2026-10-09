# Gavell

Software for intellectual property notices, professional review, and client instructions.

**[Website](https://gavell.ca)** · **[Daniel Iravani](https://danieliravani.com)**

## The project

Gavell carries an incoming intellectual property communication through review, client instruction, a resulting staff action, and a completion record. The application connects the public product site with a protected workspace for the people carrying out that workflow.

The engineering problem is maintaining a clear relationship between a notice, the version a professional reviewed, the instruction a client gave, and the action that followed.

## Engineering work

- Organization-scoped records and explicit matter access.
- Professional review and approved packet versions.
- Client instructions bound to a specific released version.
- Persisted workflow transitions, idempotency, and audit events.
- Document intake, private evidence storage, and integrity metadata.
- Advisory extraction with structured outputs and professional review.
- Subscription and integration boundaries with explicit readiness checks.

## Design decisions

**Versioned decisions.** A client instruction refers to the released packet the client actually saw. Editing a draft does not silently alter an approved version.

**Server-enforced workflow.** Authorization and state transitions are enforced by the application and database, with organization and matter boundaries carried through the data model.

**Professional authority.** The software supports the workflow; statutory deadlines, filing decisions, and professional approval remain with the responsible practitioner and firm systems.

**Stack:** TypeScript · Next.js · React · PostgreSQL · Clerk · S3-compatible storage

## About this repository

This is the public project overview and engineering summary for my work on Gavell. Application source is maintained in the Gavell project repositories.
