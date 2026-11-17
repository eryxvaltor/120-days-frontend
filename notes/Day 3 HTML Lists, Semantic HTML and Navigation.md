# Day 3: HTML Lists, Semantic HTML and Navigation

## Lists

|Type|Tag|Use when|Item tag|
|---|---|---|---|
|Unordered list|`<ul>`|Order does not matter|`<li>`|
|Ordered list|`<ol>`|Sequence matters|`<li>`|

```html
<ul>
  <li>HTML</li>
  <li>CSS</li>
</ul>

<ol>
  <li>Open the editor</li>
  <li>Write the code</li>
</ol>
```

### Nested Lists

Place a child `<ul>` or `<ol>` **inside a parent `<li>`**.

Every `<li>` must belong to a list container (`<ul>` or `<ol>`).

```html
<ul>
  <li>Frontend
    <ul>
      <li>HTML</li>
      <li>CSS</li>
    </ul>
  </li>
  <li>Backend</li>
</ul>
```

## Semantic HTML

Use elements that describe the **meaning and purpose** of content.

|Element|Purpose|
|---|---|
|`<header>`|Introductory content|
|`<nav>`|Major navigation|
|`<main>`|Primary content|
|`<section>`|Thematic grouping|
|`<article>`|Self-contained content|
|`<aside>`|Supplementary content|
|`<footer>`|Footer information|

```html
<body>
  <header>...</header>
  <nav>...</nav>
  <main>
    <section>...</section>
    <article>...</article>
    <aside>...</aside>
  </main>
  <footer>...</footer>
</body>
```

### div

`<div>` is a generic container with **no inherent semantic meaning**.

## Fragment Navigation

`<a href="#about">About</a>` points to the element with `id="about"`.

```html
<a href="#about">About</a>

<section id="about">
  <h2>About</h2>
</section>
```

IDs must be **unique** within the document.

