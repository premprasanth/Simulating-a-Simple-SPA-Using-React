# React Lab Exercise 12(A): Simulating a Simple SPA Using React

## Name: PREM PRASANTH J
## Roll no: 2305001028
## Department: CSE

## AIM

To create a simple Single Page Application (SPA) using React in which users can navigate between Home, About, Contact, Courses, and Student pages without reloading the entire webpage.

## PROGRAM

### i) Home.jsx
```jsx
function Home() {
  return (
    <div>
      <h2>Home Page</h2>
      <p>Welcome to our React SPA!</p>
    </div>
  );
}

export default Home;
```

### ii) about.jsx
```jsx
function About() {
  return (
    <div>
      <h2>About Page</h2>
      <p>This is a simple Single Page Application.</p>
    </div>
  );
}

export default About;
```

### iii) Contact.jsx
```jsx
function Contact() {
  return (
    <div>
      <h2>Contact Page</h2>
      <p>Email: student@example.com</p>
    </div>
  );
}

export default Contact;
```

### iv) App.jsx
```jsx
import { useState } from "react";
import Home from "./Home";
import About from "./About";
import Contact from "./Contact";
import Courses from "./Courses";
import Student from "./Student";
import "./index.css";

function App() {
  const [page, setPage] = useState("home");

  return (
    <div className="app">
      <h1>Simple React SPA</h1>

      <nav>
        <button onClick={() => setPage("home")}>Home</button>
        <button onClick={() => setPage("about")}>About</button>
        <button onClick={() => setPage("contact")}>Contact</button>
        <button onClick={() => setPage("courses")}>Courses</button>
        <button onClick={() => setPage("student")}>Student</button>
      </nav>

      <hr />

      {page === "home" && <Home />}
      {page === "about" && <About />}
      {page === "contact" && <Contact />}
      {page === "courses" && <Courses />}
      {page === "student" && <Student />}
    </div>
  );
}

export default App;
```

## OUTPUT
<img width="1125" height="399" alt="image" src="https://github.com/user-attachments/assets/68787147-a720-481c-8753-9453f4357d27" />
<img width="1125" height="378" alt="image" src="https://github.com/user-attachments/assets/f09a82eb-0c43-4708-bb33-088a82ffbba6" />
<img width="1125" height="396" alt="image" src="https://github.com/user-attachments/assets/da8af465-0583-4ddc-ae1f-587721b3dfec" />

## RESULT

Thus, a simple Single Page Application was created successfully using React. The application allows users to navigate between Home, About, Contact, Courses, and Student pages dynamically without reloading the entire webpage.
