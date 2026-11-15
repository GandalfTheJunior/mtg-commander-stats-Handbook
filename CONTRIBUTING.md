# Contributing to the Developer Handbook

Keep this repository lightweight. The goal is a useful learning resource for human developers, **not** a second development-process or agent-rule system.

## Content boundaries

- Prefer short, task-oriented pages with observable checkpoints. Explain enough to teach; link to authoritative material in the [application repository](https://github.com/GandalfTheJunior/mtg-commander-stats) for exact technical contracts and policies.
- Do not copy entire product specifications, security rules, architecture decisions, or testing references.
- Write documentation in English. Explain German application UI terminology where it helps a human reader.
- Do not include passwords, authentication cookies, CSRF tokens, invitation or claim codes, real user data, or unredacted diagnostic output.

## Every published page

State clearly:

- **Application commit:** the full SHA of the application version checked.
- **Verified:** date, operating system/environment, and human verifier (name or GitHub handle).
- **Depends on:** relevant paths in the application repository whose changes should prompt rechecking this page.

For a practical walkthrough, include the goal, prerequisites, steps, expected results, useful recovery steps, and links to authoritative references. Keep examples tied to observed behavior rather than assumptions.

## Human validation and review

1. Draft **one useful page at a time**. AI assistance can propose text but cannot certify its correctness.
2. A human follows the instructions **without a coding agent**, or for a system-map page independently checks the described routes and code paths.
3. Add a brief redacted record under `walkthroughs/`: page, application commit, date, platform, verifier, reached checkpoints, confusing steps, and any corrections made.
4. Correct the page based on the observed result and update its verification stamp.
5. Submit the change for human review via a pull request. No AI-authored change should be merged automatically.

A changed application file is a reason to **review** dependent pages, not proof that their content is wrong. Recheck before updating the verification stamp.

## Keeping the application workflow independent

Documentation feedback and PRs belong here. This handbook does not establish new requirements for pull requests in the application repository; its existing process and authoritative documentation remain unchanged.
