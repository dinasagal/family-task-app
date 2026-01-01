# 👨‍👩‍👧 Family Task Manager

A **child‑friendly, role‑based task management web app** for families.

Parents can create, assign, complete, and delete tasks, while children can create and manage **only their own tasks**. The app is designed with a **soft & friendly UI** suitable for kids, and simple logic that’s easy to understand and extend.

---

## ✨ Features

### 👨 Parent abilities

* Add new tasks
* Assign tasks to any child
* View **all** family tasks
* Mark any task as done / restore
* Delete tasks
* Reset all app data

### 👧 Child abilities

* Add their own tasks
* View **only their own** tasks
* Mark their own tasks as done

### 🧠 General

* Role‑based UI & permissions
* Tasks stored in `localStorage`
* Login / logout support
* Session persistence (optional)
* Soft, calm, child‑friendly design

---

## 🛠 Tech Stack

* **HTML** – structure
* **CSS** – soft & friendly UI
* **Vanilla JavaScript** – app logic
* **localStorage** – data persistence
* **Service Worker** – PWA ready (optional)

No frameworks, no backend.

---

## 📂 Project Structure

```
├── index.html      # App structure
├── style.css       # Soft & friendly UI styles
├── app.js          # Application logic
├── manifest.json   # PWA configuration
├── sw.js           # Service Worker
└── README.md
```

---

## 🚀 How to Run

1. Clone or download the project
2. Serve it locally (required for Service Worker)

Example:

```bash
python -m http.server
```

3. Open in browser:

```
http://localhost:8000
```

---

## 🔐 Roles & Permissions

| Action          | Parent | Child        |
| --------------- | ------ | ------------ |
| Add tasks       | ✅      | ✅ (own only) |
| Assign tasks    | ✅      | ❌            |
| View all tasks  | ✅      | ❌            |
| View own tasks  | ✅      | ✅            |
| Mark tasks done | ✅      | ✅ (own only) |
| Delete tasks    | ✅      | ❌            |
| Reset app       | ✅      | ❌            |

Permissions are enforced **both in UI and logic**.

---

## 🧩 Data Model

### User

```js
{
  name: "Alice",
  role: "parent" | "child"
}
```

### Task

```js
{
  id: Number,
  title: String,
  content: String,
  category: String,
  color: String,
  due: String,
  assignedTo: String,
  createdBy: String,
  done: Boolean
}
```

---

## 🎨 UI Philosophy

This app uses a **Soft & Friendly** design approach:

* Calm pastel colors
* Rounded cards and buttons
* Clear spacing and readable text
* Minimal clutter

Suitable for children while still looking professional.

---

## 🔮 Possible Improvements

* ⭐ Reward points for completed tasks
* 👨‍👩‍👧 Multiple parents support
* 🔔 Due‑date reminders
* 🔐 Password‑based authentication
* ☁ Backend (Firebase / Supabase)

---

## 💼 Why this project matters

This project demonstrates:

* Role‑based access control
* Frontend state management
* Clean separation of logic and UI
* Real‑world app structure

Great as a **junior developer portfolio project**.

---

## 📄 License

Free to use for learning and personal projects.

