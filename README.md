# 100 Days of Code 2025

## Index:

### HTML & CSS

1. **[HTML - Anatomy of an HTML element 👇](#anatomy-of-an-html-element)**
2. **[CSS - Anatomy of an CSS Ruleset/Rule 👇](#anatomy-of-a-css-ruleset)**
3. **[CSS - Inline, Internal, External 👇](#css---inline-internal-external)**
4. **[CSS - Correct order for Pseudo-classes for `<a>` (anchor tags) & `<button>` (buttons) 👇](#correct-order-for-pseudo-classes-for-a-anchor-tags--button-buttons)**

<br />

---

## Anatomy of an HTML element

![HTML Anatomy](./01-html-css-basics/extra-files/html-anatomy.jpg)  
**Element Name: `paragraph element`**

<br />

**[Return to Top 👆](#100-days-of-code-2025)**

---

## Anatomy of a CSS ruleset

![Anatomy of a CSS ruleset](./01-html-css-basics/extra-files/css-anatomy.jpg)

<br />

**[Return to Top 👆](#100-days-of-code-2025)**

---

## CSS - Inline, Internal, External

## Inline Styling

```html
<!-- Using inline CSS via the style attribute -->
<h1
  style="font-family: sans-serif; text-align: center; color: rgb(83, 75, 75);"
>
  Arri's Challenge for Monday, January 20th, 2025
</h1>
```

## Internal Styling

```html
<head>
  <!-- Using internal CSS -->
  <style>
    p {
      font-family: sans-serif;
      text-align: center;
      color: rgb(83, 75, 75);
    }
  </style>
</head>
```

## External Styling

```html
<head>
  <!-- Using external CSS -->
  <link rel="stylesheet" href="styles.css" />
</head>
```

<br />

**[Return to Top 👆](#100-days-of-code-2025)**

---

## Correct order for Pseudo-classes for `<a>` (anchor tags) & `<button>` (buttons)

### Anchor Tags:  

<br />

> [!IMPORTANT] 
> **Remember: `LoVe HAte Focus D`!!**  

<br />

```css
a {
  color: rgb(167, 1, 78);
  text-decoration: none;
  transition: all 300ms ease-in-out; /* Increased for smoother transitions */
}

/* 1. :link Pseudo-class - unvisited links */
a:link {
  color: rgb(167, 1, 78);
}

/* 2. :visited Pseudo-class - visited links */
a:visited {
  color: purple;
}

/* 3. :hover Pseudo-class - mouse over links */
a:hover {
  text-decoration: underline;
}

/* 4. :active Pseudo-class - clicked/active links */
a:active {
  color: red;
}

/* 5. :focus Pseudo-class - keyboard navigation */
a:focus {
  outline: 2px solid rgb(167, 1, 78);
  outline-offset: 2px;
}

/* 6. :focus-visible Pseudo-class - enhanced keyboard focus */
a:focus-visible {
  outline: 2px solid rgb(167, 1, 78);
  outline-offset: 2px;
}

/* 7. :disabled Pseudo-class - disabled state */
a:disabled {
  color: #cccccc;
  cursor: not-allowed;
  opacity: 0.7;
}
```

### Buttons:  

<br />

> [!IMPORTANT] 
> **Remember: `HAF D` (Hover → Active → Focus → Disabled)!!**  

<br />

```css
button {
  background: #007bff;
  color: white;
  padding: 10px 20px;
  border: none;
  border-radius: 4px;
  cursor: pointer;
  transition: all 300ms ease-in-out;
}

/* 1. :hover Pseudo-class - mouse over buttons */
button:hover {
  background: #0056b3;
}

/* 2. :active Pseudo-class - clicked/pressed buttons */
button:active {
  transform: scale(0.98);
}

/* 3. :focus Pseudo-class - keyboard navigation */
button:focus {
  outline: 2px solid #0056b3;
  outline-offset: 2px;
}

/* 4. :focus-visible Pseudo-class - enhanced keyboard focus */
button:focus-visible {
  outline: 2px solid #0056b3;
  outline-offset: 2px;
}

/* 5. :disabled Pseudo-class - disabled state */
button:disabled {
  background: #cccccc;
  cursor: not-allowed;
  opacity: 0.7;
}
```

<br />

**[Return to Top 👆](#100-days-of-code-2025)**

---
