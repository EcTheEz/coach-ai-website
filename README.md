# Coach AI — free, browser-only student planner

A static student planner hosted with GitHub Pages. There is no paid backend, sign-in, server database, or embedded API key.

## Features

- Add, prioritize, complete, and delete coursework with due dates and notes.
- See upcoming deadlines in the weekly calendar.
- Track subjects and personal learning activities.
- Browse a study library with topic notes, question sets, a 10-question target test, and flip cards.
- Work through guided math, biology, chemistry, and English lessons with explanations, worked examples, three-question practice, and feedback.
- Save a Cambridge IGCSE course profile, level, subject, topic, and goal to personalize lesson framing and recommendations.
- Get weaker topics sorted to the top using practice results stored in the browser.
- Use the offline study helper for basic topic explanations and planning next steps.
- Use browser speech recognition to ask by voice and optional device text-to-speech to hear replies, when supported by the browser.
- Export a JSON backup and restore it in another browser.
- Clear the data stored on the current device.

## Privacy and limits

Planner data is stored in `localStorage` in the browser. It stays on this device and browser profile, so it does not sync between devices. Anyone using the same browser profile may be able to see it. Export a backup before clearing browser data or switching devices.

Lessons and the helper are prepared, rule-based learning aids and work offline; they are not a live Gemini model and do not understand every question. Cambridge IGCSE is a profile label only: the starter topics are not yet matched to specific syllabus codes or exam variants. Voice recognition and read-aloud depend on the browser/device and use its speech tools. A real Gemini service would need secure server-side key handling. GitHub Pages cannot run that server, and putting a shared API key in public browser code would expose it.

## Hosting

The public site is deployed from the `main` branch root of `EcTheEz/coach-ai-website` using GitHub Pages. Update `index.html`, `style.css`, and `app.js`, then commit to `main`; Pages republishes the static files.

No paid service is needed for this version.
Voice note: browser speech recognition may rely on that browser's own service and can require microphone permission; read-aloud depends on text-to-speech support. The app's typed coach replies and lesson content are processed in the page.
