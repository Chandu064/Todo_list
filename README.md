HTML Structure:
External Libraries: Links to Bootstrap CSS, jQuery, Popper.js, Bootstrap JavaScript, and Font Awesome for styling and functionality.
Custom CSS: Linked stylesheet todoCSS.css for additional styling.
Body Content:
Container Structure: Utilizes Bootstrap grid system for layout.
Todo Input Section:
Provides an input field (<input>) for users to input tasks.
Includes an "Add" button (<button>) to add tasks.
Todo List Section:
Displays a heading for the list of tasks.
Contains an unordered list (<ul>) with the id todoItemsContainer to hold the tasks.
Each task item will be appended as list items (<li>).
Tasks include a checkbox to mark completion status, the task text, and a delete icon.
Save Button: A button (<button>) with the id saveTodoButton presumably to save tasks to local storage.
JavaScript Functionality:
Local Storage Management:
Defines a function getTodoListFromLocalStorage() to retrieve the todo list from local storage. If none exists, it returns an empty array.
Initializes todoList array with the retrieved todo list or an empty array.
Saves the todoList to local storage when the "Save" button is clicked.
Event Handlers:
addTodoButton.onclick: Triggers onAddTodo() function to add a new task.
inputElement.onclick: Triggers onTodoStatusChange() function to toggle task completion status.
deleteIcon.onclick: Triggers onDeleteTodo() function to delete a task.
Task Management Functions:
onAddTodo(): Adds a new task to the todo list.
onTodoStatusChange(): Toggles the completion status of a task.
onDeleteTodo(): Deletes a task from the todo list.
Initialization:
Loops through the existing todo list items and appends them to the HTML.
CSS Styling:
Applies custom styles to various elements for visual presentation and layout.
Defines styles for the todo list container, headings, input fields, buttons, checkboxes, labels, and delete icons.
Overall, this code creates a simple todo list application with the ability to add, mark as complete, and delete tasks, while also providing a mechanism to save tasks to local storage for persistence across sessions.
