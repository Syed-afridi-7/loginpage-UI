# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Commands

- `npm start` — dev server on http://localhost:3000
- `npm test` — run tests (Jest, interactive watch mode)
- `npm run build` — production build to `build/`

## Architecture

Create React App (React 18) project with a single-page login/signup form. No routing, no backend.

`App.js` renders `LoginPage`, which is the entire application — a togglable login/signup form with client-side validation, password strength indicator, and simulated async submit (2s delay, no actual API call). Social login buttons (Google, GitHub) are visual-only stubs.

All styling is in `LoginPage.css` using plain CSS with animations and responsive breakpoints. The app uses the Inter font loaded from Google Fonts CDN.
