# Faqada — Public Architecture Overview

This document describes the Faqada Super Agent's architecture at a conceptual level. It intentionally excludes proprietary implementation details, credentials, private schemas, internal prompts, provider economics, and customer data.

## 1. One core

Every Super Agent runs on the same core:

**Genome → Brain → Foundry → Nightly Loop → Command**

- **Genome** — the business, captured as structured knowledge: identity, offers, voice, rules, standards, and history. Everything the system does is grounded in the Genome.
- **Brain** — the reasoning layer. It reads the Genome and the current state of the business, and turns them into decisions, priorities, and next actions.
- **Foundry** — the build layer. New operators, skills, and workflows are built and tested here before they are trusted with real work.
- **Nightly Loop** — the improvement cycle. Each cycle reviews what the system did, what worked, and what did not — and upgrades the Genome, the operators, and the workflows accordingly.
- **Command** — the owner's layer: priorities, approvals, and direction. The system proposes and executes; the owner directs.

## 2. Operators

The work is done by a team of **13 AI operators**, each with a defined job, defined tools, and a defined place in the chain of command — not one general-purpose assistant stretched across everything. Operators are coordinated through the core, scoped to the context their job requires, and auditable in what they do.

## 3. Six branches

The operators' work is organized into six branches, all operational:

- **Sales** — pipeline, follow-up, and sales execution;
- **Marketing & Content** — content, campaigns, and demand generation;
- **Operations** — the systems that keep the business moving day to day;
- **Customer Success** — onboarding, support, and retention;
- **Recruiting & Teams** — hiring, team building, and training;
- **Intelligence & Compliance** — research, monitoring, and guardrails.

## 4. Context model

Useful AI requires more than a prompt. The Super Agent combines only the context appropriate to the task, such as:

- the business's Genome — offers, voice, rules, and standards;
- customer and relationship state;
- prior communication and follow-up state;
- pipeline, campaign, and operating state;
- recent actions, outcomes, and performance signals.

Access to context remains scoped, permissioned, and purpose-specific.

## 5. Safety and control principles

Faqada's architecture favors:

- explicit authorization for consequential actions;
- clear boundaries between recommendation and execution;
- server-side protection of provider credentials;
- owner-scoped data access;
- auditable state transitions;
- idempotent economic and automation events;
- controlled provider access and spend;
- human-readable failure states instead of silent automation.

## 6. Model/provider strategy

The Super Agent is designed as **provider-agnostic**. Different jobs benefit from different models, modalities, latency profiles, and cost structures.

The abstraction is:

`Business intent → governed capability layer → approved model/provider → normalized result`

This lets the system evolve as the AI ecosystem changes, without the business's operations depending on a single vendor.

## 7. Measurement

The architecture is evaluated against practical business outcomes:

- faster, more consistent execution of routine work;
- better communication quality;
- follow-up that does not slip;
- clearer performance insight for the owner;
- skills and standards that compound instead of resetting;
- higher-quality next-action guidance.

## 8. What is intentionally not public

This document does **not** publish:

- production source code;
- private prompts or orchestration logic;
- internal schemas;
- provider keys or private endpoints;
- pricing or wholesale provider economics;
- customer data or examples derived from customer data;
- security-sensitive deployment details;
- proprietary ranking or attribution implementation.

That boundary is deliberate.
