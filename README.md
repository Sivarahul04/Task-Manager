# ✅ Task Manager

A beautiful, modern task management application built with HTML, Tailwind CSS, and vanilla JavaScript.

![Task Manager Preview](https://img.shields.io/badge/Status-Ready-green) ![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white) ![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?logo=tailwind-css&logoColor=white) ![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)

## 🌟 Features

### Core Functionality
- ➕ **Add Tasks** - Quickly add new tasks with the input form
- ✔️ **Complete Tasks** - Mark tasks as done with a single click
- 🗑️ **Delete Tasks** - Remove tasks you no longer need
- 💾 **Persistent Storage** - Tasks are automatically saved to localStorage

### Organization
- 🔍 **Filter Tasks** - View All, Active, or Completed tasks
- 📊 **Progress Tracking** - Visual progress bar shows completion percentage
- 🔢 **Task Counter** - See active and completed task counts at a glance

### User Experience
- 🎨 **Modern Design** - Beautiful gradient UI with smooth animations
- 📱 **Responsive** - Works perfectly on desktop, tablet, and mobile
- ⚡ **Fast & Lightweight** - No dependencies, instant load times
- 🧹 **Bulk Actions** - Clear all completed tasks with one click

## 🚀 Getting Started

### Option 1: Direct Use
Simply open `index.html` in your web browser - no installation required!

### Option 2: Local Server
```bash
# Using Python
python -m http.server 8000

# Using Node.js (with http-server installed)
npx http-server

# Using PHP
php -S localhost:8000
```

Then navigate to `http://localhost:8000` in your browser.

## 📖 How to Use

1. **Add a Task**
   - Type your task in the input field
   - Click the "Add" button or press Enter

2. **Complete a Task**
   - Click the circle checkbox next to any task
   - The task will be marked with a green checkmark and strikethrough

3. **Delete a Task**
   - Hover over a task to reveal the delete button
   - Click the trash icon to remove the task

4. **Filter Tasks**
   - Click "All" to see all tasks
   - Click "Active" to see only incomplete tasks
   - Click "Completed" to see only finished tasks

5. **Clear Completed**
   - Click "Clear Completed" in the footer to remove all finished tasks

## 🛠️ Technical Details

### Technologies Used
| Technology | Purpose |
|------------|---------|
| HTML5 | Structure and semantics |
| Tailwind CSS (v4) | Styling and responsive design |
| Vanilla JavaScript | Interactivity and logic |
| localStorage API | Data persistence |

### Project Structure
```
task-manager/
├── index.html    # Main application file (single-page app)
└── README.md     # Documentation
```

### Data Storage
Tasks are stored in the browser's localStorage with the following structure:
```javascript
{
  id: 1234567890,        // Unique timestamp ID
  text: "Task content",   // Task description
  completed: false,       // Completion status
  createdAt: "ISO date"   // Creation timestamp
}
```

## 🎨 Customization

### Changing Colors
The app uses Tailwind CSS classes. To change the color scheme, modify these classes in `index.html`:

- **Primary gradient**: `from-indigo-500 to-purple-600`
- **Accent color**: `text-indigo-600`, `border-indigo-600`
- **Completed state**: `bg-green-500`, `bg-green-50`

### Adding Features
The codebase is modular and easy to extend. Key functions:

| Function | Description |
|----------|-------------|
| `toggleTask(id)` | Toggle task completion |
| `deleteTask(id)` | Remove a task |
| `setFilter(filter)` | Change view filter |
| `clearCompleted()` | Remove all completed tasks |
| `renderTasks()` | Update the UI |
| `saveTasks()` | Persist to localStorage |

## 📱 Browser Support

| Browser | Supported |
|---------|-----------|
| Chrome | ✅ |
| Firefox | ✅ |
| Safari | ✅ |
| Edge | ✅ |
| Opera | ✅ |

## 📄 License

This project is open source and available under the [MIT License](https://opensource.org/licenses/MIT).

## 🤝 Contributing

Contributions are welcome! Feel free to:
- Report bugs
- Suggest new features
- Submit pull requests

---

<p align="center">
  Made with ❤️ for productivity enthusiasts
</p>
