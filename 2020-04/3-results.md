# Results

- For each test case, I recorded how and with what voice (Finnish or English) the screen reader announces the button. Check out [data.md](data.md)!

- I gave scores for each test case. Check out [the Google spreadsheet](https://docs.google.com/spreadsheets/d/19fpze-03_JEFtm7MKrQM8XehMAQe3T6o2W5BM-zx4AY/), on the "Scores" tab:

  - 3: Perfect announcement
    - Example 1: [English voice] close button
    - Example 2: [English voice] close [Finnish voice] painike
  - 2: The voices and languages are matched correctly, but there's some small issue
    - Example: [English voice] close [Finnish voice] painike, close
  - 1: The accessible label is announced in the right voice, but the name of the element is announced in the wrong voice
    - Example: [English voice] close, painike
  - 0: the accessible label is announced in the wrong voice, or there's some other big issue
    - Example 1: [Finnish voice] close, painike
    - Example 2: [English voice] This button has aria-label: close button

- I calculated the mean score for of the 6 approaches. Check out [the Google spreadsheet](https://docs.google.com/spreadsheets/d/19fpze-03_JEFtm7MKrQM8XehMAQe3T6o2W5BM-zx4AY/), on the "Analysis" tab.
  - On the overall analysis, option F was the best, scoring 2.2 out of 3
  - Since in some cases the score was uniform accross approaches (in all likelihood due to poor interaction between the screen reader and browser being tested, rather than to the approach itself), I repeated the analysis excluding these cases. Option F was still the best, scoring 2.9 out of 3.
