# css-learning
My CSS learning journey from beginner to advanced with notes, examples, and projects.


# Day 1 - CSS Basics

## 🎯 Goal

Understand how CSS works and learn the different ways to apply styles to HTML elements.

---

# What is CSS?

**CSS (Cascading Style Sheets)** is used to style and design web pages.

It controls:

* Colors
* Fonts
* Spacing
* Layout
* Borders
* Animations
* Responsive design

Without CSS, web pages look plain and unstyled.

---

# Ways to Add CSS

## 1. Inline CSS

CSS is written directly inside an HTML element using the `style` attribute.

### Example

```html
<h1 style="color: blue;">Welcome</h1>
```

### Advantages

* Quick for testing small styles.

### Disadvantages

* Hard to manage in large projects.
* Repeats code.

---

## 2. Internal CSS

CSS is written inside the `<style>` tag within the HTML file.

### Example

```html
<!DOCTYPE html>
<html>
<head>
    <style>
        h1 {
            color: green;
        }
    </style>
</head>
<body>
    <h1>Hello World</h1>
</body>
</html>
```

### Advantages

* Useful for single-page websites.

### Disadvantages

* Not reusable across multiple pages.

---

## 3. External CSS

CSS is written in a separate `.css` file and linked to the HTML file.

### HTML File

```html
<link rel="stylesheet" href="style.css">
```

### CSS File

```css
h1 {
    color: red;
}
```

### Advantages

* Reusable across multiple pages.
* Easy to maintain.
* Best practice for real projects.

---

# CSS Syntax

CSS follows a simple structure:

```css
selector {
    property: value;
}
```

### Example

```css
h1 {
    color: blue;
}
```

### Breakdown

* `h1` → Selector
* `color` → Property
* `blue` → Value

---

# Selectors

Selectors are used to target HTML elements and apply styles.

---

## 1. Element Selector

Targets all elements of the same type.

### HTML

```html
<p>This is a paragraph.</p>
```

### CSS

```css
p {
    color: purple;
}
```

---

## 2. Class Selector

Targets elements with a specific class.

### HTML

```html
<p class="text">Hello CSS</p>
```

### CSS

```css
.text {
    color: green;
}
```

### Note

* Starts with a dot (`.`)
* Can be used on multiple elements

---

## 3. ID Selector

Targets a unique element using its ID.

### HTML

```html
<h1 id="title">Welcome</h1>
```

### CSS

```css
#title {
    color: red;
}
```

### Note

* Starts with a hash (`#`)
* Should be unique on a page

---

## 4. Universal Selector

Targets all elements on the page.

### CSS

```css
* {
    margin: 0;
    padding: 0;
}
```

### Common Use

Used for CSS resets and applying global styles.

---

# Practice

Create a simple webpage and style:

### Heading

```css
h1 {
    color: blue;
}
```

### Paragraph

```css
p {
    font-size: 18px;
}
```

### Button

```css
button {
    background-color: green;
    color: white;
    border: none;
}
```

---

# Key Takeaways

✅ CSS is used to style web pages.

✅ There are three ways to add CSS:

* Inline CSS
* Internal CSS
* External CSS

✅ CSS follows the syntax:

```css
selector {
    property: value;
}
```

✅ Selectors help target elements:

* Element Selector
* Class Selector
* ID Selector
* Universal Selector

✅ External CSS is the preferred method for real-world projects.

📌 Day 1 Summary
Learned the purpose of CSS.
Explored three ways to apply CSS: Inline, Internal, and External.
Understood CSS syntax (selector, property, value).
Learned basic selectors:
Element Selector
Class Selector
ID Selector
Universal Selector
Practiced styling headings, paragraphs, and buttons.