# 100 Days of Code 2025

## Index:

### HTML & CSS

1. **[Anatomy of an HTML element 👇](#anatomy-of-an-html-element)**
2. **[Anatomy of an CSS Ruleset/Rule 👇](#anatomy-of-a-css-ruleset)**
3. **[CSS - Inline, Internal, External 👇](#css---inline-internal-external)**
4. **[CSS - Correct order for `<a>` Pseudo-classes 👇](#correct-order-for-a-pseudo-classes)**

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
<h1 style="font-family: sans-serif; text-align: center; color: rgb(83, 75, 75);">Arri's Challenge for Monday, January 20th, 2025</h1>
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

## Correct order for `<a>` Pseudo-classes

> [!IMPORTANT]
> **Remember: `LoVe HAte Focus`!!**

```css
a {
  color: rgb(167, 1, 78);
  text-decoration: none;
  transition: all 3ms ease-in-out;
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
```

<br />

**[Return to Top 👆](#100-days-of-code-2025)**

---