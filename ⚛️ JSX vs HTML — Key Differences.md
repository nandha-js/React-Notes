# ⚛️ JSX vs HTML — Key Differences

JSX (JavaScript XML) looks like HTML, but it’s actually **JavaScript syntax** used in **React** to describe the UI.  
Even though they look similar, JSX and HTML have some important differences.

---

## 🧩 **In short:**
- **HTML** is static and used in normal web pages.  
- **JSX** is dynamic and lets you write **JavaScript inside UI code**.

---

## 🧱 **JSX vs HTML Comparison Table**

| 🧠 Feature | 🌐 HTML | ⚛️ JSX |
|------------|---------|--------|
| **Definition** | Markup language for building web pages | JavaScript syntax extension used in React |
| **Syntax** | Pure HTML tags | HTML-like syntax mixed with JavaScript |
| **Dynamic Data** | Cannot directly use JS expressions | Supports JS expressions inside `{}` |
| **Class Attribute** | Uses `class` | Uses `className` |
| **Inline Styles** | Written as strings | Written as objects using camelCase |
| **Closing Tags** | Optional for some elements | Must close all tags (e.g., `<img />`) |
| **Error Handling** | Browser ignores minor issues | JSX throws compile-time errors |
| **Rendering** | Rendered directly by browser | Transpiled to JavaScript using Babel before rendering |

---

## 🧠 **Example: **
```html
<!-- HTML -->
<h1>Hello World</h1>

``` 
## // JSX
const name = "Nandha";
<h1>Hello, {name}!</h1>;

## 💡 Tip:

JSX is not HTML, but it helps React developers write UI in a more natural, HTML-like way.
Under the hood, JSX is converted to React.createElement() calls.