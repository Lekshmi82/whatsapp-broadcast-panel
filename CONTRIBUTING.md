# Contributing

Thanks for helping. Bug reports, fixes and improvements are all welcome.

## Ground rules
- **Responsible use only.** Don't add features whose main purpose is unsolicited or bulk messaging to people who didn't opt in: scraping contacts, messaging non-members, evading WhatsApp's limits, or rotating numbers. Pull requests like that will be closed.
- **Safety checks stay.** Keep the typed confirmation, the pauses between groups, stop-on-error and the "already sent" skip.
- **Privacy:** never log or upload phone numbers, message contents or login data. Read reports contain counts only.
- **Never commit** `.wwebjs_auth/`, `.panel-token`, CSV files, messages or images. `.gitignore` covers them.

## Development
```bash
npm install
npm test        # runs with a simulated WhatsApp; nothing is sent
npm start       # the panel at http://localhost:3939
```
- Add or update tests for any change to sending, planning or the panel API (`test/`).
- The page in `panel/public/` is plain HTML, CSS and JavaScript. Keep it build-free and accessible (keyboard, labels, contrast).
- Changes to `vendor/` should stay minimal, be marked `LOCAL PATCH` and be documented in `vendor/README.md`.

## Reporting a bug
Please include the panel's error text (or the terminal output) and your OS and Node.js version. **Remove phone numbers, group names and IDs** before posting.
