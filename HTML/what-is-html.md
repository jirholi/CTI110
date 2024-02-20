# Beginner's Guide to HTML

HTML (Hypertext Markup Language) is the standard language used to create and design web pages. It provides the basic structure of sites, which is then enhanced and styled by CSS (Cascading Style Sheets) and JavaScript. This tutorial will introduce you to the basics of HTML, including its structure, essential elements, and how to create a simple web page.

## What is HTML?

HTML documents are the foundation of the web. They tell web browsers how to display a web page's content. Each HTML page consists of a series of elements or tags, which you can use to mark up text, link to other pages, embed images, and much more.

## Basic Structure of an HTML Document

Every HTML document follows a basic structure. Here's a simple example

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>My First Web Page</title>
</head>
<body>
    <h1>Welcome to My Website</h1>
    <p>This is a paragraph in my first web page.</p>
</body>
</html>
```

- `<!DOCTYPE html`>: Declares the document type and HTML version.
- `<html`>: The root element of an HTML page.
- `<head>`: Contains meta-information about the HTML document, like its title.
- `<title`>: Specifies the title of the web page (shown in the browser's title bar or tab).
- `<body`>: Contains the content of the HTML document, such as text, images, and links.and HTML version.

## Basic HTML Elements

- Paragraphs: Use the `<p>` tag to define a paragraph.

```html
<p>This is a paragraph.</p>
```

- Headings: HTML offers six levels of headings, `<h1>` being the highest (or most important) level and `<h6`> the least.

```html
<h1>This is a heading</h1>
<h2>This is a smaller heading</h2>
```

- Links: Use the `<a`> tag (anchor) to create links to other pages. The `href` attribute specifies the link's destination.

```html
<a href="https://www.example.com">Visit Example.com</a>
```

- Images: The `<img>` tag is used to embed images in an HTML page. The src attribute specifies the path to the image, and the alt attribute provides alternative text.

```html
<img src="image.jpg" alt="Descriptive Text">
```

- Lists: HTML supports ordered (numbered) and unordered (bulleted) lists. Use the `<ol>` tag for ordered lists and `<ul>` for unordered lists, with `<li>` for each item.

## Creating a Simple Web Page

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>My Simple Web Page</title>
</head>
<body>
    <h1>About Me</h1>
    <p>Hi, I'm learning HTML, and this is my first web page!</p>
    <a href="https://www.example.com">Check out this cool website</a>
    <img src="myphoto.jpg" alt="A photo of me">
</body>
</html>

```

## Semantic HTML

Semantic HTML introduces meaning to the web page rather than just presentation. It helps with search engine optimization, accessibility, and makes the web more inclusive. This tutorial will delve into the specifics of some key semantic HTML5 elements: `<header>`, `<nav>`, `<main>`, `<article>`, `<section>`, and `<footer>`. Each plays a unique role in structuring web content logically and accessibly.

1. The `<header>` Tag
The `<header>` element represents a container for introductory content or a set of navigational links. It's not limited to the top of the page; it can be used in any section or article, but it typically contains:

- Site title or logo
- Main navigation menu

```html
<header>
  <h1>My Website</h1>
  <nav>
    <!-- Navigation links go here -->
  </nav>
</header>
```

2.The `<nav>` Tag
The `<nav>` element is designated for navigation links. This semantic tag informs search engines and assistive technologies that the links inside are major navigation points of the website. It's best practice to have one main `<nav>` element, usually in the `<header>`.

```html
<nav>
  <ul>
    <li><a href="#home">Home</a></li>
    <li><a href="#about">About</a></li>
    <li><a href="#contact">Contact</a></li>
  </ul>
</nav>
```

3.The `<main>` Tag

The `<main>` element encapsulates the primary content of your document. This content should be unique to the document, not repeated across pages like headers or footers. The `<main>` tag aids search engines and assistive technologies in identifying the core topic or functionality of the page.

```html
<main>
  <article>
    <!-- Article content -->
  </article>
  <section>
    <!-- Section content -->
  </section>
</main>
```

4.The `<article>` Tag

An `<article>` represents a self-contained composition in a document, page, application, or site, which is intended to be independently distributable or reusable. This could be a forum post, a magazine or newspaper article, or a blog entry.

```html
<article>
  <h2>Article Title</h2>
  <p>Article content...</p>
</article>
```

5.The `<section>` Tag
The `<section>` element is used to define a section in a document. It's a thematic grouping of content, typically with a heading. Use `<section>` when the content grouped is related to a single theme. It's more specific than a `<div>` but not as specific as an `<article>`.

```html

<section>
  <h2>Section Heading</h2>
  <p>Section content...</p>
</section>
```

6.The `<footer>` Tag
The `<footer>` element represents a footer for its nearest sectioning content or sectioning root element. A footer typically contains information about its containing element like:

- Author information
- Copyright notices
- Contact information
- Sitemap
- Back to top links

```html
Copy code
<footer>
  <p>Copyright © 2024. All rights reserved.</p>
</footer>
```

---

## Pulling it all Together

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>My Blog</title>
</head>
<body>

<!-- <header>: This contains the website's title and the main navigation menu. -->
<header>
    <h1>John's Blog</h1>
    <!-- <nav>: It provides navigation links to different sections of the site, improving the site's usability and accessibility. -->
    <nav>
        <ul>
            <li><a href="#home">Home</a></li>
            <li><a href="#about">About Me</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
    </nav>
</header>

<!-- <main>: This encloses the central content of the web page, making it the focal point of the document. -->
<main>
    <!-- <article>: Each blog post and comment is wrapped in an <article> tag, indicating they are self-contained compositions. -->
    <article>
        <header>
            <h2>The Importance of Semantic HTML</h2>
            <p>Posted on <time datetime="2024-02-20">February 20, 2024</time> by John</p>
        </header>
        <!-- <section>: Used to group related content within the article and the comments section, each <section> has a heading to introduce its content. -->
        <section>
            <h3>What is Semantic HTML?</h3>
            <p>Semantic HTML or semantic markup is HTML that introduces meaning to the web page rather than just presentation. It uses HTML tags to convey the role of the content on web pages...</p>
        </section>
        <section>
            <h3>Benefits of Semantic HTML</h3>
            <p>Using semantic tags provides many benefits, not only for search engines but also for developers and users. It makes web pages more accessible, improves SEO, and facilitates clearer code...</p>
        </section>
        <footer>
            <p>Tags: <a href="#HTML">HTML</a>, <a href="#WebDevelopment">Web Development</a></p>
        </footer>
    </article>

    <section>
        <h2>Comments</h2>
        <article>
            <header>
                <h3>Alice</h3>
                <p>Posted on <time datetime="2024-02-21">February 21, 2024</time></p>
            </header>
            <p>This is really helpful. Thanks for sharing!</p>
        </article>
        <article>
            <header>
                <h3>Bob</h3>
                <p>Posted on <time datetime="2024-02-22">February 22, 2024</time></p>
            </header>
            <p>Great article. Semantic HTML is the way to go for accessible web design.</p>
        </article>
    </section>
</main>

<!-- <footer>: Contains copyright and contact information, offering a consistent closing statement for the web page. -->
<footer>
    <p>Contact me at <a href="mailto:john@example.com">john@example.com</a></p>
    <p>© 2024 John's Blog</p>
</footer>

</body>
</html>

</html>
```
