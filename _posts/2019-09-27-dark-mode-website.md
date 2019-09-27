---
layout: page
title: Dark mode in a website with CSS
---
This site has a dark mode and a light one. Which mode you see depends on the setting of your device. Try it!

<video class="large" autoplay loop muted playsinline>
  <source src="/images/dark_mode.mp4" type="video/mp4" />
</video>

The instant change in appearance is accomplished by this appendix to the style sheet:

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
    filter: grayscale(30%);
  }
}
```

This works in Firefox, Safari, and Chrome among other browsers.

## Light on dark

The most important block is the one that overrides the colors of text and the background:

```css
body {
  background-color: #444;
  color: #e4e4e4;
}
```

It's recommended to [avoid pure white](https://web.dev/prefers-color-scheme#avoid-pure-white) for text, and I chose likewise to avoid pure black for the background.

## Desaturate colors

The accent color I use for hyperlinks looked harsh on the dark background, so I overrode it with a less saturated one:

```css
a {
  color: #e39777;
}
```

Photographs also looked harsh. It turns out that many people prefer images, too, to be [desaturated in dark mode](https://medium.com/dev-channel/re-colorization-for-dark-mode-19e2e17b584b):

```css
img {
  filter: grayscale(30%);
}
```

You may want to use a more specific selector here in order to [treat vector images differently](https://web.dev/prefers-color-scheme#invert-vector-graphics-and-icons).
