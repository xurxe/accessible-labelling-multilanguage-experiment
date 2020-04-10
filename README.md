# Accessible labelling multilanguage experiment

Just a little experiment on how screen readers handle languages and different ways of providing accessible labels to elements.

When information is conveyed by visual means (for example, an "X" icon to indicate a Close button), we must provide an accessible label: an equivalent text alternative that can be annouced by screen readers.

Screen readers don't always perform well in multiple languages (for example, when the OS or screen reader UI is in one language, and the web content is in another). There are multiple challenges in this matter, but this experiment was specifically designed to figure out what's the best way to provide text alternatives for elements that don't support an `alt` attribute.

## TL;DR

Put the text alternatives a `<span>` element or similar, and put that **inside** the element in question. Then use CSS to hide it **visually**.

- Do not use `display: none` or `visibility: hidden`, those hide it from screen readers too.
- Something like this works well:

```css
.visually-hidden {
  position: absolute !important;
  height: 1px;
  width: 1px;
  overflow: hidden;
  clip: rect(1px 1px 1px 1px); /* IE6, IE7 */
  clip: rect(1px, 1px, 1px, 1px);
}
```

## Testing site

[Check it out on GitHub pages](https://xurxe.github.io/accessible-labelling-multilanguage-experiment/)!

## Author

Xurxe Toivo García

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
