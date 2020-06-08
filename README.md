# Accessible labelling multilanguage experiment

Just a little experiment on how screen readers handle languages and different ways of providing accessible labels to elements.

When information is conveyed by visual means (for example, an "X" icon to indicate a Close button), we must provide an accessible label: an equivalent text alternative that can be annouced by screen readers.

Screen readers don't always perform well in multiple languages (for example, when the OS or screen reader UI is in one language, and the web content is in another). There are multiple challenges in this matter, but this experiment was specifically designed to figure out what's the best way to provide text alternatives for elements that don't support an `alt` attribute.

## Overview

I made a website with a number of common ways to provide text alternatives.

Then I performed tests...

...using 4 major screen readers (VoiceOver, NVDA, JAWS, TalkBack)

...on 5 major browsers (Safari, Chrome, Firefox, Opera / Opera Touch, Edge)

...on desktop and mobile

...in 3 modes (continous reading, using keyboard or swiping shortcuts to move the reading cursor, and tabbing to move focus to the next button).

## Testing site

[Check it out on GitHub pages](https://xurxe.github.io/accessible-labelling-multilanguage-experiment/)!

## Outcomes

I'm planning on repeating this experiment once a year.

- [2020 experiment](2020-04)

## Sibling study

- [Screen reader multilanguage experiment](https://github.com/xurxe/screenreader-multilanguage-experiment), the previous study.
- [The troubled state of screen readers in multilingual situations](https://medium.com/@xurxe/the-troubled-state-of-screen-readers-in-multilingual-situations-f6a9da4ecdf3), a Medium article where I explain and analyze several related experiments.

## Author

Xurxe Toivo García

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
