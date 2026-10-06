# Coach AI — free, browser-only student planner

A static student planner hosted with GitHub Pages. There is no paid backend, sign-in, server database, or embedded API key.

## Features

- Add, prioritize, complete, and delete coursework with due dates and notes.
- See upcoming deadlines in the weekly calendar.
- Track subjects and personal learning activities.
- Use a small offline study helper for planning and breaking work into next steps.
- Export a JSON backup and restore it in another browser.
- Clear the data stored on the current device.

## Privacy and limits

Planner data is stored in `localStorage` in the browser. It stays on this device and browser profile, so it does not sync between devices. Anyone using the same browser profile may be able to see it. Export a backup before clearing browser data or switching devices.

The helper is rule-based and works offline; it is not a live Gemini model. A real Gemini service would need secure server-side key handling. GitHub Pages cannot run that server, and putting a shared API key in public browser code would expose it.

## Hosting

The public site is deployed from the `main` branch root of `EcTheEz/coach-ai-website` using GitHub Pages. Update `index.html`, `style.css`, and `app.js`, then commit to `main`; Pages republishes the static files.

No paid service is needed for this version.
