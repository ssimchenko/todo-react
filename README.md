# Todo React

A course-based task manager built to practise modern React fundamentals in a complete application.

[Live demo](https://ssimchenko.github.io/todo-react/) · [React course](https://www.youtube.com/playlist?list=PL0MUAHwery4omH4GyVQ-lI2R326tOdN7A)

## What it can do

- Add, complete and delete tasks
- Search tasks with safe text highlighting
- Persist data in `localStorage`
- Open a separate details page for each task
- Show task statistics and scroll to the first incomplete item
- Animate task creation and deletion

## What I practised

- React components, props and controlled forms
- State management with `useState`, `useReducer` and Context
- Effects, refs, memoisation and custom hooks
- A small router implemented without a routing library
- A replaceable data layer for `localStorage` and `json-server`
- SCSS Modules and feature-oriented project structure
- Production builds and deployment to GitHub Pages

## Tech stack

`React 19` · `JavaScript` · `Vite` · `SCSS Modules` · `ESLint` · `json-server`

## Project structure

```text
src/
├── app/       # application setup, global styles and routing
├── pages/     # route-level screens
├── widgets/   # composed interface blocks
├── features/  # add, search and statistics features
├── entities/  # task model, hooks and UI
└── shared/    # reusable UI, API adapters and utilities
```

The structure is inspired by Feature-Sliced Design and keeps domain logic separate from reusable UI and infrastructure.

## Run locally

```bash
npm install
npm run dev
```

The production build can be checked with:

```bash
npm run build
npm run preview
```

The app uses `localStorage` by default. To practise requests against `json-server`, start `npm run server` and run Vite with `VITE_STATIC_BACKEND=false`.

## Learning project note

I built this project while completing Alexander Lamkov's [React course](https://www.youtube.com/playlist?list=PL0MUAHwery4omH4GyVQ-lI2R326tOdN7A). The application follows the course implementation and was used to study each stage hands-on, from components and hooks to architecture and deployment.

The original lesson-by-lesson history and reference implementation are available in the [course repository](https://github.com/aleksanderlamkov/todo-react). This repository contains my completed course version, repository cleanup and documentation.
