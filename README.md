# Immunization Chat Bot — Prototype

A UI prototype for an immunization guidance chat bot, built for **Amref Health Africa** in partnership with the **Federal Ministry of Health, Ethiopia**.

Content and formulas are sourced from the *Immunization in Practice (IIP) Participant Manual*, MoH Ethiopia, Sept 2023 — Chapter 2 (Vaccine & Cold Chain Management).

---

## What's in this package

```
.
├── index.html
├── package.json
├── vite.config.js
├── README.md
└── src/
    ├── main.jsx                 # React entry point
    ├── App.jsx                  # Renders the chat bot
    └── ImmunizationChatBot.jsx  # Main application component
```

This is a **front-end only prototype** — there is no backend/server. Content (FAQs, calculators, forecasting logic) is hard-coded in `ImmunizationChatBot.jsx`, and OTP/login is a demo passthrough with no real validation, intended for UI review only.

---

## Requirements

- [Node.js](https://nodejs.org/) version 18 or later (includes `npm`)

To check if Node is installed, open a terminal and run:

```bash
node -v
npm -v
```

If these commands aren't found, download and install Node.js from https://nodejs.org/ (LTS version recommended), then re-open your terminal.

---

## Setup

1. Unzip this folder and open a terminal inside it.
2. Install dependencies:

   ```bash
   npm install
   ```

3. Start the local development server:

   ```bash
   npm run dev
   ```

4. Vite will print a local URL, typically:

   ```
   Local:   http://localhost:5173/
   ```

   Open that link in your browser (Chrome recommended). The app is designed as a mobile phone-sized screen, so it will appear centered on the page.

To stop the server, press `Ctrl + C` in the terminal.

---

## Building for deployment

To produce a static, production-ready build (for hosting on any static web host):

```bash
npm run build
```

This creates a `dist/` folder containing the final HTML/CSS/JS files. You can preview that build locally with:

```bash
npm run preview
```

The contents of `dist/` can be uploaded to any static hosting provider (e.g. Netlify, Vercel, GitHub Pages, or a plain web server).

---

## Notes for reviewers

- This is a **prototype for UI/UX and content review**, not a production system.
- No real data, patients, or credentials are used — login/OTP screens are for demonstration only.
- Works fully offline once loaded (no external API calls), aside from the initial page load.

---

## Support

For questions about this prototype, please contact the development team.
