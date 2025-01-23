# 100 Days of Code 2025

## Index:

## HTML & CSS:

1. **[HTML - Anatomy of an HTML element🔻](#anatomy-of-an-html-element)**
2. **[CSS - Anatomy of an CSS Ruleset/Rule🔻](#anatomy-of-a-css-ruleset)**
3. **[CSS - Inline, Internal, External🔻](#css---inline-internal-external)**
4. **[CSS - ⚠️ CORRECT ORDER for Pseudo-classes for `<a>` (anchor tags) & `<button>` (buttons)🔻](#correct-order-for-pseudo-classes-for-a-anchor-tags--button-buttons)**  

## HTML & CSS Deep Dive:  
5. **[CSS - Remove list styles, e.g. circle, squares, numbers, etc.🔻](#remove-list-styles-eg-circle-squares-numbers-etc)**
6. **[CSS - Box Model - ⚠️ Box Sizing🔻](#box-model---box-sizing)**  
7. **[CSS - ⚠️ Different VALUES AND SHORTHANDS for PADDING and MARGIN🔻](#different-values-and-shorthands-for-padding-and-margin)**  
8. **[CSS - ⚠️ Margin COLLAPSE🔻](#margin-collapse)**  
9. **[CSS - Centering an Element🔻](#centering-an-element)** 
10. **[HTML - ⚠️ Semantic HTML🔻](#semantic-html)**
11. **[CSS - ⚠️ Selectors and Combinators🔻](#css-selectors-and-combinators)**
12. **[HTML - Dates `<time>`🔻](#html-dates-time)**


<br />

---

## Anatomy of an HTML element

![HTML Anatomy](../assets/html-anatomy.jpg)  
**Element Name: `paragraph element`**

<br />

**[Return to Top 🔝](#100-days-of-code-2025)**

---

## Anatomy of a CSS ruleset

![Anatomy of a CSS ruleset](../assets/css-anatomy.jpg)

<br />

**[Return to Top 🔝](#100-days-of-code-2025)**

---

## CSS - Inline, Internal, External

## Inline Styling

```html
<!-- Using inline CSS via the style attribute -->
<h1 style="font-family: sans-serif; text-align: center; color: rgb(83, 75, 75);">
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

> [!TIP] 
> **"Separation of Concerns" (SoC) - Separate HTML, CSS, and JavaScript into different files.**  

<br />

```html
<head>
  <!-- Using external CSS -->
  <link rel="stylesheet" href="styles.css" />
</head>
```

<br />

**[Return to Top 🔝](#100-days-of-code-2025)**

---

## Correct order for Pseudo-classes for `<a>` (anchor tags) & `<button>` (buttons)

### Anchor Tags:  

> [!IMPORTANT] 
> **Remember: `LoVe HAte Focus D` (Link → Visited → Hover → Active → Focus → Disabled)!!**  

<br />

```html
<a href="https://developer.mozilla.org/en-US/" target="_blank" rel="noopener noreferrer">more learning resources</a>
```

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

**[Return to Top 🔝](#100-days-of-code-2025)**

---

## Remove list styles, e.g. circle, squares, numbers, etc.   


```css
/* INHERITANCE: On the parent element, can style the li's individually later on if needed. */
ol {
  list-style: none;
}
```

<br />

**[Return to Top 🔝](#100-days-of-code-2025)**

---

## Box Model - Box Sizing   


```css
/* Ensures padding and border are included in the total width and height. The default is content-box. */
* {
  box-sizing: border-box;
}
```

![Box Model](../assets/box-model.webp)  

<br />

**[Return to Top 🔝](#100-days-of-code-2025)**

---


## Different values and shorthands for PADDING and MARGIN  


```css
BUTTON {
  /* 1. Horizontal refers to the main-axis (x-axis), affecting the left and right sides. */
  /* 2. Vertical refers to the cross-axis (y-axis), affecting the top and bottom sides. */

  /* -------------------------------------------------------------------------- */

  /* Four values: Top (y-axis) | Right (x-axis) | Bottom (y-axis) | Left (x-axis) */
  padding: 5px 10px 20px 12px;

  /* Three values: Top (y-axis) | Horizontal (x-axis: Right & Left) | Bottom (y-axis) */
  padding: 5px 10px 20px;

  /* Two values: Vertical (y-axis: Top & Bottom) | Horizontal (x-axis: Right & Left) */
  padding: 5px 10px;

  /* One value: All sides (y-axis and x-axis) */
  padding: 5px;

  /* ⚠️ MARGIN ONLY ⚠️ - x-axis: Centres the element horizontally on the main axis */
  margin: auto;

  /* ⚠️ MARGIN ONLY ⚠️ - Combination of absolute and auto values */
  /* Top (y-axis): 10px */
  /* Horizontal (x-axis: Right & Left): auto (centres horizontally) */
  /* Bottom (y-axis): 20px */
  margin: 10px auto 20px;
}
```


<br />

**[Return to Top 🔝](#100-days-of-code-2025)**

---

## Margin COLLAPSE  

> [!IMPORTANT]
> **Margin collapse occurs when two vertical margins (top/bottom) meet. Instead of adding up, the larger margin "wins".**

```css
/* Basic Example */
.box-1 {
  margin-bottom: 20px;
}

.box-2 {
  margin-top: 30px;
}

/* The space between box-1 and box-2 will be 30px (not 50px) */

/* Common ways to prevent margin collapse: */
.box-1 {
  /* Method 1: Add a border */
  border-bottom: 1px solid transparent;
  
  /* Method 2: Add padding */
  padding-bottom: 1px;
  
  /* 
    EASIEST: Method 3: BFC (Block Formatting Context): 
    - A BFC is a region in a webpage that creates its own independent formatting environment   
      that follows its own rules and is isolated from outside elements. 
    - This method is the EASIEST and most RELIABLE way to prevent margin collapse.
  */
  display: flex;
  /* or */
  overflow: hidden;
}
```


<br />

**[Return to Top 🔝](#100-days-of-code-2025)**

---

## Centering an Element  


```css
ol {
  /* Horizontal Margin: auto (centres the element horizontally) */
  /* Top | Right (auto) | Bottom | Left (auto) */
  margin: 36px auto 0 auto;
}
```


<br />

**[Return to Top 🔝](#100-days-of-code-2025)**

---

## Semantic HTML  


```html
<!doctype html>
<html lang="en-US">
  <head>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width" />

    <title>Web Development Guide | Learn HTML & CSS</title>
    <link
      href="https://fonts.googleapis.com/css?family=Open+Sans+Condensed:300|Sonsie+One"
      rel="stylesheet" />
    <link rel="stylesheet" href="style.css" />
  </head>

  <body>
    <!-- Header contains the main branding and top-level site information -->
    <header>
      <h1>Modern Web Development</h1>
    </header>

    <!-- Nav element represents the main navigation menu -->
    <nav>
      <ul>
        <li><a href="#">Getting Started</a></li>
        <li><a href="#">HTML Basics</a></li>
        <li><a href="#">CSS Tutorials</a></li>
        <li><a href="#">Resources</a></li>
      </ul>

      <!-- A Search form: another common non-linear way to navigate through a site. -->
      <form>
        <input type="search" name="q" placeholder="Search tutorials..." />
        <input type="submit" value="Search" />
      </form>
    </nav>

    <!-- Main element contains the primary content of the page -->
    <main>
      <!-- Article represents a self-contained composition (like a blog post or news story) -->
      <article>
        <h2>Introduction to Semantic HTML</h2>

        <p>
          Semantic HTML is the foundation of modern web development. By using the
          right HTML elements, we create websites that are both accessible and
          SEO-friendly. This guide will help you understand how to structure your
          web pages effectively using semantic elements like header, nav, main,
          article, and footer.
        </p>

        <section>
          <h3>Understanding Document Structure</h3>

          <p>
            A well-structured HTML document helps both users and search engines
            navigate your content. Each semantic element serves a specific purpose,
            making your code more meaningful and easier to maintain.
          </p>

          <p>
            For example, the header element typically contains your site's branding
            and main navigation, while the main element wraps around your page's
            primary content. This clear structure improves accessibility and helps
            screen readers better interpret your content.
          </p>
        </section>

        <section>
          <h3>Writing Clean, Accessible Code</h3>

          <p>
            Accessibility should never be an afterthought. By using semantic HTML
            elements correctly, you're already taking important steps toward making
            your website accessible to all users, including those using screen
            readers or keyboard navigation.
          </p>

          <p>
            Remember to include proper ARIA labels where needed, use meaningful alt
            text for images, and maintain a logical heading structure. These
            practices ensure your website can be used by everyone, regardless of
            how they access the web.
          </p>
        </section>
      </article>

      <!-- Aside contains content that is related but not essential to the main content -->
      <aside>
        <h2>Recommended Reading</h2>

        <ul>
          <li><a href="#">Getting Started with HTML5</a></li>
          <li><a href="#">CSS Best Practices Guide</a></li>
          <li><a href="#">Web Accessibility Fundamentals</a></li>
          <li><a href="#">Responsive Design Basics</a></li>
          <li><a href="#">SEO for Web Developers</a></li>
        </ul>
      </aside>
    </main>

    <!-- Footer contains site-wide information like copyright, contact info, etc. -->
    <footer>
      <p>©Copyright 2024 Web Development Guide. All rights reserved.</p>
    </footer>
  </body>
</html>
```


<br />

**[Return to Top 🔝](#100-days-of-code-2025)**


---

## CSS Selectors and Combinators  

### Key Selectors

```css
/* 1. Basic Selectors - Target elements directly */
#id { }                 /* ID selector [0,1,0,0] (avoid for styling) */
.class { }              /* Class selector [0,0,1,0] */
p { }                   /* Element selector [0,0,0,1] */
* { }                   /* Universal selector [0,0,0,0] */

/* 2. Attribute Selectors - Target elements by their attributes */
[disabled] { }          /* Has attribute [0,0,1,0] */
[type="text"] { }       /* Exact match [0,0,1,0] */
[class*="btn-"] { }     /* Contains [0,0,1,0] */
[href^="https"] { }     /* Starts with [0,0,1,0] */
[src$=".pdf"] { }       /* Ends with [0,0,1,0] */

/* 3. Combinators - Define relationships between elements */
article p { }           /* Descendant: any p inside article [0,0,0,2] */
article > p { }         /* Child: direct p only [0,0,0,2] */
h2 + p { }             /* Adjacent: p right after h2 [0,0,0,2] */
h2 ~ p { }             /* Sibling: any p after h2 [0,0,0,2] */

/* 4. Pseudo-classes - Target special states */

/* Links: Remember "LoVe HAte Focus D" order! */
a:link { }             /* 1. Unvisited links [0,0,1,1] */
a:visited { }          /* 2. Visited links [0,0,1,1] */
a:hover { }            /* 3. Mouse over [0,0,1,1] */
a:active { }           /* 4. During click [0,0,1,1] */
a:focus { }            /* 5. Keyboard navigation [0,0,1,1] */
a:disabled { }         /* 6. Disabled state [0,0,1,1] */

/* Buttons: Remember "HAF D" order! */
button:hover { }       /* Mouse over [0,0,1,1] */
button:active { }      /* During click [0,0,1,1] */
button:focus { }       /* Keyboard focus [0,0,1,1] */
button:disabled { }    /* Disabled state [0,0,1,1] */

/* Form States */
input:checked { }      /* Checked inputs [0,0,1,1] */
input:valid { }        /* Valid inputs [0,0,1,1] */
input:invalid { }      /* Invalid inputs [0,0,1,1] */

/* Position-based */
li:first-child { }     /* First element [0,0,1,1] */
li:last-child { }      /* Last element [0,0,1,1] */
li:nth-child(2n) { }   /* Even elements [0,0,1,1] */

/* 5. Pseudo-elements - Style specific parts of elements */
p::first-letter { }    /* First letter [0,0,0,2] */
p::first-line { }      /* First line [0,0,0,2] */
p::selection { }       /* Selected text [0,0,0,1] */
::placeholder { }      /* Input placeholder [0,0,0,1] */

/* Content insertion */
.quote::before {       /* Before element [0,0,1,1] */
    content: "❝";
}
.quote::after {        /* After element [0,0,1,1] */
    content: "❞";
}
```

> [!IMPORTANT]
> **Remember these orders:**
> - Links: **LoVe HAte** (Link, Visited, Hover, Active)
> - Buttons: **HAF D** (Hover, Active, Focus, Disabled)

<br />

**[Return to Top 🔝](#100-days-of-code-2025)**

---

## HTML Dates `<time>`


```html
<h2>
  <time datetime="2025-01-23">Thursday, January 23rd, 2025</time>
</h2>
```

<br />

**[Return to Top 🔝](#100-days-of-code-2025)**

---