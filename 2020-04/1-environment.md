# Testing environment

## Languages

- Website language: English + Spanish
- OS language: Finnish
- Screen reader UI: Finnish
- Browser language: Finnish

## Website

I compared the following 7 approaches for labelling a close button:

- K: Using `aria-label`.
- L: Using `aria-label` and an explicit `lang` attribute.
- M: Using `aria-labelledby` and referring to a visually hidden label outside the labelled element.
- N: Using `aria-labelledby` and referring to a visually hidden and `aria-hidden` label outside the labelled element.
- O: Using `aria-labelledby` and referring to a visually hidden label inside the labelled element.
- P: Using `aria-labelledby` and referring to a visually hidden and `aria-hidden` label inside the labelled element.
- Q: Using a visually hidden label inside the labelled element.

## Combinations

- VoiceOver (desktop):

  - Device: MacBook Pro (16-inch, 2019)
  - macOS version: 10.15.2
  - VoiceOver: included with macOS
  - Safari version: 13.1 (15609.1.20.111.8)
  - Chrome version: 81.0.4044.92
  - Firefox version: 75.0
  - Opera version: 67.0.3575.137
  - Edge version: 80.0.361.111

- VoiceOver (mobile):

  - Device: iPhone 11
  - iOS version: 13.4.1
  - VoiceOver: included with iOS
  - Safari version: 13
  - Chrome version: 81.0.4044.62
  - Firefox version: 24.1
  - Opera Touch version: 2.2.1
  - Edge version: 45.2.16

- NVDA

  - Device: Asus X540LA
  - Windows version: 10 Home 18362.418
  - NVDA version: 2019.3.1
  - Safari version: N/A (not maintained)
  - Chrome version: 81.0.4044.92
  - Firefox version: 75.0
  - Opera version: 67.0.3575.137
  - Edge version: 80.0.361.111

- JAWS

  - Device: Asus X540LA
  - Windows version: 10 Home 18362.418
  - JAWS version: 2019.1912.9 Multilingual
  - JAWS with "Language Detect Change" selected
  - Safari version: N/A (not maintained)
  - Chrome version: 81.0.4044.92
  - Firefox version: 75.0
  - Opera version: 67.0.3575.137
  - Edge version: 80.0.361.111

- TalkBack

  - Device: Samsung Galaxy S8+
  - OS: Android 9 Build/PPR1.180610.011
  - TalkBack version: 8.1.0.278818032
  - Safari version: N/A (not maintained)
  - Chrome version: 81.0.4044.96
  - Firefox version: 68.7.0
  - Opera Touch version: 2.3.9
  - Edge version: 45.02.4.4931
