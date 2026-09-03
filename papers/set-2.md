# HTML Question Paper – Set 2

## Answers

**Total Marks:** 50
**Time:** 1.5 Hours

---

# Section A – MCQs

### Q1. Which attribute specifies the URL of an image?

**Answer:** **B. `src`**

---

### Q2. Which tag is used to create a list with bullet points?

**Answer:** **C. `<ul>`**

---

### Q3. Which element represents a table header cell?

**Answer:** **B. `<th>`**

---

### Q4. Which element is normally inline?

**Answer:** **D. `<span>`**

---

### Q5. What does the `target="_blank"` attribute do in a link?

**Answer:** **B. Opens the link in a new browsing context**

---

### Q6. Which element is used for a description list?

**Answer:** **A. `<dl>`**

---

### Q7. Which element is most appropriate for a standalone blog post?

**Answer:** **B. `<article>`**

---

### Q8. Which entity represents an ampersand?

**Answer:** **B. `&amp;`**

---

### Q9. Which form method appends submitted form data to the URL?

**Answer:** **C. GET**

---

### Q10. Which element is used to embed another HTML document?

**Answer:** **A. `<iframe>`**

---

# Section B – Theory Questions

## Q11. Explain the purpose of the following image attributes: `src`, `alt`, `width`, `height`.

**Answer:**

### 1. `src`

The `src` attribute specifies the **URL or path of the image** that should be displayed.

```html
<img src="image.jpg">
```

### 2. `alt`

The `alt` attribute provides **alternative text** for an image. It is useful when the image cannot be displayed and also improves accessibility.

```html
<img src="image.jpg" alt="Student Photo">
```

### 3. `width`

The `width` attribute specifies the **width of the image**.

```html
<img src="image.jpg" width="300">
```

### 4. `height`

The `height` attribute specifies the **height of the image**.

```html
<img src="image.jpg" height="200">
```

---

## Q12. Explain `<a href="">` in HTML.

**Answer:**

The `<a>` element is used to create a **hyperlink** in HTML.

The `href` attribute specifies the **destination URL** of the link.

**Example:**

```html
<a href="https://www.google.com">Visit Google</a>
```

Here:

* `<a>` creates the hyperlink.
* `href` specifies where the link should go.
* `Visit Google` is the clickable text.

---

## Q13. Explain `rowspan` and `colspan` with suitable examples.

**Answer:**

### `rowspan`

The `rowspan` attribute is used to make a table cell **span multiple rows**.

**Example:**

```html
<table border="1">
    <tr>
        <th rowspan="2">Student</th>
        <th>Subject</th>
    </tr>
    <tr>
        <td>HTML</td>
    </tr>
</table>
```

Here, `rowspan="2"` makes the **Student** cell cover two rows.

### `colspan`

The `colspan` attribute is used to make a table cell **span multiple columns**.

**Example:**

```html
<table border="1">
    <tr>
        <th colspan="2">Student Details</th>
    </tr>
    <tr>
        <td>Rahul</td>
        <td>HTML</td>
    </tr>
</table>
```

Here, `colspan="2"` makes the **Student Details** cell cover two columns.

---

## Q14. What are HTML entities? Why are they required? Give any four examples.

**Answer:**

HTML entities are special codes used to display **reserved characters or special symbols** in HTML.

They are required because some characters, such as `<` and `>`, have special meanings in HTML. Entities allow us to display these characters as normal text.

### Examples:

| Character | HTML Entity |
| --------- | ----------- |
| `<`       | `&lt;`      |
| `>`       | `&gt;`      |
| `&`       | `&amp;`     |
| `©`       | `&copy;`    |

**Example:**

```html
<p>&lt;h1&gt;Hello World&lt;/h1&gt;</p>
<p>&amp;</p>
<p>&copy;</p>
```

---

## Q15. Explain the following attributes: `action`, `method`, `placeholder`.

**Answer:**

### 1. `action`

The `action` attribute specifies **where the form data should be sent** after the form is submitted.

```html
<form action="submit.php">
```

### 2. `method`

The `method` attribute specifies **how the form data should be sent**.

Common methods are:

* `GET`
* `POST`

```html
<form action="submit.php" method="post">
```

### 3. `placeholder`

The `placeholder` attribute provides a **short hint** that describes the expected input.

```html
<input type="text" placeholder="Enter your name">
```

---

# Section C – Coding Questions

## Q16. Student Registration Form – 8 Marks

### Question

Create an HTML student registration form containing:

* Full Name
* Email
* Password
* Date of Birth
* Gender using radio buttons
* Course using a dropdown
* Skills using checkboxes
* Address using `<textarea>`
* Submit and Reset buttons
* Appropriate `<label>` elements

