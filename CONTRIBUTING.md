# Contributing to Fleemail Web

Thanks for helping improve Fleemail Web.

## Local setup

This project has no build step. Clone the repository and serve its root directory:

```bash
npx serve .
```

## Development guidelines

- Keep the client dependency-light and usable on desktop and mobile.
- Preserve keyboard navigation and visible focus states.
- Sanitize all message HTML before rendering it.
- Never add mailbox credentials, server secrets, or private messages to the repository.
- Update the preview image and README when a visible workflow changes substantially.

## Pull requests

Keep changes focused and explain the user problem they solve. Test inbox loading, message reading, saved inboxes, mobile navigation, loading states, and API failure states. Include before-and-after screenshots for interface work.

## Bug reports

Include reproduction steps, expected behavior, actual behavior, browser, and device. Remove email content, personal addresses, credentials, and tokens from screenshots or logs.
