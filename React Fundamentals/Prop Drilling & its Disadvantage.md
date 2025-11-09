# 🔗 Prop Drilling in React

**Prop Drilling** happens when you pass data through **multiple nested components**,  
just to reach a deeply nested child component that actually needs it.

---

## 🧩 **In short:**
You send props from **Parent ➜ Child ➜ Grandchild ➜ ...**,  
even if some components in the chain **don’t use the data**.

---

## 🧠 **Example:**
```jsx
function App() {
  const user = "Nandha";
  return <Parent user={user} />;
}

function Parent({ user }) {
  return <Child user={user} />;
}

function Child({ user }) {
  return <GrandChild user={user} />;
}

function GrandChild({ user }) {
  return <h3>Hello, {user}!</h3>;
}

Output:
👉 Hello, Nandha
```
## ⚠️ Disadvantages of Prop Drilling:

❌ Hard to manage when components get deeply nested

❌ Causes unnecessary re-renders

❌ Makes the code less readable and maintainable

❌ Difficult to add or remove components in the middle

## 💡 Tip:

To avoid prop drilling, use:

React Context API

State Management Libraries like Redux or Zustand