# ARIA labelling experiment

Just a little experiment on how screen readers handle languages and ARIA labels.

## Demo

[Check it out on GitHub pages](https://xurxe.github.io/aria-labelling-test/)!

## Test results

All tests done with website in English, OS in Finnish

### MacBook + VoiceOver + Safari

- macOS version: 10.15.2
- Safari version: 13.0.4

1. [Finnish voice] close, painike
2. [Finnish voice] close, painike
3. [Finnish voice] close, painike, close
4. [Finnish voice] close, painike
5. [Finnish voice] close, painike
6. [English voice] close [Finnish voice] painike

### MacBook + VoiceOver + Chrome

- macOS version: 10.15.2
- Chrome version: 79.0.3945.130

1. [Finnish voice] close, painike
2. [Finnish voice] close, painike
3. [English voice] close [Finnish voice] painike [English voice] close
4. [English voice] close [Finnish voice] painike
5. [English voice] close [Finnish voice] painike
6. [English voice] close [Finnish voice] painike

### MacBook + VoiceOver + Firefox

VoiceOver and Firefox don't really work together

### MacBook + VoiceOver + Opera

- macOS version: 10.15.2
- Opera version: 66.0.3515.72

1. [Finnish voice] close, painike
2. [Finnish voice] close, painike
3. [English voice] close [Finnish voice] painike, close
4. [English voice] close [Finnish voice] painike
5. [English voice] close [Finnish voice] painike
6. [English voice] close [Finnish voice] painike

### MacBook + VoiceOver + Edge

- macOS version: 10.15.2
- Edge version: 80.0.361.48

1. [Finnish voice] close, painike
2. [Finnish voice] close, painike
3. [English voice] close [Finnish voice] painike, close
4. [English voice] close [Finnish voice] painike
5. [English voice] close [Finnish voice] painike, close
6. [English voice] close [Finnish voice] painike

### iPhone + VoiceOver + Safari and Chrome

- iOS version: 13.3
- Chrome version: 79.0.3945.73
- Safari version: 13.0

On iPhone, you can perform a simple gesture (by default, swipe up with one finger) to change VoiceOver language regardless of the OS language. When VoiceOver was in Finnish, everything was ready with a Finnish voice. When VoiceOver was in English, everything was read with an English voice.

### Asus + NVDA + Chrome

- Windows version: 10 Home 18362.418
- Chrome version: 80.0.3987.87

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

### Asus + NVDA + Firefox

- Windows version: 10 Home 18362.418
- Firefox version: 72.0.2

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

### Asus + NVDA + Opera

- Windows version: 10 Home 18362.418
- Opera version: 66.0.3515.72

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

### Asus + NVDA + Edge

- Windows version: 10 Home 18362.418
- Edge version: 44.18362.387.0

With screen reader UI in Finnish and screen reader voice in Finnish:

1. [Finnish voice] painike
2. [Finnish voice] painike
3. [Finnish voice] painike [English voice] close
4. [Finnish voice] painike
5. [Finnish voice] painike, painike [English voice] close [Finnish voice] painike
6. [Finnish voice] painike, painike [English voice] close

With screen reader UI in English and screen reader voice in Finnish:

1. [Finnish voice] button
2. [Finnish voice] button
3. [Finnish voice] button [English voice] close
4. [Finnish voice] button
5. [Finnish voice] button, button [English voice] close [Finnish voice] button
6. [Finnish voice] button, button [English voice] close

## Author

Xurxe Toivo García

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

Coming soon.
