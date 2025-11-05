# 🚀 Ultimate Task Manager Pro

**Ultimate Task Manager Pro** is a modern, feature-rich web application for comprehensive personal and project task management — all contained in a **single HTML file**.  
It showcases advanced **React state management**, **dynamic styling**, and **complex data organization**, while maintaining **zero setup complexity**.

---

## ✨ Key Features

### ⚙️ Architecture
- **Single-File Application:** Entire app resides in `index.html` using CDN imports — no build tools, no installs, no dependencies.
- **Persistent Storage:** Uses browser `localStorage` (via React `useEffect`) to automatically save and load tasks across sessions.

### 🧩 Advanced Task Management
- **Subtasks / Checklists:** Break down larger tasks into manageable steps.
- **Tags:** Add searchable tags (e.g., `#urgent`, `#client-a`) for flexible grouping.
- **Notes / Comments:** Built-in editor for adding detailed context to tasks.
- **Priority & Categorization:** Assign **High**, **Medium**, or **Low** priority, and categorize under **Work**, **Personal**, or **Health**.

### 🔍 Smart Search, Filter, and Sort
- **Universal Search:** Real-time, case-insensitive search across title, category, priority, notes, and tags.
- **Dynamic Filtering:** Filter by status (Active/Completed), category, or tag.
- **Sorting Options:** Sort by **Priority**, **Due Date**, or **Completion Date**.

### 🎨 Modern UI & Theming
- **Tailwind CSS** for a sleek, responsive design.
- **Instant Dark/Light Mode** with automatic preference detection and persistence.
- **Responsive Layout** for all devices.

### 📊 Completion Tracking
- Automatically records the exact date and time when a task is completed.

---

## 🛠️ Technology Stack

| Component | Technology |
|------------|-------------|
| **Framework** | React 18 (Hooks: `useState`, `useEffect`, `useMemo`, `useRef`) |
| **Styling** | Tailwind CSS (CDN-based) |
| **Transpilation** | Babel Standalone (in-browser JSX compilation) |
| **Storage** | Browser `localStorage` |
| **Build Setup** | None — all via CDN imports |

---

## 🚀 Getting Started (Zero Setup)

1. **Save the Code**
   - Copy the complete code from the provided `index.html` file.
2. **Run the App**
   - Save it as `index.html` on your system.
   - Open it directly in any modern web browser (Chrome, Firefox, Edge, etc.).
3. **Done!**
   - The app loads instantly, manages persistence automatically, and is ready to use.

---

## 📝 Usage Guide

### ➕ Adding Tasks
- Enter a **task title** and optional metadata (**Due Date**, **Category**, **Priority**, **Tags**).
- Use commas to separate multiple tags (e.g., `bug, review, v1.0`).
- Click the ➕ button to add the task.

### 🔎 Filtering
- Use filter buttons to narrow tasks by **Status**, **Category**, or **Tags**.

### 🧭 Task Actions
| Action | Description |
|--------|--------------|
| ✅ Circle Checkmark | Toggle completion |
| ✏️ Pencil | Edit task title, notes, and tags |
| 🗒️ Notes Icon | Open detailed notes editor |
| 🗑️ Trash | Delete task |

### 🧾 Subtasks & Notes
- Expand a task to add **subtasks** or write detailed **notes** for context.

---

## 💡 Code Highlights

### 🔁 Main Component
All core logic resides inside the `App` functional component.

### ⚡ Performance & Logic Hooks
- **`useMemo`**: Memoizes filtered and sorted task lists for efficient rendering.
- **`useEffect`**: Handles side effects — theme persistence, localStorage sync, and initialization.
- **`useState`**: Manages all UI and task states dynamically.

### 🎨 Dynamic Styling
- Theme and UI classes (`themeClasses`, `inputClasses`, etc.) switch Tailwind utilities based on dark/light mode.
- Instant theme transitions powered by conditional rendering and state-based class toggling.
