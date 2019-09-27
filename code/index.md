---
layout: page
title: Code
---
Here's some CSS:

```css
@media (prefers-color-scheme: dark) {
  body {
    background-color: #444;
    color: #e4e4e4;
  }
  a {
    color: #e39777;
  }
  img {
    /* Images should be desaturated for dark mode:
     * https://web.dev/prefers-color-scheme#re-colorize-and-darken-photographic-images
     */
    filter: grayscale(30%);
  }
}
```
