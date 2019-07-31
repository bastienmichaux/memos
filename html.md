# html

Top-most elements: charset, viewport, Content-Security-Policy. [More](https://htmlhead.dev/).

```html
<!doctype html>
<html>
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<meta http-equiv="Content-Security-Policy" content="default-src 'self'">
</head>
</html>
```

Sectioning

```html
<header>Introductory content, can be multiple</header>
<nav>Set of major links</nav>
<main>Main content of the document</main>
<article>Independent content</article>
<section>Thematic grouping, should have a heading</section>
<aside>"Surrounding" content (sidebars)</aside>
<footer>Copyright, terms of use, contact, etc</footer>
```

Accessibility:
* always use `alt` on medias (images, videos, etc)

Other:
* use closing tags for auto-closing elements if you expect the content to be used by XML software

Ya know:
* all elements before `<body>` are added to a default `<head>` if none is provided
