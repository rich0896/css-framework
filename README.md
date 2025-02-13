# Pastel CSS

Pastel CSS is a lightweight, customizable CSS framework designed to bring a soft, modern aesthetic to web design. Built with Sass for flexibility, it offers a pastel-inspired color palette, sleek UI components, and utility classes for effortless styling. 🌸🎨✨

## Table of Contents

1. [Introduction](#introduction)
2. [Getting Started](#getting-started)
3. [Font Imports & CSS Reset](#font-imports--css-reset)
4. [Colour Utility Classes](#colour-utility-classes)
5. [Spacing & Layout Utilities](#spacing--layout-utilities)
    - [Padding & Margin](#padding--margin)
    - [Opacity](#opacity-utilities)
    - [Border Radius](#border-radius-utilities)
    - [Display & Flex Utilities](#display--flex-utilities)
    - [Typography & Width Utilities](#typography--width-utilities)
6. [Component & Element Styles](#component--element-styles)
    - [Lists](#lists)
    - [Buttons](#buttons)
    - [Tables](#tables)
    - [Headings](#headings)
    - [Forms & Inputs](#forms-and-inputs)

## Introduction

This CSS framework provides a solid foundation to build modern, responsive, and visually consistent web interfaces. It offers:

- **Predefined fonts and a CSS reset:** Ensuring consistency across browsers.
- **Utility classes:** For colours, spacing, opacity, border radius, display, flex layout, typography, and sizing.
- **Component styles:** For common UI elements like lists, buttons, tables, headings, and forms.

The goal is to reduce repetitive CSS code and provide an easy starting point for customization.

## Getting Started

Include the compiled `pastel.css` CSS file in your HTML:

```html
<link rel="stylesheet" href="path/to/your/pastel.css">
```

You can now use the utility classes and element styles directly in your HTML.

## Font Imports & CSS Reset

At the very top of the file, the framework imports fonts and applies a comprehensive CSS reset.

### Fonts

Three Google Fonts are imported to provide a range of typography options:

- **Almarai:** Used for headings.
- **Gemunu Libre:** Used for buttons, labels and captions.
- **Fira Code:** Standard paragraph text.

### CSS Reset

[The new CSS reset](https://github.com/elad2412/the-new-css-reset) is applied to remove browser inconsistencies.

This:
- Removes browser-specific default styles.
- Provides a clean slate for custom styling.

## Colour Utility Classes

A robust set of utility classes for text and background colours is available. They are organized by colour groups and variants.

### Naming Conventions

Each colour group includes:

- **Base Colour:**
    - `.text-{color}` and `.bg-{color}`
    - `.text-hover-{color}:hover` for hover effects.
- **Light Variants:**
    - `.text-{color}-light-1` to `.text-{color}-light-9`
    - `.bg-{color}-light-1` to `.bg-{color}-light-9`
    - Hover variants follow the same naming.
- **Dark Variants:**
    - `.text-{color}-dark-1` to `.text-{color}-dark-9`
    - `.bg-{color}-dark-1` to `.bg-{color}-dark-9`
    - Hover variants are also provided.

### Example

```html
<p class="text-primary">This text is styled with the primary color.</p>
<div class="bg-secondary">This div has a secondary background.</div>
```


## Spacing & Layout Utilities

A suite of utility classes is provided for spacing, opacity, border radius, display properties, flex layout, typography, and width.

### Padding & Margin

#### Padding Classes

- **Uniform Padding:**
    
    - `.p-0` — `padding: 0;`
    - `.p-1` — `padding: 0.75rem;`
    - `.p-2` — `padding: 1.5rem;`
    - `.p-3` — `padding: 3rem;`
    - `.p-4` — `padding: 4.5rem;`
    - `.p-5` — `padding: 6rem;`
- **Side-Specific Padding:**
    
    - Left: `.pl-0` to `.pl-5`
    - Right: `.pr-0` to `.pr-5`
    - Top: `.pt-0` to `.pt-5`
    - Bottom: `.pb-0` to `.pb-5`

#### Margin Classes

- **Uniform Margin:**
    
    - `.m-0` — `margin: 0;`
    - `.m-1` — `margin: 0.75rem;`
    - `.m-2` — `margin: 1.5rem;`
    - `.m-3` — `margin: 3rem;`
    - `.m-4` — `margin: 4.5rem;`
    - `.m-5` — `margin: 6rem;`
- **Side-Specific Margin:**
    
    - Left: `.ml-0` to `.ml-5`
    - Right: `.mr-0` to `.mr-5`
    - Top: `.mt-0` to `.mt-5`
    - Bottom: `.mb-0` to `.mb-5`

_Usage Example:_

```html
<div class="p-2 m-3">This element has 1.5rem padding and 3rem margin.</div>
```

### Opacity Utilities

Adjust element transparency:

- `.o-10` — `opacity: 0.1;`
- `.o-20` — `opacity: 0.2;`
- … up to …
- `.o-100` — `opacity: 1;`

_Usage Example:_

```html
<img src="image.jpg" class="o-70" alt="Semi-transparent image">
```

### Border Radius Utilities

Control the rounding of element corners:

- `.br` — `border-radius: 20px;`
- `.br-none` — `border-radius: 0;`
- `.br-xs` — `border-radius: 5px;`
- `.br-sm` — `border-radius: 10px;`
- `.br-lg` — `border-radius: 40px;`
- `.br-full` — `border-radius: 50%;`

_Usage Example:_

```html
<div class="br-sm">Element with small rounded corners.</div>
```

### Display & Flex Utilities

#### Display Classes

- `.display-n` — `display: none;`
- `.display-b` — `display: block;`
- `.display-f` — `display: flex;`
- `.display-i` — `display: inline;`
- `.display-i-b` — `display: inline-block;`

#### Flex Direction

- `.fd-row` — `flex-direction: row;`
- `.fd-row-reverse` — `flex-direction: row-reverse;`
- `.fd-column` — `flex-direction: column;`
- `.fd-column-reverse` — `flex-direction: column-reverse;`

#### Flex Alignment

- **Justify Content:**
    - `.jc-start` — `justify-content: flex-start;`
    - `.jc-end` — `justify-content: flex-end;`
    - `.jc-center` — `justify-content: center;`
    - `.jc-between` — `justify-content: space-between;`
    - `.jc-around` — `justify-content: space-around;`
- **Align Items:**
    - `.ai-start` — `align-items: flex-start;`
    - `.ai-end` — `align-items: flex-end;`
    - `.ai-center` — `align-items: center;`
    - `.ai-baseline` — `align-items: baseline;`
    - `.ai-stretch` — `align-items: stretch;`
- **Align Self (for individual flex items):**
    - `.as-start`, `.as-end`, `.as-center`, `.as-baseline`, `.as-stretch`

_Usage Example:_

```html
<div class="display-f fd-row jc-between ai-center">
  <div>Item 1</div>
  <div>Item 2</div>
</div>
```

### Typography & Width Utilities

#### Font Size Classes

- `.font-sm` — `font-size: 16px;`
- `.font-md` — `font-size: 30px;`
- `.font-lg` — `font-size: 32px;`
- `.font-xl` — `font-size: 40px;`
- `.font-2xl` — `font-size: 54px;`

#### Font Weight Classes

- `.fw-light` — `font-weight: 300;`
- `.fw-normal` — `font-weight: 400;`
- `.fw-medium` — `font-weight: 500;`
- `.fw-semibold` — `font-weight: 600;`
- `.fw-bold` — `font-weight: 700;`

#### Text Alignment & Transformation

- **Alignment:**
    - `.text-left`, `.text-center`, `.text-right`, `.text-justify`
- **Transformation:**
    - `.text-uppercase`, `.text-lowercase`, `.text-capitalize`
- **Decoration:**
    - `.text-underline`, `.text-line-through`, `.text-overline`
    - _(Note: The class `.text-none` appears twice with different intended uses. Consider renaming one if needed.)_

#### Width Classes

- `.w-auto` — `width: auto;`
- `.w-full` — `width: 100%;`
- `.w-screen` — `width: 100vw;`
- `.w-half` — `width: 50%;`
- `.w-third` — `width: 33.333333%;`
- `.w-quarter` — `width: 25%;`
- `.w-fifth` — `width: 20%;`
- `.w-sixth` — `width: 16.666667%;`

_Usage Example:_

```html
<h1 class="font-2xl fw-bold text-center">Large Heading</h1>
<div class="w-half">This element takes up 50% of its container's width.</div>
```

---

## Component & Element Styles

The framework also provides default styling for common HTML elements to ensure consistency.

### Lists

Lists are styled using the `"Fira Code"` font with customized markers:

```css
html ul {
  font-family: "Fira Code", serif;
  list-style: square;
  list-style-position: inside;
}

html ol {
  font-family: "Fira Code", serif;
  list-style: lower-roman;
  list-style-position: inside;
}
```

_Usage Example:_

```html
<ul>
  <li>Item One</li>
  <li>Item Two</li>
</ul>
<ol>
  <li>First</li>
  <li>Second</li>
</ol>
```

### Buttons

Buttons (and anchor elements with button classes) are styled for consistency and include hover effects.

#### Primary Button

```css
button,
button.btn.btn-primary,
a.btn.btn-primary {
  background: #597aff;
  color: #ffffff;
  border: none;
  font-family: "Gemunu Libre", serif;
  font-size: 16px;
  text-align: center;
  min-width: 100px;
  padding: 8px;
  cursor: pointer;
  user-select: none;
}
button:hover,
button.btn.btn-primary:hover,
a.btn.btn-primary:hover {
  background: rgb(140, 162.8614457831, 255);
}
```

#### Other Variants

- **Secondary:** Background `#59ffb7` (hover: lighter variant).
- **Danger:** Background `#ff5959` (hover: `#ff8c8c`).
- **Warning:** Background `#ffac59` (hover: `rgb(255, 197.5, 140)`).
- **Info:** Background `#8b59ff` (hover: `rgb(174.6385542169, 140, 255)`).

_Usage Example:_

```html
<button class="btn btn-primary">Primary</button>
<button class="btn btn-danger">Danger</button>
<a href="#" class="btn btn-primary">Primary Link</a>
```

### Tables

Tables are given a clean, code-style look:

```css
html table {
  font-family: "Fira Code", serif;
  font-size: 15px;
  width: 100%;
}
html table th, html table td {
  border: 1px solid #000000;
  padding: 10px;
  text-align: center;
}
html table th {
  background-color: #597aff;
  color: #ffffff;
  font-weight: bold;
}
```

_Usage Example:_

```html
<table>
  <thead>
    <tr>
      <th>Header 1</th>
      <th>Header 2</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Data 1</td>
      <td>Data 2</td>
    </tr>
  </tbody>
</table>
```

### Headings

Headings are styled with the `"Almarai"` font for a distinctive look:

```css
h1, h2, h3, h4 {
  font-family: "Almarai", serif;
}

h1 {
  font-size: 64px;
  font-weight: 800;
}

h2 {
  font-size: 54px;
  font-weight: 800;
}

h3 {
  font-size: 40px;
  font-weight: 700;
}

h4 {
  font-size: 32px;
  font-weight: 700;
}
```

_Usage Example:_

```html
<h1>Main Title</h1>
<h2>Section Title</h2>
<h3>Subsection Title</h3>
<h4>Minor Heading</h4>
```

### Forms and Inputs

Forms and their elements are styled for clarity and usability.

#### Form Container

```css
.form {
  display: flex;
  flex-direction: column;
  padding: 1em;
  max-width: 300px;
}
```

#### Labels

```css
label {
  display: block;
  font-family: "Gemunu Libre", serif;
  font-size: 30px;
  font-weight: 700;
  color: #000000;
}
```

#### Form Button (within a form)

```css
.form button {
  font-family: "Almarai", serif;
  font-size: 10px;
  font-weight: 700;
  text-align: center;
  color: #000000;
  background-color: #ffac59;
  border: none;
  width: 141px;
  height: 27px;
  margin-top: 1em;
  cursor: pointer;
  align-self: center;
}
.form button:hover {
  background-color: #ff5959;
}
```

#### Input Fields

```css
input {
  font-family: "Fira Code", serif;
  font-size: 16px;
  border: 1px solid #000000;
  background-color: rgba(179, 179, 179, 0.3);
  padding: 0.2em;
  margin-bottom: 1em;
  border-radius: 3px;
}

input::placeholder {
  font-family: "Fira Code", serif;
  font-size: 16px;
  color: rgba(0, 0, 0, 0.5);
}
```

_Usage Example:_

```html
<form class="form">
  <label for="username">Username</label>
  <input type="text" id="username" placeholder="Enter your username">
  <button type="submit">Submit</button>
</form>
```
