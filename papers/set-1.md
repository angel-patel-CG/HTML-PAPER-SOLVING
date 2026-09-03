# HTML Question Paper – Set 1

## Answers

**Total Marks:** 50
**Time:** 1.5 Hours

---

# Section A – MCQs

### Q1. Which attribute is used to provide alternative text for an image?

**Answer:** **B. `alt`**

---

### Q2. Which HTML element is used to create a hyperlink?

**Answer:** **B. `<a>`**

---

### Q3. Which element is used to create a table row?

**Answer:** **C. `<tr>`**

---

### Q4. Which of the following is a block-level element?

**Answer:** **C. `<div>`**

---

### Q5. Which element is used to display another webpage inside the current webpage?

**Answer:** **B. `<iframe>`**

---

### Q6. Which tag is used to represent computer code?

**Answer:** **B. `<code>`**

---

### Q7. Which element represents the main content of a webpage?

**Answer:** **C. `<main>`**

---

### Q8. Which entity represents the `<` character?

**Answer:** **A. `&lt;`**

---

### Q9. Which attribute specifies where form data should be sent?

**Answer:** **B. `action`**

---

### Q10. Which tag creates an ordered list?

**Answer:** **C. `<ol>`**

---

# Section B – Theory Questions

## Q11. Explain the difference between `<strong>` and `<b>`. Also explain `<em>` and `<i>`.

**Answer:**

### `<strong>` vs `<b>`

* `<strong>` is used to indicate that the text has **strong importance** or significance.
* `<b>` is used to make text **bold** without giving it any special importance.

**Example:**

```html
<strong>Important Text</strong>
<b>Bold Text</b>
```

### `<em>` vs `<i>`

* `<em>` is used to give **emphasis** to text.
* `<i>` is generally used to display text in **italic style** without semantic emphasis.

**Example:**

```html
<em>Emphasized Text</em>
<i>Italic Text</i>
```

---

## Q12. What is the difference between ordered, unordered, and description lists? Give an example of each.

**Answer:**

There are three common types of lists in HTML:

### 1. Ordered List

An ordered list displays items in a specific order, usually using numbers.

```html
<ol>
    <li>HTML</li>
    <li>CSS</li>
    <li>JavaScript</li>
</ol>
```

### 2. Unordered List

An unordered list displays items using bullets.

```html
<ul>
    <li>HTML</li>
    <li>CSS</li>
    <li>JavaScript</li>
</ul>
```

### 3. Description List

A description list is used to display terms and their descriptions.

```html
<dl>
    <dt>HTML</dt>
    <dd>HyperText Markup Language</dd>
</dl>
```

---

## Q13. Explain the difference between inline and block-level elements with at least two examples of each.

**Answer:**

### Block-level Elements

Block-level elements normally start on a **new line** and take up the available width.

**Examples:**

* `<div>`
* `<p>`
* `<h1>`

**Example:**

```html
<div>This is a block element.</div>
<p>This is a paragraph.</p>
```

### Inline Elements

Inline elements do not normally start on a new line. They take only the space required by their content.

**Examples:**

* `<span>`
* `<a>`
* `<strong>`

**Example:**

```html
<span>This is inline.</span>
<a href="#">This is also inline.</a>
```

---

## Q14. What are semantic HTML elements? Explain any four semantic elements with their purpose.

**Answer:**

Semantic HTML elements clearly describe the **meaning and purpose of the content** to both browsers and developers.

### 1. `<header>`

Used for introductory content or the header of a webpage or section.

```html
<header>
    <h1>My Website</h1>
</header>
```

### 2. `<nav>`

Used to contain navigation links.

```html
<nav>
    <a href="home.html">Home</a>
    <a href="about.html">About</a>
</nav>
```

### 3. `<main>`

Represents the main content of the webpage.

```html
<main>
    <h2>Welcome</h2>
    <p>This is the main content.</p>
</main>
```

### 4. `<footer>`

Used for footer information such as copyright or contact information.

```html
<footer>
    <p>Copyright 2026</p>
</footer>
```

---

## Q15. What is an `<iframe>`?

**Answer:**

An `<iframe>` (inline frame) is an HTML element used to **embed another webpage or external content inside the current webpage**.

**Example:**

```html
<iframe src="https://example.com" width="600" height="400"></iframe>
```

The `src` attribute specifies the page or resource that should be displayed inside the iframe.

---

