# HTML Question Paper – Set 3

## Complete Answers

**Total Marks:** 50
**Time:** 1.5 Hours

---

# Section A – MCQs

### 10 × 1 = 10 Marks

### Q1. Which tag is used to insert an image?

**Answer:** B. `<img>`

---

### Q2. Which formatting element indicates strong importance?

**Answer:** C. `<strong>`

---

### Q3. Which attribute is used to specify the destination of a hyperlink?

**Answer:** B. `href`

---

### Q4. Which tag represents a list item?

**Answer:** B. `<li>`

---

### Q5. What is the default display behavior of `<div>`?

**Answer:** B. Block

---

### Q6. Which element provides additional information related to the main content?

**Answer:** A. `<aside>`

---

### Q7. Which element is commonly used to display preformatted text?

**Answer:** B. `<pre>`

---

### Q8. Which entity represents a non-breaking space?

**Answer:** B. `&nbsp;`

---

### Q9. Which HTML element is used to create a form?

**Answer:** B. `<form>`

---

### Q10. Which element is used to define navigation links?

**Answer:** C. `<nav>`

---

# Section B – Theory Questions

### 5 × 3 = 15 Marks

## Q11. Explain the difference between `<b>`, `<strong>`, `<i>`, and `<em>`. When would you prefer semantic elements?

**Answer:**

* `<b>` makes text **bold** without giving it special importance.
* `<strong>` indicates that the text has **strong importance**.
* `<i>` displays text in **italic** style without necessarily giving it emphasis.
* `<em>` indicates **emphasized** text and usually displays it in italic.

### Example:

```html
<p><b>Bold Text</b></p>
<p><strong>Important Text</strong></p>
<p><i>Italic Text</i></p>
<p><em>Emphasized Text</em></p>
```

**Semantic elements** such as `<strong>` and `<em>` should be preferred when the meaning or importance of the text matters, because they provide meaningful information about the content.

---

## Q12. What is the difference between an ordered list and an unordered list? Explain how you can create a nested list.

**Answer:**

An **ordered list** uses `<ol>` and displays items in a specific order, usually with numbers.

An **unordered list** uses `<ul>` and displays items using bullet points.

### Ordered List:

```html
<ol>
    <li>HTML</li>
    <li>CSS</li>
    <li>JavaScript</li>
</ol>
```

### Unordered List:

```html
<ul>
    <li>HTML</li>
    <li>CSS</li>
    <li>JavaScript</li>
</ul>
```

### Nested List:

A nested list is created by placing one list inside an `<li>` element.

```html
<ul>
    <li>Frontend
        <ul>
            <li>HTML</li>
            <li>CSS</li>
            <li>JavaScript</li>
        </ul>
    </li>
    <li>Backend</li>
</ul>
```

---

## Q13. Explain inline and block elements. What happens when multiple block elements are placed one after another?

**Answer:**

### Block Elements

Block elements normally start on a **new line** and take up the available width.

Examples:

```html
<div>Block 1</div>
<p>Block 2</p>
```

### Inline Elements

Inline elements do **not normally start on a new line**. They occupy only the space required by their content.

Examples:

```html
<span>Text 1</span>
<a href="#">Link</a>
```

When multiple block elements are placed one after another, **each block element starts on a new line**, so they appear vertically one below another.

---

## Q14. Explain the purpose of the following semantic elements: `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<footer>`.

**Answer:**

* **`<header>`** – Represents introductory content or the header of a page or section.
* **`<nav>`** – Contains important navigation links.
* **`<main>`** – Contains the main content of the webpage.
* **`<section>`** – Represents a thematic section of content.
* **`<article>`** – Represents independent, self-contained content such as a blog post or news article.
* **`<footer>`** – Represents footer information such as copyright or contact information.

These elements make the HTML structure more meaningful and easier to understand.

---

## Q15. Explain the difference between GET and POST methods in HTML forms. Mention one use case for each.

**Answer:**

### GET

* Sends form data as part of the **URL**.
* Data can be visible in the browser address bar.
* Suitable for retrieving or searching information.

**Example use case:** Search form.

```html
<form method="get">
    <input type="text" name="search">
    <button type="submit">Search</button>
</form>
```

### POST

* Sends form data in the **HTTP request body**.
* Data is not normally displayed in the URL.
* Suitable for submitting or changing data.

