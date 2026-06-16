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



# Day 3 - CSS Box Model

## 📌 Goal

Learn how spacing and sizing work in CSS using the Box Model.

---

# What is the CSS Box Model?

Every HTML element is treated as a rectangular box.

The box model consists of:

1. Content
2. Padding
3. Border
4. Margin

```text
+----------------------+
|       Margin         |
|  +----------------+  |
|  |    Border      |  |
|  | +------------+ |  |
|  | |  Padding   | |  |
|  | |  Content   | |  |
|  | +------------+ |  |
|  +----------------+  |
+----------------------+
```

---

# 1. Width

The `width` property defines the horizontal size of an element.

```css
.box {
    width: 300px;
}
```

### Example

```css
.card {
    width: 250px;
}
```

---

# 2. Height

The `height` property defines the vertical size of an element.

```css
.box {
    height: 150px;
}
```

### Example

```css
.card {
    height: 200px;
}
```

---

# 3. Border

The `border` property creates a boundary around an element.

### Syntax

```css
border: width style color;
```

### Example

```css
.card {
    border: 2px solid black;
}
```

Other border styles:

```css
border: 2px dashed red;
border: 2px dotted blue;
```

---

# 4. Padding

Padding is the space between the content and the border.

```css
.card {
    padding: 20px;
}
```

### Example

```css
.card {
    border: 2px solid black;
    padding: 15px;
}
```

Padding makes the content appear more spacious.

---

# 5. Margin

Margin is the space outside the border.

```css
.card {
    margin: 20px;
}
```

### Example

```css
.card {
    margin: 30px;
}
```

Margin creates distance between elements.

---

# 6. Box Sizing

The `box-sizing` property controls how width and height are calculated.

### Default: content-box

```css
.box {
    width: 300px;
    padding: 20px;
    border: 5px solid black;
}
```

Actual width becomes:

```text
300 + 20 + 20 + 5 + 5 = 350px
```

---

### border-box

```css
.box {
    box-sizing: border-box;
}
```

Now padding and border are included inside the specified width.

```css
.box {
    width: 300px;
    padding: 20px;
    border: 5px solid black;
    box-sizing: border-box;
}
```

Actual width remains:

```text
300px
```

### Best Practice

```css
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}
```

Many developers use this globally.

---

# Practice Task

## Create 3 Different Styled Cards

### Card 1

```css
.card1 {
    width: 250px;
    padding: 15px;
    border: 2px solid black;
    margin: 20px;
}
```

### Card 2

```css
.card2 {
    width: 300px;
    padding: 25px;
    border: 3px dashed blue;
    margin: 20px;
}
```

### Card 3

```css
.card3 {
    width: 280px;
    padding: 20px;
    border: 2px dotted green;
    margin: 20px;
    box-sizing: border-box;
}
```

---

# Key Points

* `width` controls horizontal size.
* `height` controls vertical size.
* `border` creates an outline around an element.
* `padding` adds space inside the border.
* `margin` adds space outside the border.
* `box-sizing: border-box` makes sizing easier and more predictable.

📖 Day 3 Summary

Today I learned the CSS Box Model, which controls the size and spacing of elements.

I studied:

Width
Height
Border
Padding
Margin
Box Sizing

I also practiced by creating 3 different styled cards using these properties.


# Day 4 - Backgrounds & Borders

## 📌 Goal

Learn how to improve the design and appearance of web pages using backgrounds and borders.

---

# What are Backgrounds?

Background properties are used to add colors and images behind an element.

They help make a webpage more attractive and visually appealing.

---

# 1. background-color

The `background-color` property sets a background color for an element.

### Syntax

```css
background-color: color;
```

### Example

```css
.box {
    background-color: lightblue;
}
```

You can use:

```css
background-color: red;
background-color: #3498db;
background-color: rgb(52, 152, 219);
```

---

# 2. background-image

The `background-image` property adds an image as the background.

### Syntax

```css
background-image: url("image.jpg");
```

### Example

```css
.hero {
    background-image: url("nature.jpg");
}
```

---

# 3. background-size

The `background-size` property controls the size of the background image.

### Example

```css
.hero {
    background-size: cover;
}
```

Common values:

```css
background-size: cover;
background-size: contain;
background-size: 100% 100%;
```

### cover

The image covers the entire element.

```css
background-size: cover;
```

---

# 4. background-position

The `background-position` property controls where the image appears.

### Example

```css
.hero {
    background-position: center;
}
```

Other values:

