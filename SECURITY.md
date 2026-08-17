# Security policy

## Reporting a vulnerability

Please use GitHub's private vulnerability reporting for this repository. Do not publish an exploit, mailbox data, credentials, or private email content in an issue.

Include a concise description, reproduction steps, impact, and any suggested mitigation. You should receive an initial response within seven days.

## Supported version

Security fixes target the latest commit on the `main` branch.

## Security model

Fleemail Web is a public browser client. Incoming email HTML must be sanitized before it reaches the document, and the frontend must never contain private backend credentials. Treat temporary inboxes as public identifiers and do not use them for sensitive accounts.
