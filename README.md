# DocsifyPageloadScrollPlugin

## Description
This plugin try to ensure "direct-link to section", will scroll to the correct section/element.

Internally it check `?id=<element-id>` parameter exist on the URL, uses `scrollIntoView()` on the element id, with delayed execution (2 second default) when Docsify's `hook.ready` is called.


## Usage

Just include this script tag like the other default Docsify plugins (search, emoji, etc). Put it after Docsify script tag.
```html
<script src="https://cdn.jsdelivr.net/gh/rizdaprasetya/docsify-fix-pageload-scroll@master/index.js"></script>
```

## Background

Custom plugin to overcome Docsify scrolling issue.

Docsify have auto scrolling issue on direct-link to section of a page with images: https://github.com/docsifyjs/docsify/issues/351

There was proposed fix, but sadly does not get merged for quite sometime.

This plugin does not directly fix it, but it adds another scroll, after the page loaded.
