# ⚙️ HTML Attributes vs JSX Attributes — Key Differences

HTML and JSX look similar, but their **attributes** are slightly different.  
Since JSX is based on **JavaScript**, some attribute names and styles follow **JS naming rules**.

---

## 🧩 **In short:**
JSX attributes use **camelCase** and sometimes **different names** compared to HTML.

---

## 🧱 **HTML vs JSX Attribute Comparison Table**

| 🧠 Feature / Attribute | 🌐 HTML | ⚛️ JSX |
|-------------------------|---------|--------|
| **CSS Class** | `class` | `className` |
| **Inline Style** | `style="color: red;"` | `style={{ color: "red" }}` |
| **Event Handler** | `onclick="handleClick()"` | `onClick={handleClick}` |
| **Label “for” Attribute** | `for` | `htmlFor` |
| **Tab Index** | `tabindex` | `tabIndex` |
| **Checked / Disabled** | `checked="true"` | `checked={true}` |
| **Boolean Attributes** | Can omit value (`disabled`) | Must specify value or `{true}` |
| **Custom Attributes** | Any attribute | Must use `data-*` format (e.g. `data-id`) |

---

## 🧠 **Example:**
```html
<!-- HTML -->
<button class="btn" onclick="alert('Hi!')">Click Me</button>

// JSX
<button className="btn" onClick={() => alert("Hi!")}>Click Me</button>

```
## 💡 Tip:

JSX follows JavaScript naming conventions, not HTML’s.

Always use camelCase for event names and attributes in JSX.

Inline styles are written as objects, not strings.
