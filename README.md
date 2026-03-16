# EasyTask — Angular Task Management App

A task management application built with **Angular 17+** as part of a structured learning path toward becoming a professional Angular developer.

---

## Built With

- **Angular 17+** — Frontend framework
- **TypeScript** — Strongly typed JavaScript
- **NgModule Architecture** — Feature-based module organization
- **Angular Forms** — Template-driven forms with `ngModel`
- **LocalStorage** — Client-side data persistence

---

## Angular Concepts Covered

| Concept                         | Implementation                                      |
| ------------------------------- | --------------------------------------------------- |
| Component Architecture          | `HeaderComponent`, `UserComponent`, `TaskComponent` |
| NgModule Pattern                | `AppModule`, `TasksModule`, `SharedModule`          |
| @Input / @Output                | User selection, task events                         |
| Services & Dependency Injection | `TasksService` with `providedIn: 'root'`            |
| Template-driven Forms           | New task creation with `[(ngModel)]`                |
| Content Projection              | `CardComponent` with `<ng-content>`                 |
| Angular Pipes                   | `DatePipe` for due date formatting                  |
| Control Flow (`@if`, `@for`)    | Conditional rendering & task lists                  |
| LocalStorage Persistence        | Tasks saved across page refreshes                   |

---

## Project Structure

```
src/app/
├── header/              # App header component
├── user/                # User list & selection
│   ├── user.component
│   ├── user.model.ts
│   └── dummy-users.ts
├── tasks/               # Task management feature
│   ├── task/            # Single task display
│   ├── new-task/        # Add task form
│   ├── tasks.component  # Tasks container
│   ├── tasks.service.ts # State & business logic
│   ├── tasks.module.ts  # Feature module
│   └── task.model.ts
└── shared/
    └── card/            # Reusable card component
        └── shared.module.ts
```

---

## Getting Started

### Prerequisites

- Node.js 18+
- Angular CLI 17+

```bash
npm install -g @angular/cli
```

### Installation

```bash
git clone https://github.com/YOUR_USERNAME/easytask-angular.git
cd easytask-angular
npm install
ng serve
```

Open your browser at `http://localhost:4200`

---

## Features

- View all users in a sidebar
- Select a user to see their tasks
- Add new tasks with title, summary, and due date
- Mark tasks as complete (removes from list)
- Tasks persist in localStorage across sessions

---

## Roadmap

- [ ] Angular Routing (multi-page navigation)
- [ ] Reactive Forms
- [ ] HTTP Client (REST API integration)
- [ ] RxJS & Observables
- [ ] Angular Signals
