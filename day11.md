
## Training day :- 11

###  HTML Topics

#### 1.  HTML Forms and Input Types

#####  What is an HTML Form?

An HTML **form** is used to **collect user input** and send it to the server for processing.

```html
<form action="submit_form.php" method="post">
  <!-- Form elements go here -->
</form>
```

---

##### 🔤 Common Input Types

| Input Type | Purpose                        | Example                   |
| ---------- | ------------------------------ | ------------------------- |
| `text`     | Single-line text input         | `<input type="text">`     |
| `password` | Hidden input for passwords     | `<input type="password">` |
| `email`    | Validated email input          | `<input type="email">`    |
| `number`   | Numeric input                  | `<input type="number">`   |
| `radio`    | Choose one option from many    | `<input type="radio">`    |
| `checkbox` | Choose multiple options        | `<input type="checkbox">` |
| `submit`   | Submit the form                | `<input type="submit">`   |
| `reset`    | Reset all fields               | `<input type="reset">`    |
| `date`     | Select a date                  | `<input type="date">`     |
| `file`     | Upload a file                  | `<input type="file">`     |
| `hidden`   | Send hidden data with the form | `<input type="hidden">`   |

---

####  Example Form

```html
<form action="/submit" method="post">
  Name: <input type="text" name="name"><br>
  Email: <input type="email" name="email"><br>
  Password: <input type="password" name="password"><br>

  Gender:
  <input type="radio" name="gender" value="male"> Male
  <input type="radio" name="gender" value="female"> Female<br>

  Hobbies:
  <input type="checkbox" name="hobby" value="Reading"> Reading
  <input type="checkbox" name="hobby" value="Travel"> Travel<br>

  Upload File: <input type="file"><br>

  <input type="submit" value="Submit">
</form>
```

---

#### 2.  Semantic HTML

##### What is Semantic HTML?

Semantic HTML uses tags that **clearly describe the meaning** of the content inside them. It improves:

* Code readability
* Accessibility
* SEO (Search Engine Optimization)

---

####  Common Semantic Tags

| Tag         | Meaning/Purpose                           |
| ----------- | ----------------------------------------- |
| `<header>`  | Top section of a page (logo, title, menu) |
| `<footer>`  | Bottom section (copyright, contact)       |
| `<nav>`     | Contains navigation links                 |
| `<section>` | Thematic content section                  |
| `<article>` | Independent, self-contained content       |

---

