# MTG Commander Stats — Developer Handbook

Human-first guidance for developers who want to understand, run, debug, test, and maintain [MTG Commander Stats](https://github.com/GandalfTheJunior/mtg-commander-stats) (also referred to as **Cozy Commander**) without depending on coding agents.

> **Status: bootstrap.** The handbook structure exists, but no guide has been written or validated yet. Planned chapters are not published instructions.

## Where to start

| Planned guide | Purpose | Status |
| --- | --- | --- |
| Getting Started | Clone the application, install prerequisites, start the stack, and open it in a browser | Not written |
| System Map | Understand the browser, Vite, Spring Boot, PostgreSQL, and where the corresponding code lives | Not written |

We will add each guide only after a developer has checked it against the actual application without using a coding agent.

## Repository layout

- `pages/` — short, practical developer guides and codebase orientation.
- `walkthroughs/` — redacted records of human verification for those guides.
- [`CONTRIBUTING.md`](CONTRIBUTING.md) — the minimal rules for writing and reviewing handbook content.

## Source of truth

This handbook **teaches, orients, and links**. It is not a normative specification for application behavior, architecture, security, or development policy. Those sources remain in the [application repository](https://github.com/GandalfTheJunior/mtg-commander-stats), including its [README](https://github.com/GandalfTheJunior/mtg-commander-stats/blob/main/README.md), `docs/`, code, and tests.

A handbook guide records the application commit and environment against which it was checked. That stamp is a verification record, not a promise that every later commit behaves identically.

## Feedback

Report unclear or outdated handbook instructions in [this repository's Issues](https://github.com/GandalfTheJunior/mtg-commander-stats-Handbook/issues). Report application defects in the [application repository's Issues](https://github.com/GandalfTheJunior/mtg-commander-stats/issues). When uncertain, start with a handbook issue and we can route it.

The handbook effort is coordinated in [application issue #272](https://github.com/GandalfTheJunior/mtg-commander-stats/issues/272).

**License:** To be selected by the repository owner before contributions or reuse terms are assumed.
