# Security Policy

Spike researches security issues in other projects. Its own code and configuration should also be handled responsibly.

## Reporting a vulnerability in Spike

Do **not** disclose exploitable details, credentials, or private data in public GitHub issues or pull requests.

If GitHub's private vulnerability reporting feature is enabled for this repository, use **Security → Report a vulnerability**. If the feature is not available, contact the repository maintainer privately through a contact channel they have explicitly published before sharing sensitive details.

Please include:
- A concise description of the issue and affected component
- Reproduction steps that do not expose third-party private data
- Potential impact and any safe mitigation suggestions

Do not upload secrets, credentials, or live exploit material.

## Researching external projects

- Only test systems within an authorized scope.
- Follow each project's security policy and coordinated disclosure process.
- Do not confuse scanner output with confirmed exploitable vulnerabilities.
- Never publish an unpatched vulnerability or automatically submit a public proof-of-concept without authorization.

## Credentials

Use local environment variables or an appropriate secrets manager for GitHub and model-provider tokens. Do not commit `.env` files, credentials, or generated reports containing sensitive information.
