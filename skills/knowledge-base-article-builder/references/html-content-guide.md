# Clean HTML Content Guide

Use simple semantic HTML that remains readable when pasted into a knowledge-base platform's source editor or processed by an HTML sanitizer.

## Preferred tags

Use only the tags supported by the target platform. When no platform rules are supplied, prefer:

```text
h1 h2 h3 h4 h5 h6
p
ul ol li
strong em
a
table thead tbody tr th td
```

## Preferred attributes

- Links: `href`
- Tables: `border`, `cellpadding`, `cellspacing`
- Table cells: `colspan`, `rowspan`, only when needed

Remove unsupported attributes and all unnecessary styling.

## Avoid

- `<style>` or `<script>`
- CSS or inline style attributes
- `class`, `id`, data attributes, and embedded fonts
- Layout wrappers such as `<div>`, `<span>`, `<section>`, `<article>`, `<header>`, `<footer>`, or `<nav>`
- JavaScript, decorative layout icons, and structural images
- Columns, grids, cards, or other visual structures that may be removed by a sanitizer
- HTML comments

## Cleaning existing HTML

1. Remove comments, scripts, styles, and unsupported attributes.
2. Unwrap unsupported layout tags while preserving readable child content.
3. Preserve valid headings, paragraphs, lists, links, and legitimate tables.
4. Use descriptive link text and absolute URLs when the target platform requires them.
5. Confirm that the result remains understandable without visual styling.

When pasting into a platform editor, provide the content inside the body of the document unless the platform specifically requires a complete HTML document.
