# Contributing to Spike

Thanks for helping improve Spike. This repository contains an autonomous security-bounty research agent, so changes should prioritize accuracy, safety, and reproducibility.

## Local setup

1. Clone the repository and run `npm install`.
2. Copy `.env.example` to a local `.env` file.
3. Set the credentials required for the command you intend to run. Never commit `.env` or access tokens.
4. Check `./bin/spike` for the supported command interface and consult the README for usage examples.

## Proposing a change

1. Open an issue for significant changes so the scope is clear.
2. Create a branch and keep your change focused.
3. Explain what you changed, why it matters, and how you verified it in your pull request.
4. Report any limitations or tests you could not run.

The current `npm test` entry in `package.json` is a placeholder that exits with an error; it is **not** an automated test suite. Do not report it as a passing check.

## Security research

Only scan targets for which you have permission and follow each project's published disclosure and bounty rules. Avoid destructive tests, data extraction, or public publication of unpatched vulnerabilities. Never include secrets or sensitive findings in an issue or pull request.

See `SECURITY.md` when available for repository-specific reporting guidance.
