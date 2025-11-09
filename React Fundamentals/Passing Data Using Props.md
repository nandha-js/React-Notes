# 📦 Passing Data Using Props in React

**Props (short for “properties”)** are used to **send data from one component to another**, usually **from parent to child**.

---

## 🧩 **In short:**
Props let you make components **reusable** by passing different data each time.

---

## 🧠 **Example:**
```jsx
// Parent Component
function App() {
  return <Welcome name="Nandha" />;
}

// Child Component
function Welcome(props) {
  return <h2>Hello, {props.name}!</h2>;
}

Output:
👉 Hello, Nandha

```

## 💡 Tip:

Props are read-only (you can’t modify them inside the child component).

Use destructuring to access props easily:

function Welcome({ name }) {
  return <h2>Hello, {name}!</h2>;
}
