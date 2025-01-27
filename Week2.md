
# Week 2 (Html,CSS,RectBasics)  

## Day 1
### Html

```html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Basic HTML Structure</title>
</head>
<body>

    <header>
        <div>
            <h1>My Website</h1>
        </div>
        <nav>
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#services">Services</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <main>
        <section id="home">
            <h2>Home Section</h2>
            <p>Welcome to the home section of the website. We introduce the website here.</p>
        </section>

        <section id="about">
            <h2>About Section</h2>
            <p>Information about the website or company is provided here.</p>
            <article>
                <h3>Article Title</h3>
                <p>This is an article within the about section.</p>
            </article>
        </section>

        <section id="services">
            <h2>Our Services</h2>
            <div>
                <h3>Service 1</h3>
                <p>Description of the first service offered.</p>
            </div>
            <div>
                <h3>Service 2</h3>
                <p>Description of the second service offered.</p>
            </div>
            <div>
                <h3>Service 3</h3>
                <p>Description of the third service offered.</p>
            </div>
        </section>

        <section id="contact">
            <h2>Contact Section</h2>
            <p>Feel free to contact us using the form below.</p>
            <form>
                <label for="name">Name:</label>
                <input type="text" id="name" name="name" required><br><br>

                <label for="email">Email:</label>
                <input type="email" id="email" name="email" required><br><br>

                <textarea id="message" name="message" rows="4" placeholder="Your message..." required></textarea><br><br>

                <button type="submit">Submit</button>
            </form>
        </section>
    </main>

    <footer>
        <p>&copy; 2025 My Website. All Rights Reserved.</p>
        <address>
            Contact us at: <a href="mailto:contact@example.com">contact@example.com</a>
        </address>
    </footer>

</body>
</html>

```



## Day 2  

### HTML Code  

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Updated Semantic HTML and CSS Example</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>

    <header class="header">
        <div class="logo">
            <h1>My Website</h1>
        </div>
        <nav class="navigation">
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#services">Services</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <main>
        <section id="home" class="home">
            <h2>Home Section</h2>
            <p>Welcome to the home section of the website. We introduce the website here.</p>
        </section>

        <section id="about" class="about">
            <h2>About Section</h2>
            <p>Information about the website or company is provided here.</p>
            <article class="article">
                <h3>Article Title</h3>
                <p>This is an article within the about section.</p>
            </article>
        </section>

        <section id="services" class="services">
            <h2>Our Services</h2>
            <div class="service-item">
                <h3>Service 1</h3>
                <p>Description of the first service offered.</p>
            </div>
            <div class="service-item">
                <h3>Service 2</h3>
                <p>Description of the second service offered.</p>
            </div>
            <div class="service-item">
                <h3>Service 3</h3>
                <p>Description of the third service offered.</p>
            </div>
        </section>

        <section id="contact" class="contact">
            <h2>Contact Section</h2>
            <p>Feel free to contact us using the form below.</p>
            <form class="contact-form">
                <label for="name">Name:</label>
                <input type="text" id="name" name="name" required><br><br>

                <label for="email">Email:</label>
                <input type="email" id="email" name="email" required><br><br>

                <textarea id="message" name="message" rows="4" placeholder="Your message..." required></textarea><br><br>

                <button type="submit">Submit</button>
            </form>
        </section>
    </main>

    <footer class="footer">
        <p>&copy; 2025 My Website. All Rights Reserved.</p>
        <address>
            Contact us at: <a href="mailto:contact@example.com">contact@example.com</a>
        </address>
    </footer>

</body>
</html>
```

### CSS Code  

```css
/* Basic Reset */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: Arial, sans-serif;
    background-color: #f4f4f4;
    color: #333;
}

/* Header */
.header {
    background-color: #333;
    color: #fff;
    padding: 10px 20px;
    text-align: center;
}

.header h1 {
    font-size: 1.8rem;
}

/* Navigation */
.navigation ul {
    list-style: none;
    text-align: center;
    margin-top: 10px;
}

.navigation ul li {
    display: inline;
    margin: 0 10px;
}

.navigation ul li a {
    text-decoration: none;
    color: #fff;
    font-size: 1rem;
}

