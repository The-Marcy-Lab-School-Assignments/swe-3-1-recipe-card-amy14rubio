# Short Response Questions

Answer the following questions in your own words. Each response should be 2-4 sentences.

## Question 1: HTML Structure

What is the difference between the `<head>` and `<body>` sections of an HTML document? What kind of content goes in each?

The <head> section contains **metadata** such as the _page title, character set, and links to CSS or scripts_, while the <body> section contains all of the **visible content** displayed on the webpage.

## Question 2: Semantic HTML

Why should we use semantic elements like `<header>`, `<main>`, and `<footer>` instead of using `<div>` tags for everything?

We should use semantic elements like `<header>`, `<main>`, and `<footer>` because they help define the **purpose** of the content inside each element. They also allow for **clearer CSS targeting** and improve **accessibility** by providing meaningful structure instead of a page full of `<div>` tags.

## Question 3: CSS Selectors

Given the following HTML:

```html
<ul>
  <li class="vegetable">Carrots</li>
  <li class="vegetable">Broccoli</li>
  <li class="fruit" id="favorite">Mango</li>
</ul>
```

Write THREE different CSS rules:

1. One that makes ALL list items have a `yellow` background
2. One that makes only the vegetables have `green` text color
3. One that makes only the Mango `bold`

```css
li {
  background-color: yellow;
}

.vegetable {
  color: green;
}

#favorite {
  font-weight: bold;
}
```

## Question 4: The Box Model

In your own words, explain the four parts of the CSS box model (content, padding, border, margin). What is the purpose of each part?

The **content** is the information stored inside the element. The **padding** is the space between the content and the border. The **border** surrounds the padding and content. The **margin** is the space outside the border that separates the element from other elements.

## Question 5: Box-Sizing

What problem does `box-sizing: border-box` solve? Why do we include it in a CSS reset at the top of our CSS files?

The problem that `box-sizing: border-box` solves is that it ensures an element’s **padding and border are included within its defined width and height**. This helps prevent **layout issues** and keeps **sizing behavior** consistent throughout all elements.

## Question 6: Display Property

What is the difference between `display: block`, `display: inline`, and `display: inline-block`? Give an example of when you might use `inline-block`.

The difference is that `display: block` is the default display value for _block-level elements_ and forces **line breaks**, taking up the full width of its container. `display: inline` **does not force line breaks** and only takes up as much width as its content, padding and margin **cannot be applied vertically** and **neither can width or height be set**. `display: inline-block` behaves like an inline element but **allows control** over width, height, margin, and padding. You might use inline-block when designing a `nav` bar so that elements are aligned horizontally while still allowing spacing and sizing control.