```css
background-position: top;
background-position: bottom;
background-position: left;
background-position: right;
background-position: center;
```

---

# 5. border-radius

The `border-radius` property creates rounded corners.

### Example

```css
.box {
    border-radius: 10px;
}
```

### Circle Example

```css
.profile-image {
    width: 150px;
    height: 150px;
    border-radius: 50%;
}
```

---

# 6. box-shadow

The `box-shadow` property adds shadow effects around elements.

### Syntax

```css
box-shadow: horizontal vertical blur color;
```

### Example

```css
.card {
    box-shadow: 0 4px 10px gray;
}
```

### Strong Shadow

```css
.card {
    box-shadow: 0 8px 20px rgba(0, 0, 0, 0.3);
}
```


# Key Points

* `background-color` adds color behind an element.
* `background-image` adds an image as the background.
* `background-size` controls image size.
* `background-position` controls image placement.
* `border-radius` creates rounded corners.
* `box-shadow` adds depth using shadows.
* These properties make websites look modern and attractive.

📖 Day 4 Summary

Today I learned how to improve webpage design using CSS backgrounds and border effects.

Topics covered:

Background Color
Background Image
Background Size
Background Position
Border Radius
Box Shadow

Practice completed:

Designed a Profile Card using rounded corners, shadows, and background styling.


# Day 5 - Display & Position

## 📌 Goal

Learn how to control the layout and positioning of elements on a webpage.

---

# What is Display?

The `display` property determines how an element appears and behaves in the layout.

Different display values affect how elements take up space and interact with other elements.

---

# 1. display: block

A block element:

* Takes the full available width.
* Starts on a new line.
* Can have width and height.

### Examples of Block Elements

```html
<div></div>
<p></p>
<h1></h1>
```

### Example

```css
.box {
    display: block;
}
```

---

# 2. display: inline

An inline element:

* Takes only the space it needs.
* Does not start on a new line.
* Width and height usually do not work.

### Examples of Inline Elements

```html
<span></span>
<a></a>
<strong></strong>
```

### Example

```css
span {
    display: inline;
}
```

---

# 3. display: inline-block

Combines features of inline and block.

* Stays on the same line.
* Allows width and height.

### Example

```css
.button {
    display: inline-block;
    width: 150px;
    height: 50px;
}
```

---

# 4. display: none

Completely hides an element.

### Example

```css
.hidden {
    display: none;
}
```

The element:

* Is not visible.
* Does not take space on the page.

---

# What is Position?

The `position` property controls where an element appears on the page.

---

# 5. position: static

Default position for all elements.

### Example

```css
.box {
    position: static;
}
```

Characteristics:

* Normal document flow.
* top, right, bottom, left do not work.

---

# 6. position: relative

Moves an element relative to its original position.

### Example

```css
.box {
    position: relative;
    top: 20px;
    left: 30px;
}
```

The original space remains reserved.

---

# 7. position: absolute

Positions an element relative to its nearest positioned parent.

### Example

```css
.parent {
    position: relative;
}

.child {
    position: absolute;
    top: 10px;
    right: 10px;
}
```

Characteristics:

* Removed from normal flow.
* Can overlap other elements.

---

# 8. position: fixed

The element stays fixed on the screen.

### Example

```css
.chat-button {
    position: fixed;
    bottom: 20px;
    right: 20px;
}
```

Characteristics:

* Remains visible while scrolling.
* Commonly used for floating buttons.

---

# 9. position: sticky

Acts like relative until a scroll point is reached.

Then it becomes fixed.

### Example

```css
.navbar {
    position: sticky;
    top: 0;
}
```

Commonly used for:

* Navigation bars
* Section headers

---

# 10. z-index

Controls which element appears on top.

Higher value = appears above lower values.

### Example

```css
.box1 {
    z-index: 1;
}

.box2 {
    z-index: 10;
}
```

`box2` will appear above `box1`.

### Important

`z-index` works on positioned elements.

```css
.box {
    position: relative;
    z-index: 5;
}
```


# Display Comparison

| Value        | New Line | Width/Height |
| ------------ | -------- | ------------ |
| block        | Yes      | Yes          |
| inline       | No       | No           |
| inline-block | No       | Yes          |
| none         | Hidden   | Hidden       |

---

# Position Comparison

| Value    | Description                   |
| -------- | ----------------------------- |
| static   | Default position              |
| relative | Moves from original position  |
| absolute | Relative to positioned parent |
| fixed    | Fixed to screen               |
| sticky   | Becomes fixed while scrolling |

