
# CO3 - React Exercise - Export and Import

### NAME : Sukhmeet Kaur G
### REG NO : 2305001032

## Project Description
To implement a React application demonstrating the use of Export and Import concepts using JavaScript ES6 modules.

## Technologies Used
- React JS
- JavaScript (ES6)
- HTML
- CSS
- Vite

## Concepts
- JavaScript Modules
- Named Export
- Named Import
- Default Export
- Importing Variables
- Importing Functions
- React Components

## Project Structure
- `App.jsx` – Displays student details and imported function output.
- `App.css` – Contains the styling and layout of the application.
- `index.css` – Contains global styling.
- `main.jsx` – Entry point of the React application.
- `student.js` – Exports student details and a function.

## Source Code

### 1. student.js
```javascript

export const studentName = "Sukhmeet Kaur";

export const department = "Computer Science and Engineering";

export const college = "NMV University";

export function displayStudent() {
    return `Hello! I am ${studentName}, studying ${department} at ${college}.`;
}

```

### 2. App.jsx
```jsx

import React from "react";
import { studentName, department, college, displayStudent } from "./student.js";
import "./App.css";

function App() {
    return (
        <div className="container">
            <h1>React Export and Import</h1>

            <div className="card">
                <h2>Student Details</h2>
                <p><strong>Name:</strong> {studentName}</p>
                <p><strong>Department:</strong> {department}</p>
                <p><strong>College:</strong> {college}</p>

                <h3>Imported Function Output</h3>
                <p>{displayStudent()}</p>
            </div>
        </div>
    );
}

export default App;

```

### 3. App.css
```css

.container {
    text-align: center;
    padding: 50px 20px;
}

h1 {
    color: #2457a6;
}

.card {
    background: #f0f5ff;
    padding: 30px;
    max-width: 550px;
    margin: 30px auto;
    border-radius: 12px;
    box-shadow: 0 4px 12px rgba(0,0,0,0.1);
}

h2 {
    color: #2457a6;
}

h3 {
    color: #16804a;
}

p {
    font-size: 17px;
    line-height: 1.6;
}

```

### 4. index.css
```css

body {
    margin: 0;
    font-family: Arial, sans-serif;
    background-color: #ffffff;
    color: #333;
}

```

### 5. main.jsx
```jsx

import React from "react";
import ReactDOM from "react-dom/client";
import App from "./App.jsx";
import "./index.css";

ReactDOM.createRoot(document.getElementById("root")).render(
    <React.StrictMode>
        <App />
    </React.StrictMode>
);

```
## Author
Sukhmeet Kaur G

## Purpose
Created as part of the skill assessment.

## Output Screenshot
The application displays student information and a message generated using an imported function.
<img width="1600" height="709" alt="WhatsApp Image 2026-11-12 at 7 36 11 PM" src="https://github.com/user-attachments/assets/631d2624-10cb-4c36-8fea-5ede2daf46cd" />

