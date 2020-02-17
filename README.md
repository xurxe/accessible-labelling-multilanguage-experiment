# Accessible labelling experiment

Just a little experiment on how screen readers handle languages and different ways of providing accessible labels to elements.

When information is conveyed by visual means (for example, an "X" icon to indicate a Close button), we must provide an accessible label: an equivalent text alternative that can be annouced by screen readers.

Screen readers don't always perform well in multiple languages (for example, when the OS or screen reader UI is in one language, and the web content is in another). There are multiple challenges in this matter, but this experiment was specifically designed to figure out what's the best way to provide text alternatives for elements that don't support an `alt` attribute.

## TL;DR

Put the text alternatives a `<span>` element or similar, and put that **inside** the element in question. Then use CSS to hide it **visually** (do not use `display: none` or `visibility: hidden`, those hide it from screen readers too).

## Setup

I compared the following 6 approaches:

A. Using `aria-label`.

B. Using `aria-label` and an explicit `lang` attribute.

C. Using `aria-labelledby` and referring to a visually-hidden label outside the labelled element.

D. Using `aria-labelledby` and referring to a visually-hidden and `aria-hidden` label outside the labelled element.

E. Using `aria-labelledby` and referring to a visually-hidden label inside the labelled element.

F. Using a visually hidden label inside the labelled element.

...using 4 major screen readers (VoiceOver, NVDA, JAWS, TalkBack)

...on 5 major browsers (Safari, Chrome, Firefox, Opera / Opera Touch, Edge)

...on desktop and mobile

...in 3 modes (continous reading, using keyboard or swiping shortcuts to move the reading cursor, tabbing to move focus)

## Results

- For each test case, I recorded how and with what voice (Finnish or English) the screen reader announces the button. Check out [data.md](data.md)!

- I gave scores for each test case. Check out [the Google spreadsheet](https://docs.google.com/spreadsheets/d/19fpze-03_JEFtm7MKrQM8XehMAQe3T6o2W5BM-zx4AY/), on the "Scores" tab:

  - 3: Perfect announcement
    - Example 1: [English voice] close button
    - Example 2: [English voice] close [Finnish voice] painike
  - 2: The voices and languages are matched correctly, but there's some small issue
    - Example: [English voice] close [Finnish voice] painike, close
  - 1: The accessible label is announced in the right voice, but the name of the element is announced in the wrong voice
    - Example: [English voice] close, painike
  - 0: the accessible label is announced in the wrong voice
    - Example: [Finnish voice] close, painike

- I calculated the mean score for of the 6 approaches. Check out [the Google spreadsheet](https://docs.google.com/spreadsheets/d/19fpze-03_JEFtm7MKrQM8XehMAQe3T6o2W5BM-zx4AY/), on the "Analysis" tab.
  - On the overall analysis, option F was the best, scoring 2.2 out of 3
  - Since in some cases the score was uniform accross approaches (in all likelihood due to poor interaction between the screen reader and browser being tested, rather than to the approach itself), I repeated the analysis exclusing these cases. Option F was still the best, scoring 2.9 out of 3.

## Testing site

[Check it out on GitHub pages](https://xurxe.github.io/accessible-labelling-experiment/)!

## Testing environment

- Website language: English
- OS language: Finnish
- VoiceOver (desktop):

  - Device: MacBook Pro (16-inch, 2019)
  - macOS version: 10.15.2
  - VoiceOver: included with macOS
  - Safari version: 13.0.4
  - Chrome version: 79.0.3945.130
  - Firefox version: 72.0.2
  - Opera version: 66.0.3515.72
  - Edge version: 80.0.361.48

- VoiceOver (mobile):

  - Device: iPhone 11
  - iOS version: 13.3
  - VoiceOver: included with iOS
  - Safari version: 13.0
  - Chrome version: 79.0.3945.73
  - Firefox version: 20.2 (16690)
  - Opera Touch version: 2.0.4
  - Edge version: 44.10.13

- NVDA

  - Device: Asus X540LA
  - Windows version: 10 Home 18362.418
  - NVDA version: 2019.3.1
  - Safari version: N/A (not maintained)
  - Chrome version: 80.0.3987.87
  - Firefox version: 72.0.2
  - Opera version: 66.0.3515.72
  - Edge version: 80.0.361.50

- JAWS

  - Device: Asus X540LA
  - Windows version: 10 Home 18362.418
  - JAWS version: 2019.1912.9 Multilingual
  - JAWS with "Language Detect Change" selected
  - Safari version: N/A (not maintained)
  - Chrome version: 80.0.3987.87
  - Firefox version: 72.0.2
  - Opera version: 66.0.3515.72
  - Edge version: 80.0.361.50

- TalkBack

  - Device: Samsung Galaxy S8+
  - OS: Android 9 Build/PPR1.180610.011
  - TalkBack version: 8.1.0.278818032
  - Safari version: N/A (not maintained)
  - Chrome version: 80.0.3987.99
  - Firefox version: 68.5.0
  - Opera Touch version: 2.3.0
  - Edge version: 44.11.4.4140

## Author

Xurxe Toivo García

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

Coming soon.
