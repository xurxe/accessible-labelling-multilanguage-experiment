# ARIA labelling experiment

Just a little experiment on how screen readers handle languages and ARIA labels.

## Test results

All tests done with website in English, OS in Finnish

### MacBook + VoiceOver + Chrome

- macOS version: 10.15.2
- Chrome version: 79.0.3945.130

1. [Finnish voice] close, painike
2. [Finnish voice] close, painike
3. [English voice] close [Finnish voice] painike [English voice] close
4. [English voice] close [Finnish voice] painike
5. [English voice] close [Finnish voice] painike
6. [English voice] close [Finnish voice] painike

### MacBook + VoiceOver + Safari

- macOS version: 10.15.2
- Safari version: 13.0.4

1. [Finnish voice] close, painike
2. [Finnish voice] close, painike
3. [Finnish voice] close, painike, close
4. [Finnish voice] close, painike
5. [Finnish voice] close, painike
6. [English voice] close [Finnish voice] painike

### iPhone + VoiceOver + Chrome and Safari

- iOS version: 13.3
- Chrome version: 79.0.3945.73
- Safari version: 13.0

On iPhone, you can perform a simple gesture (by default, swipe up with one finger) to change VoiceOver language regardless of the OS language. When VoiceOver was in Finnish, everything was ready with a Finnish voice. When VoiceOver was in English, everything was read with an English voice.

## Demo

[See it live!](https://xurxe.github.io/aria-labelling-test)

## Author

Xurxe Toivo García

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

Coming soon.
