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



# Day 02 - Colors & Text Styling

## Goal

Learn how to apply colors and style text to make web pages visually appealing and easier to read.

---

## Topics Covered

* Colors in CSS

  * Color Names
  * HEX Colors
  * RGB Colors
* Text Styling Properties

  * color
  * font-size
  * font-family
  * font-weight
  * text-align
  * text-transform
  * text-decoration
  * line-height

---

## Colors in CSS

CSS provides multiple ways to define colors.

### 1. Color Names

You can use predefined color names.

```css
h1 {
  color: blue;
}

p {
  color: red;
}
```

### 2. HEX Colors

HEX (Hexadecimal) colors start with `#` followed by six characters.

```css
h1 {
  color: #ff0000;
}

p {
  color: #0000ff;
}
```

Examples:

| Color | HEX Value |
| ----- | --------- |
| Red   | #ff0000   |
| Green | #00ff00   |
| Blue  | #0000ff   |
| Black | #000000   |
| White | #ffffff   |

### 3. RGB Colors

RGB stands for Red, Green, and Blue.

```css
h1 {
  color: rgb(255, 0, 0);
}

p {
  color: rgb(0, 0, 255);
}
```

Values range from `0` to `255`.

---

## Text Styling Properties

### color

Changes the text color.

```css
p {
  color: navy;
}
```

### font-size

Controls the size of text.

```css
p {
  font-size: 18px;
}
```

### font-family

Defines the font style.

```css
body {
  font-family: Arial, sans-serif;
}
```

### font-weight

Controls the thickness of text.

```css
h1 {
  font-weight: bold;
}
```

Common values:

* normal
* bold
* 100 - 900

### text-align

Aligns text horizontally.

```css
h1 {
  text-align: center;
}
```

Values:

* left
* center
* right
* justify

### text-transform

Changes the text case.

```css
h1 {
  text-transform: uppercase;
}
```

Values:

* uppercase
* lowercase
* capitalize

### text-decoration

Adds or removes text decoration.

```css
a {
  text-decoration: none;
}
```

Examples:

```css
text-decoration: underline;
text-decoration: line-through;
```

### line-height

Controls spacing between lines of text.

```css
p {
  line-height: 1.8;
}
```

---

## Practice Project: Simple Article Page

### HTML

```html
<h1>Learning CSS</h1>

<p>
CSS helps make websites attractive and user-friendly.
It controls colors, fonts, spacing, and layout.
</p>
```

### CSS

```css
body {
  font-family: Arial, sans-serif;
}

h1 {
  color: #3498db;
  text-align: center;
  text-transform: uppercase;
}

p {
  color: rgb(80, 80, 80);
  font-size: 18px;
  line-height: 1.8;
}
```

---

## Key Points

* CSS colors can be defined using Names, HEX, or RGB values.
* The `color` property changes text color.
* `font-size` controls text size.
* `font-family` changes the font style.
* `font-weight` controls text thickness.
* `text-align` manages text alignment.
* `text-transform` changes text case.
* `text-decoration` adds or removes decorations.
* `line-height` improves readability by adjusting line spacing.

📖 Day 02 Summary

Today I learned how to add colors and style text using CSS. I explored different color formats such as Color Names, HEX, and RGB. I also practiced important text properties like font-size, font-family, font-weight, text-align, text-transform, text-decoration, and line-height. Finally, I applied these concepts by creating a simple article page.