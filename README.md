# Project Template

A simple Vite-based frontend project with a help modal and AI-powered prompt support.

## Features

- Static frontend built with Vite
- `main.js` controls a help button and modal interaction
- `prompt.js` defines the prompt content sent to the AI
- Uses `groq-sdk` for chat completion requests
- Supports environment-based API key configuration

## Project Structure

- `index.html` — main landing page
- `orders.html`, `profile.html` — additional static pages
- `main.js` — application logic, button click handler, and AI call
- `prompt.js` — prompt content generator
- `env.js` — API key helper for environment variables
- `style.css` — project styling
- `vite.config.js` — Vite configuration

## Setup

1. Install dependencies:

```bash
npm install
```

2. Add your API key to a root `.env` file:

```env
VITE_GROK_API_KEY=your_api_key_here
```

3. Start the development server:

```bash
npm run dev
```

4. Open the URL shown in the terminal to view the app.

## Usage

- Click the **Help** button on the page to open the help modal.
- The app sends the prompt from `prompt.js` to the AI service and displays the response in the modal body.

## Notes

- The project uses Vite environment variables, so the client-side variable must be prefixed with `VITE_`.
- Keep API keys secret and do not commit them to source control.
- `.env` is already ignored by `.gitignore`.

## Build

To create a production build:

```bash
npm run build
```

To preview the production build locally:

```bash
npm run preview
```
