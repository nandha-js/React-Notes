# 🔁 Child to Parent Data Passing in React

In React, data usually flows **from parent to child** using props.  
But to send data **from child to parent**, we use a **callback function**.

---

## 🧩 **In short:**
The **parent** passes a function to the **child** as a prop,  
and the **child** calls that function to send data back.

---

## 🧠 **Example:**
```jsx
// Parent Component
function App() {
  const handleData = (message) => {
    console.log("Received from child:", message);
  };

  return <Child sendData={handleData} />;
}

// Child Component
function Child({ sendData }) {
  return (
    <button onClick={() => sendData("Hello Parent!")}>
      Send Data to Parent
    </button>
  );
}

Output in Console:
👉 Received from child: Hello Parent!
```
## 💡 Tip:

This method is called “lifting state up.”

Useful when multiple components need to share or sync data.

You can pass not just text — but also objects, arrays, or form data to the pare