.navigation ul li a:hover {
    color: #ccc;
}

/* Main Content */
main {
    padding: 20px;
}

h2 {
    font-size: 1.5rem;
    color: #333;
    margin-bottom: 10px;
}

h3 {
    font-size: 1.2rem;
    margin-bottom: 5px;
}

/* Sections */
section {
    margin-bottom: 20px;
    background-color: #fff;
    padding: 10px;
    border: 1px solid #ddd;
    border-radius: 5px;
}

/* Contact Form */
.contact-form input,
.contact-form textarea,
.contact-form button {
    display: block;
    width: 100%;
    padding: 8px;
    margin-bottom: 10px;
    border: 1px solid #ddd;
    border-radius: 5px;
}

.contact-form button {
    background-color: #333;
    color: #fff;
    cursor: pointer;
}

.contact-form button:hover {
    background-color: #444;
}

/* Footer */
.footer {
    background-color: #333;
    color: #fff;
    text-align: center;
    padding: 10px;
}
```

---

## Day 3  

```css
/* Day 2: Advanced Styling */

/* Header - Add more padding and improve text alignment */
.header {
    background-color: #333;
    color: #fff;
    padding: 15px 25px; /* Updated padding */
    text-align: left; /* Updated text alignment */
}

/* Navigation - Improved spacing and hover effects */
.navigation ul li {
    display: inline-block; /* Changed to inline-block */
    margin: 0 15px; /* Updated spacing */
}

.navigation ul li a:hover {
    color: #aaa; /* Subtle hover effect */
    border-bottom: 2px solid #aaa; /* Added underline effect */
}

/* Main Content */
main {
    padding: 30px; /* Added more padding */
    background-color: #fff; /* Better sectioning */
}

/* Home Section - Added border for definition */
.home {
    border: 1px solid #ccc;
    padding: 15px; /* Day 2 padding update */
    border-radius: 8px; /* Rounded corners */
}

/* About Section - Updated styling */
.about {
    background-color: #f9f9f9; /* Light background for distinction */
    padding: 20px; /* Day 2 padding */
    border: 1px solid #ddd;
    border-radius: 8px;
}

/* Contact Form - Improved hover and transition effect */
.contact-form button:hover {
    background-color: #555;
    transition: background-color 0.3s ease; /* Smooth hover effect */
}

/* Footer - Added borders and padding for better style */
.footer {
    background-color: #222;
    color: #ccc;
    border-top: 1px solid #444; /* Border for footer */
    padding: 15px;
    font-size: 0.9rem; /* Slightly smaller font */
}
```

Here is the updated **React 2-day Basics** schedule, formatted in **Markdown** with detailed code examples.

---

## **Day 4: React Basics**

### **1. React Components:**

#### **Functional Component:**
```jsx
import React from 'react';

const MyComponent = () => {
  return <h1>Hello, React!</h1>;
};

export default MyComponent;
```

#### **Class Component:**
```jsx
import React, { Component } from 'react';

class MyComponent extends Component {
  render() {
    return <h1>Hello, React!</h1>;
  }
}

export default MyComponent;
```

### **2. JSX Syntax:**
JSX allows you to write HTML inside JavaScript.
```jsx
const MyComponent = () => {
  return (
    <div>
      <h1>Hello, React!</h1>
      <p>This is JSX syntax.</p>
    </div>
  );
};
```

### **3. Styling in React:**

#### **Inline Styling:**
Inline styles are provided as an object, with keys written in camelCase.
```jsx
const MyComponent = () => {
  const divStyle = {
    backgroundColor: 'blue',
    color: 'white',
    padding: '10px',
  };
  return <div style={divStyle}>Hello with inline styling!</div>;
};
```

#### **External CSS:**
You can import and use external CSS files.
```jsx
// App.js
import './App.css';

const MyComponent = () => {
  return <div className="my-class">Hello with external CSS!</div>;
};

export default MyComponent;

// App.css
.my-class {
  background-color: green;
  color: white;
  padding: 10px;
}
```

---

## **Day 5: React Basics - Conditional Rendering, Props, and Event Handling**

### **4. Props (Passing Data to Components):**
Props are used to pass data from a parent component to a child component.
```jsx
const Greeting = (props) => {
  return <h1>Hello, {props.name}!</h1>;
};

