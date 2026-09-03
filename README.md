<div align="center">

# Fleemail Web

**Temporary inboxes with a fast, calm, and security-conscious interface.**

![HTML](https://img.shields.io/badge/HTML-Semantic-E34F26?logo=html5&logoColor=white)
![CSS](https://img.shields.io/badge/CSS-Responsive-1572B6?logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-Vanilla-F7DF1E?logo=javascript&logoColor=111)
![SSE](https://img.shields.io/badge/Updates-Server--Sent_Events-7c3aed)
[![License: MIT](https://img.shields.io/badge/License-MIT-22c55e.svg)](LICENSE)

A clean, responsive frontend for temporary inboxes. Fleemail lets users open an address, read incoming messages, save frequently used inboxes, and switch comfortably between desktop and mobile layouts.

[**Open the live application →**](https://fleemail.netlify.app)

</div>

![Fleemail responsive inbox interface](assets/preview.webp)

## Experience at a glance

| Area | Experience |
| --- | --- |
| **Inbox** | Open any supported temporary address and follow incoming mail live |
| **Reading** | View complete messages in a focused reading surface |
| **Safety** | Sanitize incoming HTML with DOMPurify before rendering |
| **Continuity** | Save frequently used inboxes locally in the browser |
| **Responsive UI** | Move comfortably between desktop and mobile navigation |
| **Accessibility** | Use keyboard-friendly controls and semantic page structure |

## Features

- Temporary inbox lookup
- Live inbox updates
- Safe email HTML rendering with DOMPurify
- Full message reading experience
- Saved inboxes stored locally in the browser
- Responsive desktop and mobile navigation
- Keyboard-friendly interactions

## Data flow

```text
Temporary mailbox service
        ↓ HTTPS + live events
Fleemail browser client
        ↓ sanitize untrusted message HTML
Safe inbox and message reader
```

## Built with

- Semantic HTML
- Modern CSS
- Vanilla JavaScript
- Server-sent events
- DOMPurify
- Netlify

## Run locally

No build step is required. Serve the directory with any static file server:

```bash
npx serve .
```

Then open the URL printed in your terminal.

## Architecture

This public repository contains the browser interface. It communicates with the separately maintained Fleemail mail service over HTTPS. Mailbox credentials and server configuration are intentionally not part of this repository.

## Security

Incoming message HTML is sanitized before it is rendered. Do not commit mailbox credentials, API secrets, or private server configuration to this frontend repository.

## Project documentation

- [Contributing guide](CONTRIBUTING.md) — local workflow, testing checklist, and pull-request expectations
- [Security policy](SECURITY.md) — private reporting and frontend security boundaries

## License

Released under the [MIT License](LICENSE).
