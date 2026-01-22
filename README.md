# TypeScript Project Management App

A modern, browser-based project management application built entirely with TypeScript. This app demonstrates TypeScript's strengths in type safety, object-oriented programming, and interactive UI development.

## Features

- **Add Projects:** Create new projects with a title, description, and number of people.
- **Project Lists:** Projects are organized into Active and Finished lists for easy tracking.
- **Drag and Drop:** Move projects between lists using intuitive drag-and-drop functionality.
- **Input Validation:** Ensures only valid projects are added, with checks for required fields and value ranges.
- **Component-Based UI:** Modular, reusable UI components for maintainability and scalability.

## TypeScript Highlights

- **Type Safety:** All variables, function parameters, and return types are explicitly typed for reliability and maintainability.
- **Enums:** Uses the `ProjectStatus` enum to manage project states (`Active` and `Finished`).
- **Classes & Inheritance:**
  - `Project`, `State`, `ProjectState`, `Component`, `ProjectItem`, `ProjectList`, and `ProjectInput` classes structure the app.
  - `Component` is an abstract base class for reusable UI components.
- **Interfaces:**
  - `Draggable` and `DragTarget` interfaces define contracts for drag-and-drop functionality.
  - `Validatable` interface is used for input validation.
- **Singleton Pattern:** `ProjectState` uses a static instance to ensure a single state manager.
- **Decorators:** The `autobind` decorator is used to automatically bind event handler methods to their class instances.
- **Generics:** The `State<T>` class is generic, allowing for flexible state management.
- **Type Guards:** Type checks are used throughout for safe property access and event handling.

## Architecture Overview

- **State Management:** Centralized project state using a singleton pattern. Listeners are notified of changes for reactive UI updates.
- **Component System:** Abstract `Component` class for all UI elements, supporting easy extension and code reuse.
- **Drag-and-Drop:** Interfaces and event handlers enable moving projects between lists with visual feedback.
- **Validation:** Input validation logic ensures data integrity before adding projects.

## How TypeScript Improves This Project

- Prevents runtime errors by catching type issues at compile time.
- Makes code easier to refactor and maintain.
- Enables powerful IDE features like autocompletion and inline documentation.
- Encourages modular, object-oriented design.
- Provides clear contracts for components and state management.