const App = () => {
  return <Greeting name="Alice" />;
};
```

### **5. Conditional Rendering:**
You can conditionally render elements using JavaScript expressions.
```jsx
const UserGreeting = ({ isLoggedIn }) => {
  return isLoggedIn ? <h1>Welcome Back!</h1> : <h1>Please log in.</h1>;
};
```

### **6. Event Handling:**
React uses camelCase for event names like `onClick`, `onChange`, etc.
```jsx
const Button = () => {
  const handleClick = () => {
    alert('Button clicked!');
  };

  return <button onClick={handleClick}>Click Me</button>;
};
```

### **7. List Rendering:**
You can dynamically render a list of elements using the `.map()` function.
```jsx
const List = () => {
  const items = ['Item 1', 'Item 2', 'Item 3'];

  return (
    <ul>
      {items.map((item, index) => (
        <li key={index}>{item}</li>
      ))}
    </ul>
  );
};
```

---
## Day 6 (Project Based on React)
### **Task List App (Basic Example)**

#### **Folder Structure:**
```
src/
|-- App.js
|-- Task.js
|-- TaskList.js
|-- App.css
|-- index.js
```

#### **1. `App.js` (Main Component)**
```jsx
import React, { useState } from 'react';
import './App.css';
import TaskList from './TaskList';

const App = () => {
  const [task, setTask] = useState('');
  const [tasks, setTasks] = useState([]);

  const handleAddTask = () => {
    if (task) {
      setTasks([...tasks, { text: task, completed: false }]);
      setTask('');
    }
  };

  return (
    <div className="app">
      <h1>Task List App</h1>
      <input 
        type="text" 
        value={task} 
        onChange={(e) => setTask(e.target.value)} 
        placeholder="Enter a task"
      />
      <button onClick={handleAddTask}>Add Task</button>

      {/* Conditional Rendering: If no tasks, show a message */}
      {tasks.length === 0 ? <p>No tasks yet. Add one!</p> : <TaskList tasks={tasks} setTasks={setTasks} />}
    </div>
  );
};

export default App;
```

#### **2. `TaskList.js` (List of Tasks Component)**
```jsx
import React from 'react';
import Task from './Task';

const TaskList = ({ tasks, setTasks }) => {
  const toggleTaskCompletion = (index) => {
    const newTasks = [...tasks];
    newTasks[index].completed = !newTasks[index].completed;
    setTasks(newTasks);
  };

  return (
    <div className="task-list">
      <h2>Tasks:</h2>
      <ul>
        {tasks.map((task, index) => (
          <Task 
            key={index} 
            task={task} 
            index={index} 
            toggleCompletion={toggleTaskCompletion} 
          />
        ))}
      </ul>
    </div>
  );
};

export default TaskList;
```

#### **3. `Task.js` (Task Component)**
```jsx
import React from 'react';

const Task = ({ task, index, toggleCompletion }) => {
  return (
    <li 
      onClick={() => toggleCompletion(index)} 
      style={{ textDecoration: task.completed ? 'line-through' : 'none' }}
    >
      {task.text}
    </li>
  );
};

export default Task;
```

#### **4. `App.css` (Styling)**
```css
/* Basic App Styling */
.app {
  font-family: Arial, sans-serif;
  text-align: center;
  margin-top: 50px;
}

input {
  padding: 10px;
  font-size: 16px;
  margin-right: 10px;
}

button {
  padding: 10px;
  font-size: 16px;
  cursor: pointer;
}

.task-list {
  margin-top: 20px;
}

.task-list ul {
  list-style-type: none;
  padding: 0;
}

.task-list li {
  padding: 10px;
  background-color: #f1f1f1;
  margin: 5px 0;
  cursor: pointer;
}

.task-list li:hover {
  background-color: #ddd;
}
```

#### **5. `index.js` (Entry Point)**
```jsx
import React from 'react';
import ReactDOM from 'react-dom';
import './index.css';
import App from './App';

ReactDOM.render(
  <React.StrictMode>
    <App />
  </React.StrictMode>,
  document.getElementById('root')
);
```
