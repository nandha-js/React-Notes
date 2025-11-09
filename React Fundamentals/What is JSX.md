# ⚛️ What is JSX in React?

**JSX (JavaScript XML)** is a **syntax extension for JavaScript** that lets you **write HTML-like code inside JavaScript**.  
It makes creating React components easier and more readable.

---

## 🧩 **In short:**
JSX allows you to **combine HTML and JavaScript** in one file.  
It looks like HTML but is actually converted to JavaScript behind the scenes.

---

## 🧠 **Example:**
```jsx
const element = <h1>Hello, JSX!</h1>;


This JSX code is converted by React into:

const element = React.createElement("h1", null, "Hello, JSX!");

```
## 💡 Tip:

JSX must have one parent element.

You can use curly braces {} inside JSX to write JavaScript expressions.

## 🧩 Example:
const name = "Nandha";
return <h2>Hello, {name}!</h2>;
