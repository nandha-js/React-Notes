# 👨‍👦 Parent to Child Data Passing in React

In React, data is passed **from parent to child** using **props** (short for properties).  
This is the main way components **communicate** with each other.

---

## 🧩 **In short:**
The **parent component** sends data as an **attribute**,  
and the **child component** receives it using **props**.

---

## 🧠 **Example:**
```jsx
// Parent Component
function App() {
  const user = "Nandha";
  return <Child name={user} />;
}

// Child Component
function Child(props) {
  return <h2>Hello, {props.name}!</h2>;
}
Output:
👉 Hello, Nandha

```

## 💡 Tip:

Props allow data flow in one direction — from parent ➜ child.

You can pass strings, numbers, arrays, objects, or even functions as props.

## 🧩 Example:

function App() {
  const details = { name: "Nandha", age: 22 };
  return <Profile info={details} />;
}

function Profile({ info }) {
  return <p>{info.name} is {info.age} years old.</p>;
}
