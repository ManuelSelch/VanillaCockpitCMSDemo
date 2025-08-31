## Vanilla Cockpit Demo
- This demo shows how to connect a vanilla html, csss & js webpage to a `headless CMS backend` like [Cockpit CMS](https://getcockpit.com)

## Concept
- Instead of manually updating every HTML element with `JS`, we use `data-field` attributes to map `HTML` elements to fields in a Cockpit singleton

0. import cockpit lib
```html
<script src="./lib/cockpit.js"></script>
```

1. Mark your HTML elements with `data-field`
```html
<h1 data-field="title"></h1>
<p data-field="subtitle"></p>
```

2. Automatically load the Cockpit CMS data
```html
<body onload="loadCMS('home')">
    ...
</body>
```

3. Enjoy