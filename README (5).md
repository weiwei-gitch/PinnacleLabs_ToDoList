# TaskFlow — Web To-Do List App

A clean, feature-rich to-do list web application built with plain HTML, CSS, and JavaScript. No frameworks, no dependencies, no build tools — just open the file in a browser and start using it.

---

## Features

### Task Management
- **Create tasks** — add a title, optional due date, and priority level
- **Edit tasks** — update title, due date, or priority inline
- **Delete tasks** — remove tasks with a single click
- **Mark complete** — toggle tasks as done/pending with an animated checkbox

### Priority Levels
Tasks can be assigned one of three priority levels, each color-coded for quick scanning:
- 🔴 **High** — urgent tasks
- 🟠 **Medium** — default priority
- 🔵 **Low** — non-critical tasks

### Smart Filters & Sorting
Filter tasks by: **All · Pending · Done · Overdue · High Priority**

Sort tasks by: **Newest · Oldest · Due Date · Priority**

### Progress Tracking
An overall progress bar shows the percentage of completed tasks at a glance, alongside a stats grid displaying Total, Completed, Overdue, and Pending counts.

### Calendar View
A full monthly calendar displays tasks on their due dates, color-coded by priority. Navigate months with the arrow buttons and spot overdue or upcoming tasks instantly.

### Persistence
All tasks are saved to `localStorage` automatically — data survives page refreshes and browser restarts.

### Dark Mode
Toggle between light and dark themes using the button in the sidebar. The warm amber palette adapts cleanly to both modes.

### Responsive Layout
The sidebar collapses to icon-only mode on smaller screens (below 700px), keeping the interface usable on mobile.

---

## Pages

| Page | Description |
|------|-------------|
| **My Tasks** | Main task manager with stats, progress bar, add form, filters, and task list |
| **Calendar** | Monthly calendar view with tasks plotted on their due dates |

---

## Getting Started

No installation or setup needed.

1. Download `todo-app.html`
2. Open it in any modern browser (Chrome, Firefox, Edge, Safari)
3. Start adding tasks

> An internet connection is required on first load to fetch the Tabler Icons font from jsDelivr CDN. After that, the app works fully offline.

---

## Project Structure

```
todo-app.html
├── HTML        — layout, sidebar, task list, calendar grid
├── CSS         — variables, dark mode, animations, responsive rules
└── JavaScript  — task logic, localStorage, filtering, calendar rendering
```

Everything lives in a single `.html` file with no external dependencies beyond the Tabler Icons webfont.

---

## Tech Stack

| Layer | Technology |
|-------|-----------|
| Markup | HTML5 |
| Styling | CSS3 (custom properties, grid, flexbox) |
| Logic | Vanilla JavaScript (ES6+) |
| Icons | [Tabler Icons](https://tabler.io/icons) v3.19 |
| Storage | `localStorage` API |

---

## Browser Support

Works in all modern browsers. Requires ES6+ support (Chrome 60+, Firefox 55+, Edge 79+, Safari 12+).

---

## Customisation

All colors are defined as CSS custom properties in the `:root` block at the top of the `<style>` tag, making it easy to re-theme the app:

```css
:root {
  --a400: #E8922A;   /* primary accent */
  --a600: #B86A10;   /* hover / active */
  --bg:   #FFF8F0;   /* page background */
}
```

Dark mode overrides live in the `[data-theme="dark"]` block directly below.

---

## License

Free to use and modify for personal and commercial projects.