### Answer

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Student Registration Form</title>
</head>
<body>

    <h1>Student Registration Form</h1>

    <form action="#" method="post">

        <!-- Full Name -->
        <label for="fullname">Full Name:</label>
        <input type="text" id="fullname" name="fullname" 
               placeholder="Enter your full name" required>

        <br><br>

        <!-- Email -->
        <label for="email">Email:</label>
        <input type="email" id="email" name="email" 
               placeholder="Enter your email" required>

        <br><br>

        <!-- Password -->
        <label for="password">Password:</label>
        <input type="password" id="password" name="password" 
               placeholder="Enter your password" required>

        <br><br>

        <!-- Date of Birth -->
        <label for="dob">Date of Birth:</label>
        <input type="date" id="dob" name="dob">

        <br><br>

        <!-- Gender -->
        <label>Gender:</label>

        <input type="radio" id="male" name="gender" value="male">
        <label for="male">Male</label>

        <input type="radio" id="female" name="gender" value="female">
        <label for="female">Female</label>

        <input type="radio" id="other" name="gender" value="other">
        <label for="other">Other</label>

        <br><br>

        <!-- Course -->
        <label for="course">Course:</label>
        <select id="course" name="course">
            <option value="">Select Course</option>
            <option value="html">HTML</option>
            <option value="css">CSS</option>
            <option value="javascript">JavaScript</option>
            <option value="python">Python</option>
        </select>

        <br><br>

        <!-- Skills -->
        <label>Skills:</label>

        <input type="checkbox" id="html" name="skills" value="html">
        <label for="html">HTML</label>

        <input type="checkbox" id="css" name="skills" value="css">
        <label for="css">CSS</label>

        <input type="checkbox" id="javascript" name="skills" value="javascript">
        <label for="javascript">JavaScript</label>

        <input type="checkbox" id="python" name="skills" value="python">
        <label for="python">Python</label>

        <br><br>

        <!-- Address -->
        <label for="address">Address:</label>
        <br>
        <textarea id="address" name="address" 
                  rows="5" cols="40" 
                  placeholder="Enter your address"></textarea>

        <br><br>

        <!-- Buttons -->
        <input type="submit" value="Submit">
        <input type="reset" value="Reset">

    </form>

</body>
</html>
```

---

## Q17. Table with Rowspan and Colspan – 6 Marks

### Question

Create the following table:

| Day       | Morning    | Afternoon  |
| --------- | ---------- | ---------- |
| Monday    | HTML       | CSS        |
| Tuesday   | JavaScript | React      |
| Wednesday | HTML       | JavaScript |

Requirements:

* Use `<th>` for headings.
* Use border to make the border visible.
* Add a caption to the table.

### Answer

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Class Schedule</title>
</head>
<body>

    <h1>Class Schedule</h1>

    <table border="1">

        <caption>Weekly Class Schedule</caption>

        <tr>
            <th>Day</th>
            <th>Morning</th>
            <th>Afternoon</th>
        </tr>

        <tr>
            <td>Monday</td>
            <td>HTML</td>
            <td>CSS</td>
        </tr>

        <tr>
            <td>Tuesday</td>
            <td>JavaScript</td>
            <td>React</td>
        </tr>

        <tr>
            <td>Wednesday</td>
            <td>HTML</td>
            <td>JavaScript</td>
        </tr>

    </table>

</body>
</html>
```

---

## Q18. Iframe and Linking – 5 Marks

### Question

Create a webpage that:

* Contains a heading **"Useful Resources"**
* Contains three hyperlinks.
* Opens one link in a new tab.
* Embeds another webpage using an iframe.
* Sets the iframe width and height.

### Answer

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Useful Resources</title>
</head>
<body>

    <h1>Useful Resources</h1>

    <h2>Useful Links</h2>

    <ul>
        <li>
            <a href="https://www.google.com">
                Google
            </a>
        </li>

        <li>
            <a href="https://www.w3schools.com" target="_blank">
                W3Schools
            </a>
        </li>

        <li>
            <a href="https://developer.mozilla.org">
                MDN Web Docs
            </a>
        </li>
    </ul>

    <h2>Embedded Webpage</h2>

    <iframe 
        src="https://www.example.com"
        width="600"
        height="400">
    </iframe>

</body>
</html>
```

---

## Q19. Inline, Block and Formatting – 3 Marks

### Question

Create an HTML page demonstrating:

* Two block-level elements.
* Three inline elements.
* Three text-formatting elements.
* Add comments indicating block-level and inline elements.

### Answer

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HTML Elements</title>
</head>
<body>

    <h1>Block and Inline Elements</h1>

    <!-- Block-level elements -->
    <div>
        This is a block-level div element.
    </div>

    <p>
        This is a block-level paragraph element.
    </p>

    <!-- Inline elements -->
    <span>This is an inline span element.</span>

    <a href="#">This is an inline link.</a>

    <strong>This is an inline strong element.</strong>

    <h2>Text Formatting</h2>

    <!-- Text formatting elements -->
    <p><strong>Bold and important text</strong></p>

    <p><em>Emphasized text</em></p>

    <p><mark>Highlighted text</mark></p>

</body>
</html>
```

---

## Q20. Semantic Elements – 3 Marks

### Question

Create a webpage using the following semantic structure:

* Header
* Navigation
* Main
* Section
* Article
* Aside
* Footer

### Answer

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Semantic HTML</title>
</head>
<body>

    <!-- Header -->
    <header>
        <h1>My Website</h1>
        <p>Welcome to my website</p>
    </header>

    <!-- Navigation -->
    <nav>
        <a href="#">Home</a>
        <a href="#">About</a>
        <a href="#">Contact</a>
    </nav>

    <!-- Main Content -->
    <main>

        <!-- Section -->
        <section>
            <h2>HTML Section</h2>

            <!-- Article -->
            <article>
                <h3>What is HTML?</h3>
                <p>
                    HTML stands for HyperText Markup Language.
                    It is used to create the structure of webpages.
                </p>
            </article>

        </section>

        <!-- Aside -->
        <aside>
            <h3>Related Information</h3>
            <p>
                HTML is used with CSS and JavaScript
                to create modern webpages.
            </p>
        </aside>

    </main>

    <!-- Footer -->
    <footer>
        <p>Copyright &copy; 2026 My Website</p>
    </footer>

</body>
</html>
```

---

# End of Answers
