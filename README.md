

# 📘 Flutter Development Intern Task – Week 2

## 📱 Counter & To-Do App with Local Storage

---

## 📌 Overview

This project focuses on understanding **state management** and **persistent local storage** in Flutter.

During this week, two mini applications were developed:

1. Counter App (with persistent storage)
2. To-Do List App (with SharedPreferences)

The objective was to learn how to manage state using `setState()` and store data locally using `SharedPreferences`.

---

# 🔢 1️⃣ Counter App

## 🎯 Features

* Increment counter value
* Display updated count in UI
* Save counter value locally
* Restore saved value after app restart

## 🧠 Concepts Used

* StatefulWidget
* setState()
* Async / Await
* SharedPreferences
* initState() lifecycle method

## 💾 Persistence Logic

* Counter value is saved using:

  ```
  sp.setInt("counter", count);
  ```

* On app startup:

  ```
  sp.getInt("counter");
  ```

* The saved value is loaded inside `initState()`.

---

# 📝 2️⃣ To-Do List App

## 🎯 Features

* Add new tasks
* Display tasks using ListView
* Delete tasks
* Save tasks locally
* Restore tasks after restart

## 🧠 Concepts Used

* ListView.builder
* TextEditingController
* setState()
* SharedPreferences
* Data conversion (String formatting & splitting)

## 💾 Data Storage Approach

Tasks are stored as formatted strings:

```
Task Title|true
Task Title|false
```

Where:

* First part → Task title
* Second part → Completion status

On app start:

* Data is loaded
* String is split using `|`
* Lists are reconstructed

---

# 🛠 Technologies Used

* Flutter
* Dart
* SharedPreferences package

---

# 📂 Project Structure

```
lib/
 ├── counter.dart
 ├── todo_screen.dart
 └── main.dart
```

---

# ▶ How to Run

1. Clone repository:

```
git clone <your-repo-link>
```

2. Navigate to project:

```
cd project-name
```

3. Install dependencies:

```
flutter pub get
```

4. Run app:

```
flutter run
```

---

# 🧠 Learning Outcomes

* Understanding StatefulWidget rebuild mechanism
* Managing dynamic UI updates
* Working with asynchronous functions
* Implementing local persistent storage
* Understanding Flutter lifecycle (initState)

---

# 🌟 Future Improvements

* Add task editing feature
* Add dark mode
* Use structured data model instead of formatted strings
* Implement Provider for advanced state management
* Migrate to Firebase for cloud sync

---

# 👨‍💻 Author

**Syed Hasnat Ali**
Flutter Development Intern
BSCS – Virtual University of Pakistan

---