---

# Key Points

* `display` controls how elements appear.
* `block` takes full width.
* `inline` stays in the same line.
* `inline-block` allows width and height.
* `none` completely hides elements.
* `position` controls element placement.
* `sticky` is commonly used for navbars.
* `z-index` controls stacking order.

📖 Day 5 Summary

Today I learned how to control webpage layouts using the display and position properties.

Topics Covered
display
block
inline
inline-block
none
position
static
relative
absolute
fixed
sticky
z-index

# 📅 Day 6: Flexbox

## 🎯 Goal

Learn how to create modern and responsive layouts using Flexbox.

---

# What is Flexbox?

Flexbox (Flexible Box Layout) is a CSS layout model that helps arrange items in rows or columns.

It makes it easier to:

* Align items
* Distribute space
* Create responsive layouts
* Build modern UI designs

To use Flexbox, set the container's display property to `flex`.

```css
.container {
    display: flex;
}
```

---

# 1. display: flex

Converts a normal container into a flex container.

```css
.container {
    display: flex;
}
```

### Example

```html
<div class="container">
    <div>Box 1</div>
    <div>Box 2</div>
    <div>Box 3</div>
</div>
```

```css
.container {
    display: flex;
}
```

### Output

Items appear in a row by default.

```
Box 1  Box 2  Box 3
```

---

# 2. flex-direction

Controls the direction of flex items.

### Row (Default)

```css
.container {
    display: flex;
    flex-direction: row;
}
```

```
Box 1  Box 2  Box 3
```

### Column

```css
.container {
    display: flex;
    flex-direction: column;
}
```

```
Box 1
Box 2
Box 3
```

### Other Values

```css
flex-direction: row-reverse;
flex-direction: column-reverse;
```

---

# 3. justify-content

Aligns items along the **main axis**.

### Center

```css
.container {
    display: flex;
    justify-content: center;
}
```

### Common Values

```css
justify-content: flex-start;
justify-content: flex-end;
justify-content: center;
justify-content: space-between;
justify-content: space-around;
justify-content: space-evenly;
```

### Example

```css
.container {
    display: flex;
    justify-content: space-between;
}
```

```
Box1          Box2          Box3
```

---

# 4. align-items

Aligns items along the **cross axis**.

```css
.container {
    display: flex;
    align-items: center;
}
```

### Common Values

```css
align-items: flex-start;
align-items: flex-end;
align-items: center;
align-items: stretch;
```

### Example

```css
.container {
    display: flex;
    height: 200px;
    align-items: center;
}
```

Items will be vertically centered inside the container.

---

# 5. flex-wrap

Controls whether items stay on one line or move to the next line.

### No Wrap (Default)

```css
.container {
    display: flex;
    flex-wrap: nowrap;
}
```

### Wrap

```css
.container {
    display: flex;
    flex-wrap: wrap;
}
```

When there isn't enough space, items move to the next line.

---

# 6. gap

Adds space between flex items.

```css
.container {
    display: flex;
    gap: 20px;
}
```

### Benefits

* Cleaner than using margins
* Easy spacing control
* Works for rows and columns

---

# Combining Flexbox Properties

```css
.container {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    align-items: center;
    gap: 20px;
}
```

This creates a flexible and responsive layout.

---

# Practice Project: Responsive Card Layout

## HTML

```html
<div class="cards">
    <div class="card">Card 1</div>
    <div class="card">Card 2</div>
    <div class="card">Card 3</div>
    <div class="card">Card 4</div>
</div>
```

## CSS

```css
.cards {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 20px;
}

.card {
    width: 200px;
    padding: 20px;
    border: 1px solid #ccc;
    border-radius: 10px;
}
```

### Result

* Cards appear in a row on larger screens.
* Cards automatically move to the next line on smaller screens.
* Layout becomes responsive with minimal code.

---

# Key Points to Remember

✅ Flexbox is used for one-dimensional layouts (row or column).

✅ `display: flex` activates Flexbox.

✅ `flex-direction` controls layout direction.

✅ `justify-content` aligns items on the main axis.

✅ `align-items` aligns items on the cross axis.

✅ `flex-wrap` allows items to move to the next line.

✅ `gap` creates spacing between items.

✅ Flexbox is widely used for modern responsive layouts.

📖 Day 6 Summary

Today I learned Flexbox, one of the most important CSS layout systems.

You covered:

display: flex
flex-direction
justify-content
align-items
flex-wrap
gap
