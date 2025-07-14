### training day 12:-

## 3. CSS Styling: Inline, Internal & External

### What is CSS?

CSS (Cascading Style Sheets) is used to style HTML elements. It controls layout, color, fonts, spacing, and more.

There are **three ways to apply CSS**:

### Inline CSS

* Applied directly to an HTML element using the `style` attribute.
* Best for quick, one-time styling.

```html
<p style="color: green; font-size: 18px;">This is styled text.</p>
```

###  Internal CSS

* Defined inside a `<style>` tag within the `<head>` of an HTML file.
* Useful for styling a single web page.

```html
<head>
  <style>
    body {
      background-color: #f0fff0;
      font-family: Arial;
    }
    h1 {
      color: darkgreen;
    }
  </style>
</head>
```

###  External CSS

* Written in a separate `.css` file.
* Linked to the HTML file using the `<link>` tag.
* Recommended for styling multiple pages consistently.

**HTML File:**

```html
<head>
  <link rel="stylesheet" href="styles.css">
</head>
```

**styles.css File:**

```css
body {
  background-color: #e6ffe6;
  font-family: Verdana;
}
h1 {
  color: seagreen;
  text-align: center;
}
```

---

###  Comparison Table

| Feature     | Inline CSS             | Internal CSS                 | External CSS               |
| ----------- | ---------------------- | ---------------------------- | -------------------------- |
| Location    | Inside HTML element    | Inside `<style>` in `<head>` | In separate `.css` file    |
| Scope       | One element only       | Whole single HTML page       | Multiple HTML files        |
| Reusability |  No                   | limited                   |  High                     |
| Use Case    | Quick fixes or testing | Small websites or one-pagers | Full websites / many pages |

---
