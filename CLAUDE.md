# School Scheduler

Automatic school timetable generator and editor built with Angular 21.

## Tech Stack

- Angular 21 (standalone components, signals)
- TypeScript 5.9 (strict mode)
- Angular Material + CDK (drag & drop, UI components)
- SCSS with Material theming (cyan primary, orange tertiary)
- Vitest for unit testing
- ESLint + Prettier

## Commands

- `npm start` / `ng serve` - dev server at localhost:4200
- `npm run build` / `ng build` - production build (output in dist/)
- `npm test` / `ng test` - run unit tests with Vitest
- `npm run lint` / `eslint .` - lint

## Code Style

- Tabs for indentation (size 4)
- Single quotes in TypeScript
- Print width: 100
- HTML files use Angular parser for Prettier
- Standalone components (no NgModules)
- Use Angular signals for reactive state
- Component files: `name.ts`, `name.html`, `name.scss` (no `.component` suffix)
- Prefix: `app`

## Project Structure

- `src/app/` - application source
- `src/styles.scss` - global styles with Material theme
- `public/` - static assets
- `docs/` - feature documentation and INDEX.md
- `.claude/agents/` - custom Claude agents (planner, frontend-developer)

## Architecture Notes

- Slot-based schedule model: lessons placed into predefined weekly time slots
- Three main sections planned: Schedule (timetable editor), Workload (teacher analysis), Setup (config)
- Uses Angular Router for navigation
- No backend - client-side only