**Example use case:** Registration or login form.

```html
<form method="post">
    <input type="text" name="username">
    <button type="submit">Submit</button>
</form>
```

---

# Section C – Coding Questions

### 25 Marks

## Q16. Personal Profile Page – 7 Marks

Create a personal profile webpage containing a profile image, name, introduction, skills using an unordered list, education using an ordered list, GitHub profile link, and at least four formatting elements.

### Answer:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Personal Profile</title>
</head>
<body>

    <h1>Personal Profile</h1>

    <!-- Profile Image -->
    <img src="profile.jpg" alt="Profile Picture" width="150" height="150">

    <!-- Name -->
    <h2>Angel Patel</h2>

    <!-- Short Introduction -->
    <p>
        Hello! My name is <strong>Angel Patel</strong>.
        I am a <em>web development student</em> interested in
        <b>HTML, CSS, and JavaScript</b>.
    </p>

    <!-- Skills -->
    <h3>Skills</h3>
    <ul>
        <li>HTML</li>
        <li>CSS</li>
        <li>JavaScript</li>
        <li>Python</li>
    </ul>

    <!-- Education -->
    <h3>Education</h3>
    <ol>
        <li>School Education</li>
        <li>Higher Secondary Education</li>
        <li>Web Development Course</li>
    </ol>

    <!-- GitHub Profile -->
    <h3>GitHub Profile</h3>
    <p>
        Visit my
        <a href="https://github.com/" target="_blank">GitHub Profile</a>.
    </p>

    <!-- Additional Formatting Elements -->
    <p>
        <mark>Web Developer</mark><br>
        <small>Learning new technologies</small><br>
        <del>Old Skill</del><br>
        <u>Continuous Learning</u>
    </p>

</body>
</html>
```

**Formatting elements used:** `<strong>`, `<em>`, `<b>`, `<mark>`, `<small>`, `<del>`, and `<u>`.

---

## Q17. Employee Table – 6 Marks

Create an employee table with Employee ID, Name, Department, Salary. Use `<caption>`, `<thead>`, `<tbody>`, `<tfoot>`, and an appropriate `colspan`.

### Answer:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Employee Table</title>
</head>
<body>

    <table border="1">
        <caption>Employee Details</caption>

        <thead>
            <tr>
                <th>Employee ID</th>
                <th>Name</th>
                <th>Department</th>
                <th>Salary</th>
            </tr>
        </thead>

        <tbody>
            <tr>
                <td>101</td>
                <td>Amit</td>
                <td>Development</td>
                <td>45000</td>
            </tr>

            <tr>
                <td>102</td>
                <td>Neha</td>
                <td>Design</td>
                <td>40000</td>
            </tr>

            <tr>
                <td>103</td>
                <td>Rahul</td>
                <td>Testing</td>
                <td>42000</td>
            </tr>
        </tbody>

        <tfoot>
            <tr>
                <th colspan="3">Total Salary</th>
                <th>127000</th>
            </tr>
        </tfoot>

    </table>

</body>
</html>
```

**Total Salary = 45000 + 40000 + 42000 = 127000**

---

## Q18. Contact Form – 6 Marks

Create a contact form containing Name, Email, Phone, Subject dropdown, Message textarea, preferred contact method using radio buttons, terms checkbox, and Submit button. Use `name`, `id`, `for`, `placeholder`, and `required`.

