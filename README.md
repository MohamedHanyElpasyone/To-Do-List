# To-Do List

A simple to-do list application built with Vue 3, TypeScript, and Tailwind CSS.

## Live Demo

(Soon)

## What it Solves

This app helps users manage daily tasks without losing progress. Unlike paper lists or unsaved digital notes, tasks persist in browser storage — so your to-do list is still there when you close and reopen the app.

**Key benefits:**

- **Never lose tasks** — data saved to browser's localStorage
- **Stay organized** — see what's pending vs. completed at a glance
- **Simple & fast** — no accounts, no setup, just open and start

## Features

- **Add tasks** — quickly create new to-do items
- **Mark complete** — check off finished tasks
- **Delete tasks** — remove items you no longer need
- **Filter views** — switch between All, Active, and Completed tabs
- **Persistent storage** — tasks survive page refreshes and browser restarts

## Tech Stack

- **Vue 3** - Progressive JavaScript framework
- **TypeScript** - Type-safe JavaScript
- **Vite** - Fast build tool and dev server
- **Tailwind CSS v4** - Utility-first CSS framework

## Getting Started

### Prerequisites

- Node.js ^20.19.0 || >=22.12.0

### Install Dependencies

```bash
npm install
```

### Run Development Server

```bash
npm run dev
```

Open http://localhost:5173 to view the app.

### Build for Production

```bash
npm run build
```

The production files will be generated in the `dist/` folder.

### Preview Production Build

```bash
npm run preview
```

## Available Scripts

| Command           | Description                            |
| ----------------- | -------------------------------------- |
| `npm run dev`     | Start development server               |
| `npm run build`   | Build for production (with type check) |
| `npm run preview` | Preview production build locally       |
| `npm run lint`    | Run all linters (ESLint + Oxlint)      |
| `npm run format`  | Format code with Prettier              |

## Project Initial Structure

```
├── src/
│   ├── assets/          # Static assets
│   ├── components/      # Reusable components
│   ├── App.vue          # Root component
│   ├── main.ts          # Application entry point
│   └── main.css         # Global styles + Tailwind
├── index.html           # HTML template
├── vite.config.ts       # Vite configuration
└── package.json         # Dependencies and scripts
```
