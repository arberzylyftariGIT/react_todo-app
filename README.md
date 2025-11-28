# 📝 React Todo App

A modern Todo application built with **React**, **TypeScript**, and **Vite**, using a dark UI theme and smooth animations.
This is a cleaned and customized portfolio version of a task originally done in a course – code structure, styling, and configuration are now independent and maintained by me.

---

## 🌐 Live Demo

https://reacttodo-app-alpha.vercel.app/

---

## 🚀 Features

### Core Functionality
- Add new todos
- Toggle todo status (active / completed)
- Edit todo titles inline
- Delete single todos
- Filter by **All / Active / Completed**
- Clear all completed todos
- Smooth animations when adding/removing todos

### UI / UX
- Dark theme with centered layout
- Custom checkbox-style circle for todo status
- Hover effects on items and delete button
- Clean, responsive design
- Inline edit input with focus styling
- Overlay when items are in loading/error state (depending on API state)

### Code & Architecture
- Component-based structure:
  - `Header`, `Footer`, `TodoList`, `TodoItem`, `Error` components
- Typed API layer for todos using `fetchClient`
- Strongly typed models in `src/types`
- Utility functions in `src/utils`
- SCSS split into:
  - `todoapp.scss` – main layout & card
  - `todo.scss` – single todo row styling
  - `filter.scss` – filters (All / Active / Completed)
  - `index.scss` – base & imports

---

## 🛠 Tech Stack

- **React 18**
- **TypeScript**
- **Vite**
- **SCSS / Sass**
- **React Transition Group**
- **classnames**

---

## 📂 Project Structure

```text
react_todo-app/
  public/
    icons/
  src/
    api/
      todos.ts
    components/
      Header/
        Header.tsx
      Footer/
        Footer.tsx
      TodoList/
        TodoList.tsx
      TodoItem/
        TodoItem.tsx
      Error/
        Error.tsx
    constants/
      ErrorMessage.tsx
    styles/
      index.scss
      todoapp.scss
      todo.scss
      filter.scss
    types/
      Todo.ts
      FilterTypes.ts
    utils/
      fetchClient.ts
    App.tsx
    index.tsx
  index.html
  package.json
  tsconfig.json
  vite.config.ts