# Section C – Coding Questions

## Q16. Image and Linking – 5 Marks

### Question

Create an HTML page that contains:

* A heading **"My Favorite Website"**
* An image with appropriate `src` and `alt` attributes.
* A normal hyperlink to another page.

### Answer

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Favorite Website</title>
</head>
<body>

    <h1>My Favorite Website</h1>

    <img src="image.jpg" alt="My Favorite Website Image" width="300">

    <p>
        <a href="https://www.google.com">Visit My Favorite Website</a>
    </p>

</body>
</html>
```

---

## Q17. Tables – 7 Marks

### Question

Create the following table using HTML:

| Student | Subject    | Marks | Grade |
| ------- | ---------- | ----: | ----- |
| Rahul   | HTML       |    85 | A     |
| Priya   | CSS        |    92 | A+    |
| Aman    | JavaScript |    78 | B+    |
| Neha    | HTML       |    88 | A     |

### Answer

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Student Marks</title>
</head>
<body>

    <h1>Student Marks Table</h1>

    <table border="1">
        <tr>
            <th>Student</th>
            <th>Subject</th>
            <th>Marks</th>
            <th>Grade</th>
        </tr>

        <tr>
            <td>Rahul</td>
            <td>HTML</td>
            <td>85</td>
            <td>A</td>
        </tr>

        <tr>
            <td>Priya</td>
            <td>CSS</td>
            <td>92</td>
            <td>A+</td>
        </tr>

        <tr>
            <td>Aman</td>
            <td>JavaScript</td>
            <td>78</td>
            <td>B+</td>
        </tr>

        <tr>
            <td>Neha</td>
            <td>HTML</td>
            <td>88</td>
            <td>A</td>
        </tr>
    </table>

</body>
</html>
```

---

## Q18. Lists and Formatting – 5 Marks

### Question

Create a webpage containing:

1. An ordered list of 5 programming languages.
2. An unordered list of 5 HTML topics.
3. Use at least four formatting elements.

### Answer

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Lists and Formatting</title>
</head>
<body>

    <h1>Programming Languages</h1>

    <ol>
        <li>Python</li>
        <li>Java</li>
        <li>C++</li>
        <li>JavaScript</li>
        <li>C</li>
    </ol>

    <h1>HTML Topics</h1>

    <ul>
        <li>HTML Elements</li>
        <li>HTML Attributes</li>
        <li>HTML Forms</li>
        <li>HTML Tables</li>
        <li>HTML Lists</li>
    </ul>

    <h2>Formatting Elements</h2>

    <p><strong>This is important text.</strong></p>

    <p><em>This text is emphasized.</em></p>

    <p><mark>This text is highlighted.</mark></p>

    <p><del>This text is deleted.</del></p>

    <p>Water formula: H<sub>2</sub>O</p>

    <p>Square: 5<sup>2</sup></p>

</body>
</html>
```

---

## Q19. Computer Code and Entities – 4 Marks

### Question

Create a webpage that displays:

`<h1>Hello World</h1>`

as text rather than allowing the browser to interpret it as HTML.

Also display:

* `<`
* `>`
* `&`
* `©`

using appropriate HTML entities.

### Answer

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HTML Entities</title>
</head>
<body>

    <h1>Computer Code</h1>

    <p>
        &lt;h1&gt;Hello World&lt;/h1&gt;
    </p>

    <h2>HTML Entities</h2>

    <p>Less than: &lt;</p>
    <p>Greater than: &gt;</p>
    <p>Ampersand: &amp;</p>
    <p>Copyright: &copy;</p>

</body>
</html>
```

---

## Q20. Semantic Elements – 4 Marks

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

    <header>
        <h1>My Website</h1>
        <p>Welcome to my website</p>
    </header>

    <nav>
        <a href="#">Home</a>
        <a href="#">About</a>
        <a href="#">Contact</a>
    </nav>

    <main>

        <section>
            <h2>HTML Section</h2>

            <article>
                <h3>What is HTML?</h3>
                <p>
                    HTML stands for HyperText Markup Language.
                    It is used to create the structure of webpages.
                </p>
            </article>

        </section>

        <aside>
            <h3>Related Information</h3>
            <p>HTML is used together with CSS and JavaScript.</p>
        </aside>

    </main>

    <footer>
        <p>Copyright &copy; 2026 My Website</p>
    </footer>

</body>
</html>
```

---

# End of Answers
