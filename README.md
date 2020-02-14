# Accessible naming experiment

Just a little experiment on how screen readers handle languages and different ways of providing accessible names to elements.

## Demo

[Check it out on GitHub pages](https://xurxe.github.io/aria-labelling-test/)!

## Test results

All tests done with website in English and OS in Finnish

### MacBook + VoiceOver

- macOS version: 10.15.2

#### MacBook + VoiceOver + Safari

- Safari version: 13.0.4

##### MacBook + VoiceOver + Safari + letting the screenreader run

1. [Finnish voice] close, painike
2. [Finnish voice] close, painike
3. [Finnish voice] close, painike, close
4. [Finnish voice] close, painike
5. [Finnish voice] close, painike
6. [English voice] close [Finnish voice] painike

##### MacBook + VoiceOver + Safari + using VO-right arrow to move the reading cursor

1. [Finnish voice] close, painike
2. [Finnish voice] close, painike
3. [English voice] close [Finnish voice] painike [English voice] close
4. [Finnish voice] close, painike
5. [Finnish voice] close, painike
6. [English voice] close [Finnish voice] painike

##### MacBook + VoiceOver + Safari + tabbing to move focus

1. [Finnish voice] close, painike
2. [Finnish voice] close, painike
3. [English voice] close [Finnish voice] painike
4. [Finnish voice] close, painike
5. [Finnish voice] close, painike
6. [English voice] close [Finnish voice] painike

#### MacBook + VoiceOver + Chrome

- Chrome version: 79.0.3945.130

##### MacBook + VoiceOver + Chrome + letting the screenreader run

1. [Finnish voice] close, painike
2. [Finnish voice] close, painike
3. [English voice] close [Finnish voice] painike, close
4. [English voice] close [Finnish voice] painike
5. [English voice] close [Finnish voice] painike
6. [English voice] close [Finnish voice] painike

##### MacBook + VoiceOver + Chrome + using VO-right arrow to move the reading cursor

1. [Finnish voice] close, painike
2. [Finnish voice] close, painike
3. [English voice] close [Finnish voice] painike [English voice] close
4. [English voice] close [Finnish voice] painike
5. [English voice] close [Finnish voice] painike
6. [English voice] close [Finnish voice] painike

##### MacBook + VoiceOver + Chrome + tabbing to move focus

1. [Finnish voice] close, painike
2. [Finnish voice] close, painike
3. [English voice] close [Finnish voice] painike
4. [English voice] close [Finnish voice] painike
5. [English voice] close [Finnish voice] painike
6. [English voice] close [Finnish voice] painike

#### MacBook + VoiceOver + Firefox

VoiceOver and Firefox didn't really work together on desktop.

#### MacBook + VoiceOver + Opera

- Opera version: 66.0.3515.72

##### MacBook + VoiceOver + Opera + letting the screenreader run

1. [Finnish voice] close, painike
2. [Finnish voice] close, painike
3. [English voice] close [Finnish voice] painike, close
4. [English voice] close [Finnish voice] painike
5. [English voice] close [Finnish voice] painike
6. [English voice] close [Finnish voice] painike

##### MacBook + VoiceOver + Opera + using VO-right arrow to move the reading cursor

1. [Finnish voice] close, painike
2. [Finnish voice] close, painike
3. [English voice] close [Finnish voice] painike [English voice] close
4. [English voice] close [Finnish voice] painike
5. [English voice] close [Finnish voice] painike
6. [English voice] close [Finnish voice] painike

##### MacBook + VoiceOver + Opera + tabbing to move focus

1. [Finnish voice] close, painike
2. [Finnish voice] close, painike
3. [English voice] close [Finnish voice] painike
4. [English voice] close [Finnish voice] painike
5. [English voice] close [Finnish voice] painike
6. [English voice] close [Finnish voice] painike

#### MacBook + VoiceOver + Edge

- Edge version: 80.0.361.48

##### MacBook + VoiceOver + Edge + letting the screenreader run

1. [Finnish voice] close, painike
2. [Finnish voice] close, painike
3. [English voice] close [Finnish voice] painike, close
4. [English voice] close [Finnish voice] painike
5. [English voice] close [Finnish voice] painike, close
6. [English voice] close [Finnish voice] painike

##### MacBook + VoiceOver + Edge + using VO-right arrow to move the reading cursor

1. [Finnish voice] close, painike
2. [Finnish voice] close, painike
3. [English voice] close [Finnish voice] painike [English voice] close
4. [English voice] close [Finnish voice] painike
5. [English voice] close [Finnish voice] painike, close
6. [English voice] close [Finnish voice] painike

##### MacBook + VoiceOver + Edge + tabbing to move focus

1. [Finnish voice] close, painike
2. [Finnish voice] close, painike
3. [English voice] close [Finnish voice] painike
4. [English voice] close [Finnish voice] painike
5. [English voice] close [Finnish voice] painike, close
6. [English voice] close [Finnish voice] painike

### iPhone + VoiceOver

- iOS version: 13.3

#### iPhone + VoiceOver + Safari, Chrome, Firefox, Opera Touch, Edge

- Chrome version: 79.0.3945.73
- Safari version: 13.0
- Firefox version: 20.2 (16690)
- Opera Touch version: 2.0.4
- Edge version: 44.10.13

On iPhone, you can perform a simple gesture (by default, swipe up with one finger) to change VoiceOver language regardless of the OS language. When VoiceOver was in Finnish, everything was ready with a Finnish voice. When VoiceOver was in English, everything was read with an English voice.

### Asus + NVDA

- Windows version: 10 Home 18362.418
- NVDA version: 2019.3.1

#### Asus + NVDA + Chrome

- Chrome version: 80.0.3987.87

##### Asus + NVDA + Chrome + letting the screen reader run

With screen reader UI in Finnish and screen reader voice in Finnish:

1. [Finnish voice] painike, close
2. [Finnish voice] painike, close
3. [Finnish voice] painike, close [English voice] close
4. [Finnish voice] painike, close
5. [Finnish voice] painike, close
6. [Finnish voice] painike [English voice] close

With screen reader UI in English and screen reader voice in Finnish:

1. [Finnish voice] button, close
2. [Finnish voice] button, close
3. [Finnish voice] button, close [English voice] close
4. [Finnish voice] button, close
5. [Finnish voice] button, close
6. [Finnish voice] button [English voice] close

##### Asus + NVDA + Chrome + using down arrow to move reading cursor

Cannot go directly to button, so we have to wait to hear the entire list item. It behaves as letting the screen reader run completely.

##### Asus + NVDA + Chrome + tabbing to move focus

With screen reader UI in Finnish and screen reader voice in Finnish:

1. [Finnish voice] close painike
2. [Finnish voice] close painike
3. [Finnish voice] close painike
4. [Finnish voice] close painike
5. [Finnish voice] close painike
6. [English voice] close [Finnish voice] painike

With screen reader UI in English and screen reader voice in Finnish:

1. [Finnish voice] close button
2. [Finnish voice] close button
3. [Finnish voice] close button
4. [Finnish voice] close button
5. [Finnish voice] close button
6. [English voice] close [Finnish voice] button

#### Asus + NVDA + Firefox

- Firefox version: 72.0.2

##### Asus + NVDA + Firefox + letting the screen reader run

With screen reader UI in Finnish and screen reader voice in Finnish:

1. [Finnish voice] painike [English voice] close
2. [Finnish voice] painike [English voice] close
3. [Finnish voice] painike [English voice] close, close
4. [Finnish voice] painike [English voice] close
5. [Finnish voice] painike [English voice] close
6. [Finnish voice] painike [English voice] close

With screen reader UI in English and screen reader voice in Finnish:

1. [Finnish voice] button [English voice] close
2. [Finnish voice] button [English voice] close
3. [Finnish voice] button [English voice] close, close
4. [Finnish voice] button [English voice] close
5. [Finnish voice] button [English voice] close
6. [Finnish voice] button [English voice] close

##### Asus + NVDA + Firefox + using down arrow to move reading cursor

Cannot go directly to button, so we have to wait to hear the entire list item. It behaves as letting the screen reader run completely.

##### Asus + NVDA + Firefox + tabbing to move focus

With screen reader UI in Finnish and screen reader voice in Finnish:

1. [English voice] close [Finnish voice] painike
2. [English voice] close [Finnish voice] painike
3. [English voice] close [Finnish voice] painike
4. [English voice] close [Finnish voice] painike
5. [English voice] close [Finnish voice] painike
6. [English voice] close [Finnish voice] painike

With screen reader UI in English and screen reader voice in Finnish:

1. [English voice] close [Finnish voice] button
2. [English voice] close [Finnish voice] button
3. [English voice] close [Finnish voice] button
4. [English voice] close [Finnish voice] button
5. [English voice] close [Finnish voice] button
6. [English voice] close [Finnish voice] button

#### Asus + NVDA + Opera

- Opera version: 66.0.3515.72

##### Asus + NVDA + Opera + letting the screen reader run

With screen reader UI in Finnish and screen reader voice in Finnish:

1. [Finnish voice] painike, close
2. [Finnish voice] painike, close
3. [Finnish voice] painike, close [English voice] close
4. [Finnish voice] painike, close
5. [Finnish voice] painike, close
6. [Finnish voice] painike [English voice] close

With screen reader UI in English and screen reader voice in Finnish:

1. [Finnish voice] button, close
2. [Finnish voice] button, close
3. [Finnish voice] button, close [English voice] close
4. [Finnish voice] button, close
5. [Finnish voice] button, close
6. [Finnish voice] button [English voice] close

##### Asus + NVDA + Opera + using down arrow to move reading cursor

Cannot go directly to button, so we have to wait to hear the entire list item. It behaves as letting the screen reader run completely.

##### Asus + NVDA + Opera + tabbing to move focus

With screen reader UI in Finnish and screen reader voice in Finnish:

1. [Finnish voice] close painike
2. [Finnish voice] close painike
3. [Finnish voice] close painike
4. [Finnish voice] close painike
5. [Finnish voice] close painike
6. [English voice] close [Finnish voice] painike

With screen reader UI in English and screen reader voice in Finnish:

1. [Finnish voice] close button
2. [Finnish voice] close button
3. [Finnish voice] close button
4. [Finnish voice] close button
5. [Finnish voice] close button
6. [English voice] close [Finnish voice] button

#### Asus + NVDA + Edge

- Edge version: 80.0.361.50

##### Asus + NVDA + Edge + letting the screen reader run

With screen reader UI in Finnish and screen reader voice in Finnish:

1. [Finnish voice] painike, close
2. [Finnish voice] painike, close
3. [Finnish voice] painike, close [English voice] close
4. [Finnish voice] painike, close
5. [Finnish voice] painike, close
6. [Finnish voice] painike [English voice] close

With screen reader UI in English and screen reader voice in Finnish:

1. [Finnish voice] button, close
2. [Finnish voice] button, close
3. [Finnish voice] button, close [English voice] close
4. [Finnish voice] button, close
5. [Finnish voice] button, close
6. [Finnish voice] button [English voice] close

##### Asus + NVDA + Edge + using down arrow to move reading cursor

Cannot go directly to button, so we have to wait to hear the entire list item. It behaves as letting the screen reader run completely.

##### Asus + NVDA + Edge + tabbing to move focus

With screen reader UI in Finnish and screen reader voice in Finnish:

1. [Finnish voice] close painike
2. [Finnish voice] close painike
3. [Finnish voice] close painike
4. [Finnish voice] close painike
5. [Finnish voice] close painike
6. [English voice] close [Finnish voice] painike

With screen reader UI in English and screen reader voice in Finnish:

1. [Finnish voice] close, button
2. [Finnish voice] close, button
3. [Finnish voice] close, button
4. [Finnish voice] close, button
5. [Finnish voice] close, button
6. [English voice] close [Finnish voice] button

### Asus + JAWS

- Windows version: 10 Home 18362.418
- JAWS version: 2019.1912.9 Multilingual
- JAWS with "Language Detect Change" selected

#### Asus + JAWS + Chrome

- Chrome version: 80.0.3987.87

##### Asus + JAWS + Chrome + letting the screen reader run

With screen reader UI in Finnish and screen reader voice in Finnish:

1. [English voice] close painike
2. [English voice] close painike
3. [English voice] close painike, close
4. [English voice] close painike
5. [English voice] close painike
6. [English voice] close painike

With screen reader UI in English and screen reader voice in Finnish:

1. [English voice] close button
2. [English voice] close button
3. [English voice] close button, close
4. [English voice] close button
5. [English voice] close button
6. [English voice] close button

##### Asus + JAWS + Chrome + using the down arrow to move the reading cursor

With screen reader UI in Finnish and screen reader voice in Finnish:

1. [English voice] close painike
2. [English voice] close painike
3. [English voice] close painike, close
4. [English voice] close painike
5. [English voice] close painike
6. [English voice] close painike

With screen reader UI in English and screen reader voice in Finnish:

1. [English voice] close button
2. [English voice] close button
3. [English voice] close button, close
4. [English voice] close button
5. [English voice] close button
6. [English voice] close button

##### Asus + JAWS + Chrome + tabbing to move focus

With screen reader UI in Finnish and screen reader voice in Finnish:

1. [English voice] close [Finnish voice] painike
2. [English voice] close [Finnish voice] painike
3. [English voice] close [Finnish voice] painike
4. [English voice] close [Finnish voice] painike
5. [English voice] close [Finnish voice] painike
6. [English voice] close [Finnish voice] painike

With screen reader UI in English and screen reader voice in Finnish:

1. [English voice] close button
2. [English voice] close button
3. [English voice] close button
4. [English voice] close button
5. [English voice] close button
6. [English voice] close button

#### Asus + JAWS + Firefox

- Firefox version: 72.0.2

##### Asus + JAWS + Firefox + letting the screen reader run

With screen reader UI in Finnish and screen reader voice in Finnish:

1. [English voice] close painike
2. [English voice] close painike
3. [English voice] close painike, close
4. [English voice] close painike
5. [English voice] close painike
6. [English voice] close painike

With screen reader UI in English and screen reader voice in Finnish:

1. [English voice] close button
2. [English voice] close button
3. [English voice] close button, close
4. [English voice] close button
5. [English voice] close button
6. [English voice] close button

##### Asus + JAWS + Firefox + using down arrow to move the reading cursor

With screen reader UI in Finnish and screen reader voice in Finnish:

1. [English voice] close painike
2. [English voice] close painike
3. [English voice] close painike, close
4. [English voice] close painike [silence]
5. [English voice] close painike
6. [English voice] close painike

With screen reader UI in English and screen reader voice in Finnish:

1. [English voice] close button
2. [English voice] close button
3. [English voice] close button, close
4. [English voice] close button, blank
5. [English voice] close button
6. [English voice] close button

##### Asus + JAWS + Firefox + tabbing to move focus

With screen reader UI in Finnish and screen reader voice in Finnish:

1. [English voice] close [Finnish voice] painike
2. [English voice] close [Finnish voice] painike
3. [English voice] close [Finnish voice] painike
4. [English voice] close [Finnish voice] painike
5. [English voice] close [Finnish voice] painike
6. [English voice] close [Finnish voice] painike

With screen reader UI in English and screen reader voice in Finnish:

1. [English voice] close button
2. [English voice] close button
3. [English voice] close button
4. [English voice] close button
5. [English voice] close button
6. [English voice] close button

#### Asus + JAWS + Opera

- Opera version: 66.0.3515.72

##### Asus + JAWS + Opera + letting the screen reader run

With screen reader UI in Finnish and screen reader voice in Finnish:

1. [English voice] close painike
2. [English voice] close painike
3. [English voice] close painike, close
4. [English voice] close painike
5. [English voice] close painike
6. [English voice] close painike

With screen reader UI in English and screen reader voice in Finnish:

1. [English voice] close button
2. [English voice] close button
3. [English voice] close button, close
4. [English voice] close button
5. [English voice] close button
6. [English voice] close button

##### Asus + JAWS + Opera + using down arrow to move the reading cursor

With screen reader UI in Finnish and screen reader voice in Finnish:

1. [English voice] close painike
2. [English voice] close painike
3. [English voice] close painike, close
4. [English voice] close painike
5. [English voice] close painike
6. [English voice] close painike

With screen reader UI in English and screen reader voice in Finnish:

1. [English voice] close button
2. [English voice] close button
3. [English voice] close button, close
4. [English voice] close button, blank
5. [English voice] close button
6. [English voice] close button

##### Asus + JAWS + Opera + tabbing to move focus

With screen reader UI in Finnish and screen reader voice in Finnish:

1. [English voice] close [Finnish voice] painike
2. [English voice] close [Finnish voice] painike
3. [English voice] close [Finnish voice] painike
4. [English voice] close [Finnish voice] painike
5. [English voice] close [Finnish voice] painike
6. [English voice] close [Finnish voice] painike

With screen reader UI in English and screen reader voice in Finnish:

1. [English voice] close button
2. [English voice] close button
3. [English voice] close button
4. [English voice] close button
5. [English voice] close button
6. [English voice] close button

#### Asus + JAWS + Edge

- Edge version: 44.18362.387.0

##### Asus + JAWS + Edge + letting the screen reader run

With screen reader UI in Finnish and screen reader voice in Finnish:

1. [English voice] close painike
2. [English voice] close painike
3. [English voice] close painike, close
4. [English voice] close painike
5. [English voice] close painike
6. [English voice] close painike

With screen reader UI in English and screen reader voice in Finnish:

1. [English voice] close button
2. [English voice] close button
3. [English voice] close button, close
4. [English voice] close button
5. [English voice] close button
6. [English voice] close button

##### Asus + JAWS + Edge + using down arrow to move the reading cursor

With screen reader UI in Finnish and screen reader voice in Finnish:

1. [English voice] close painike
2. [English voice] close painike
3. [English voice] close painike, close
4. [English voice] close painike
5. [English voice] close painike
6. [English voice] close painike

With screen reader UI in English and screen reader voice in Finnish:

1. [English voice] close button
2. [English voice] close button
3. [English voice] close button, close
4. [English voice] close button
5. [English voice] close button
6. [English voice] close button

##### Asus + JAWS + Edge + tabbing to move focus

With screen reader UI in Finnish and screen reader voice in Finnish:

1. [Finnish voice] This button has `aria-label`: [English voice] close [Finnish voice] painike
2. [Finnish voice] This button has `aria-label` and an explicit `lang` attribute: [English voice] close [Finnish voice] painike
3. [Finnish voice] This button has `aria-labelledby`, and the visually-hidden label is outside: [English voice] close [Finnish voice] painike
4. [Finnish voice] This button has `aria-labelledby`, and the `aria-hidden` and visually-hidden label is outside: [English voice] close [Finnish voice] painike
5. [Finnish voice] This button has `aria-labelledby`, and the visually-hidden label is inside: [English voice] close [Finnish voice] painike
6. [Finnish voice] This button has a visually-hidden label inside: [English voice] close [Finnish voice] painike

With screen reader UI in English and screen reader voice in Finnish:

1. [English voice] This button has `aria-label`: close button
2. [English voice] This button has `aria-label` and an explicit `lang` attribute: close button
3. [English voice] This button has `aria-labelledby`, and the visually-hidden label is outside: close button
4. [English voice] This button has `aria-labelledby`, and the `aria-hidden` and visually-hidden label is outside: close button
5. [English voice] This button has `aria-labelledby`, and the visually-hidden label is inside: close button
6. [English voice] This button has a visually-hidden label inside: close button

## Author

Xurxe Toivo García

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

Coming soon.