### Answer:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Contact Form</title>
</head>
<body>

    <h1>Contact Us</h1>

    <form action="#" method="post">

        <!-- Name -->
        <label for="name">Name:</label>
        <input
            type="text"
            id="name"
            name="name"
            placeholder="Enter your name"
            required
        >
        <br><br>

        <!-- Email -->
        <label for="email">Email:</label>
        <input
            type="email"
            id="email"
            name="email"
            placeholder="Enter your email"
            required
        >
        <br><br>

        <!-- Phone -->
        <label for="phone">Phone:</label>
        <input
            type="tel"
            id="phone"
            name="phone"
            placeholder="Enter your phone number"
            required
        >
        <br><br>

        <!-- Subject -->
        <label for="subject">Subject:</label>
        <select id="subject" name="subject" required>
            <option value="">Select Subject</option>
            <option value="general">General Inquiry</option>
            <option value="support">Support</option>
            <option value="feedback">Feedback</option>
        </select>
        <br><br>

        <!-- Message -->
        <label for="message">Message:</label><br>
        <textarea
            id="message"
            name="message"
            placeholder="Enter your message"
            rows="5"
            cols="30"
            required
        ></textarea>
        <br><br>

        <!-- Preferred Contact Method -->
        <p>Preferred Contact Method:</p>

        <input
            type="radio"
            id="contact_email"
            name="contact_method"
            value="email"
            required
        >
        <label for="contact_email">Email</label>

        <input
            type="radio"
            id="contact_phone"
            name="contact_method"
            value="phone"
        >
        <label for="contact_phone">Phone</label>

        <br><br>

        <!-- Terms Checkbox -->
        <input
            type="checkbox"
            id="terms"
            name="terms"
            required
        >
        <label for="terms">
            I accept the terms and conditions
        </label>

        <br><br>

        <!-- Submit Button -->
        <button type="submit">Submit</button>

    </form>

</body>
</html>
```

---

## Q19. Code and Entities – 3 Marks

Display the following as visible text without the browser interpreting the tags as HTML:

```text
<div class="container">
<p>Hello & Welcome</p>
</div>
```

Also display `© 2026`, `5 < 10`, `10 > 5`, and `A & B` using HTML entities where required.

### Answer:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Code and Entities</title>
</head>
<body>

    <h1>HTML Code and Entities</h1>

    <!-- Display HTML code as visible text -->
    <pre>
&lt;div class="container"&gt;
    &lt;p&gt;Hello &amp; Welcome&lt;/p&gt;
&lt;/div&gt;
    </pre>

    <p>&copy; 2026</p>

    <p>5 &lt; 10</p>

    <p>10 &gt; 5</p>

    <p>A &amp; B</p>

</body>
</html>
```

### Important HTML Entities:

| Character | HTML Entity |
| --------- | ----------- |
| `<`       | `&lt;`      |
| `>`       | `&gt;`      |
| `&`       | `&amp;`     |
| `©`       | `&copy;`    |

---

## Q20. Complete Semantic Layout – 3 Marks

Create a webpage for a College Website using semantic HTML. It must contain `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<aside>`, and `<footer>`.

### Answer:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>College Website</title>
</head>
<body>

    <!-- Header -->
    <header>
        <h1>ABC College</h1>
        <p>Welcome to ABC College</p>
    </header>

    <!-- Navigation -->
    <nav>
        <a href="#">Home</a> |
        <a href="#">About</a> |
        <a href="#">Courses</a> |
        <a href="#">Contact</a>
    </nav>

    <!-- Main Content -->
    <main>

        <!-- Section -->
        <section>
            <h2>About Our College</h2>
            <p>
                ABC College provides quality education
                and various academic programs.
            </p>
        </section>

        <!-- Article -->
        <article>
            <h2>Latest News</h2>
            <p>
                Admissions are now open for the new academic year.
            </p>
        </article>

        <!-- Aside -->
        <aside>
            <h3>Important Information</h3>
            <p>College timings: 9:00 AM to 4:00 PM</p>
        </aside>

    </main>

    <!-- Footer -->
    <footer>
        <p>&copy; 2026 ABC College. All Rights Reserved.</p>
    </footer>

</body>
</html>
```

---

# Quick Revision

| Question | Main Concept                      |
| -------- | --------------------------------- |
| Q1       | `<img>`                           |
| Q2       | `<strong>`                        |
| Q3       | `href`                            |
| Q4       | `<li>`                            |
| Q5       | `<div>` = Block                   |
| Q6       | `<aside>`                         |
| Q7       | `<pre>`                           |
| Q8       | `&nbsp;`                          |
| Q9       | `<form>`                          |
| Q10      | `<nav>`                           |
| Q11      | Formatting vs Semantic Elements   |
| Q12      | Ordered, Unordered & Nested Lists |
| Q13      | Inline vs Block Elements          |
| Q14      | Semantic Elements                 |
| Q15      | GET vs POST                       |
| Q16      | Personal Profile                  |
| Q17      | Employee Table                    |
| Q18      | Contact Form                      |
| Q19      | HTML Entities                     |
| Q20      | Semantic Layout                   |
