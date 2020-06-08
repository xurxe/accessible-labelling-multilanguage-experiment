# Results

## Scoring

- For each test case, I recorded how and with what voice (Finnish or English) the screen reader announces the button. Check out [data.md](2020-04/data.md)!

- I gave scores for each test case. Check out [the Google Sheet's Scores tab](https://docs.google.com/spreadsheets/d/18hjaiR4UyI4lisJQK_L7eHHohkWZwv4vlrvHm1IkIXY/edit#gid=0):

  - 3: Perfect announcement; voices and languages matched correctly.
    - Example 1: [English voice] close button
    - Example 2: [English voice] close [Finnish voice] painike
  - 2: The voices and languages are matched correctly, but there's repetition.
    - Example: [English voice] close [Finnish voice] painike, close
  - 1: The accessible label is announced in the right voice, but the name of the element is announced in the wrong voice. Or, the accessible label is announced multiple times and not all of them correctly.
    - Example: [English voice] close, painike
  - 0: the accessible label is announced in the wrong voice, or there's some other big issue
    - Example 1: [Finnish voice] close, painike

## Analysis

I did some analysis. Check out [the Google Sheet's Analysis tab](https://docs.google.com/spreadsheets/d/18hjaiR4UyI4lisJQK_L7eHHohkWZwv4vlrvHm1IkIXY/edit#gid=1046548750).

- All ARIA-based approaches (A to F) led to language issues in more than 50% test cases.
- Approach G (using a visually hidden text element) led to the least amount of language issues. Furthermore, if we exclude from the analysis the test cases that gave uniformly bad results (score of 0 or 1), approach G was announced perfectly 100% of the time.
- By screen reader:
  - TalkBack had the highest score.
  - VoiceOver (mobile) had the lowest score, because it doesn't automatically switch languages.
- By browser: they all performed quite poorly, with average scores below 1.5.
- By screen reader and browser combination:
  - The most successful combination was NVDA + Firefox. This is interesting, considering that Firefox got only 0 scores with all other screen readers.
  - After Firefox, VoiceOver (desktop), performed the worst with Safari, and it also performed equally with the other three browsers. This is interesting, since I've heard often that VoiceOver is most suited to work with Safari.
  - VoiceOver (mobile) had the exact same behavior in all cases.
  - Both JAWS and TalkBack performed equally with Chrome, Opera, and Edge.

## Conclusion

Put the text alternatives a `<span>` element or similar, and put that **inside** the element in question. Then use CSS to hide it **visually**.

- Do not use `display: none` or `visibility: hidden`, those hide it from screen readers too.
- Something like this works well:

```css
.visually-hidden:not(:focus):not(:focus-within):not(:active) {
  position: absolute;
  height: 1px;
  width: 1px;
  border: 0;
  padding: 0;
  margin: 0;
  overflow: hidden;
  clip: rect(1px 1px 1px 1px); /* IE6, IE7 */
  clip: rect(1px, 1px, 1px, 1px);
  white-space: nowrap;
}
```
