# 📝 Todo App

A simple and interactive **Todo Application** built with **HTML, CSS, and JavaScript**. Users can add tasks dynamically and delete individual tasks from the list.

This project demonstrates practical JavaScript concepts including **DOM manipulation, event handling, dynamic element creation, event bubbling, and event delegation**.

## 🚀 Live Demo

🔗 **[View Live Demo](https://venumadhav66.github.io/JavaScript_Mini_Project/)**

## 📌 Project Overview

The Todo App provides a simple interface for managing tasks directly in the browser.

Users can:

- Add new tasks
- View tasks in a dynamic list
- Delete individual tasks
- Interact with dynamically generated elements

The main purpose of this project was to gain hands-on experience with JavaScript and understand how it interacts with HTML elements through the DOM.

## ✨ Features

- ➕ **Add Tasks** — Enter a task and add it to the list.
- 🗑️ **Delete Tasks** — Remove individual tasks using the delete button.
- ⚡ **Dynamic DOM Manipulation** — Creates new list items and buttons dynamically.
- 🎯 **Event Handling** — Uses event listeners to respond to user interactions.
- 🔄 **Event Delegation** — Handles dynamically created delete buttons using the parent `<ul>` element.
- 🧹 **Input Reset** — Clears the input field after adding a task.

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| **HTML5** | Structures the application |
| **CSS3** | Styles the user interface |
| **JavaScript** | Implements application logic and interactivity |
| **DOM API** | Dynamically creates, updates, and removes elements |
| **Git & GitHub** | Version control and project hosting |

## 🧠 Key JavaScript Concepts

### DOM Selection

```javascript
let btn = document.querySelector("button");
let ul = document.querySelector("ul");
let inp = document.querySelector("input");
```

### Event Handling

```javascript
btn.addEventListener("click", function () {
    // Add task
});
```

### Dynamic Element Creation

```javascript
let item = document.createElement("li");
let delBtn = document.createElement("button");
```

### Event Delegation

Instead of adding separate event listeners to every delete button, the application listens for clicks on the parent `<ul>` element.

```javascript
ul.addEventListener("click", function(event) {
    if (event.target.nodeName == "BUTTON") {
        let listItem = event.target.parentElement;
        listItem.remove();
    }
});
```

### DOM Element Removal

```javascript
listItem.remove();
```

## 🔄 Application Flow

### Adding a Task

```text
Enter task
    ↓
Click "Add Task"
    ↓
Read input value
    ↓
Create <li>
    ↓
Create Delete button
    ↓
Append button to <li>
    ↓
Append <li> to <ul>
    ↓
Clear input
```

### Deleting a Task

```text
Click "Delete"
    ↓
<ul> receives the event
    ↓
Identify clicked button
    ↓
Get parent <li>
    ↓
Remove <li>
```

## 📂 Project Structure

```text
JavaScript_Mini_Project/
│
├── index.html
├── style.css
├── app.js
└── README.md
```

## ▶️ How to Run Locally

### Clone the Repository

```bash
git clone https://github.com/VeNumadhaV66/JavaScript_Mini_Project.git
```

### Navigate to the Project

```bash
cd JavaScript_Mini_Project
```

### Run the Application

Open `index.html` directly in your browser.

Alternatively, use **Visual Studio Code + Live Server**:

1. Open the project in VS Code.
2. Install the Live Server extension.
3. Right-click `index.html`.
4. Select **Open with Live Server**.

## 🖥️ Usage

### Add a Task

1. Enter a task in the input field.
2. Click **Add Task**.
3. The task appears in the Todo list.

### Delete a Task

Click the **Delete** button next to the task you want to remove.

## 🔮 Future Enhancements

- [ ] Mark tasks as completed
- [ ] Edit existing tasks
- [ ] Store tasks using `localStorage`
- [ ] Prevent empty tasks from being added
- [ ] Add task filtering
- [ ] Add task counter
- [ ] Improve responsive design
- [ ] Add dark mode

## 📚 What I Learned

Through this project, I gained practical experience with:

- DOM element selection and manipulation
- Dynamic HTML element creation
- JavaScript event listeners
- Event bubbling
- Event delegation
- Removing elements from the DOM
- Connecting HTML, CSS, and JavaScript
- Using Git and GitHub for version control
- Deploying a frontend application using GitHub Pages

## 👨‍💻 Author

**Talari Venumadhava**

🔗 **GitHub:** [VeNumadhaV66](https://github.com/VeNumadhaV66)

🔗 **LinkedIn:** [Talari Venumadhava](https://www.linkedin.com/in/talari-venu-madhava-66751b280)

## 📄 License

This project was created for **learning and educational purposes**.