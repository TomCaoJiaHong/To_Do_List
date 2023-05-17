# Todo List React Webpage

This is a simple React project that allows you to create, manage, and track a list of todos. The app provides features such as adding new todos, marking todos as completed, and deleting todos.

## Getting Started

To run the Todo List React App locally on your machine, please follow these steps:

1. Make sure you have Node.js and npm (Node Package Manager) installed on your machine.

2. Clone the repository or download the source code files.

3. Open a terminal or command prompt and navigate to the project directory.

4. Run the following command to install the necessary dependencies: `npm install`

5. After the installation is complete, run the following command to start the development server: `npm start`

6. The application should now be running on http://localhost:5173. Open a web browser and visit this URL to access the Todo List app.

## Features
### Adding Todos
To add a new todo to the list, use the "NewTodoForm" component located at the top of the app. Enter a title for the todo in the input field and press the "Enter" key or click the "Add" button. The new todo will be added to the list.

### Toggling Todo Completion
Each todo in the list has a checkbox next to it. Clicking the checkbox will toggle the completion status of the todo. Completed todos will be visually distinguished from incomplete todos.

### Deleting Todos
To remove a todo from the list, click the "Delete" button next to the todo. The todo will be permanently removed from the list.

## Data Persistence
The webpage utilizes the browser's localStorage to store the todo items. Whenever there is a change in the todo list (adding, toggling, or deleting todos), the webpage updates the localStorage accordingly. This allows the app to persist the todos across page refreshes and browser sessions.

## Code Structure
The codebase is organized as follows:

`App.js`: This is the main component that serves as the entry point for the Todo List app. It manages the state of the todos and handles the functions for adding, toggling, and deleting todos. It also renders the "NewTodoForm" component and the "TodoList" component.

`NewTodoForm.js`: This component provides an input field and a button for adding new todos. It communicates with the App component by invoking the onSubmit function when a new todo is submitted.

`TodoList.js`: This component receives the list of todos as a prop and renders each todo item using the "TodoItem" component. It also handles the event callbacks for toggling and deleting todos.

`TodoItem.js`: This component represents an individual todo item. It renders the todo's title, checkbox, and delete button. It communicates with the TodoList component by invoking the respective event callbacks when the checkbox or delete button is clicked.

`main.jsx`: This file is responsible for rendering the root component of the application (App) to the DOM. It uses ReactDOM.createRoot to render the app inside the designated root element.

`styles.css`: This file contains the CSS styles for the Todo List app. It provides the visual styling for the components and layout of the webpage.

## Author
This project is created by [Jiahong Cao]. If you have any questions or feedback, feel free to contact me at [Jiahong.Cao@dal.ca].

## Tutorial
This project was built by following https://www.youtube.com/watch?v=Rh3tobg7hEo to Tutorial by WebDevSimplified.

The tutorial covers the basics of building a Todo List app with React and provides step-by-step instructions on creating the functionality. It can be a helpful resource for understanding the code and learning React concepts.