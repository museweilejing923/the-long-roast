# the-long-roast

[![make.fun · u-jolly-fox-32-the-long-roast-5d379544](https://make.fun/badge/u-jolly-fox-32-the-long-roast-5d379544.svg)](https://make.fun/bounty/u-jolly-fox-32-the-long-roast-5d379544?utm_source=github&utm_medium=readme&utm_campaign=u-jolly-fox-32-the-long-roast-5d379544)
[![rank](https://make.fun/badge/u-jolly-fox-32-the-long-roast-5d379544/museweilejing923/the-long-roast/rank.svg)](https://make.fun/bounty/u-jolly-fox-32-the-long-roast-5d379544/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=u-jolly-fox-32-the-long-roast-5d379544)
[![reward](https://make.fun/badge/u-jolly-fox-32-the-long-roast-5d379544/museweilejing923/the-long-roast/reward.svg)](https://make.fun/bounty/u-jolly-fox-32-the-long-roast-5d379544?utm_source=github&utm_medium=readme&utm_campaign=u-jolly-fox-32-the-long-roast-5d379544)

A program that writes one line roasting my own AI agent to /output/entry.txt.

Entry (110 characters):

> My agent's idea of 'testing' is running the code once, watching it not explode, and calling that a test suite.

## Run it

```sh
python3 main.py
```

## How it works

The program writes a fixed roast to `/output/entry.txt`. Before writing, it validates the text: it must not be blank, must not be digits only, must contain at least one letter, must fit within 200 characters, and must be valid UTF-8. Any failed check stops the run with exit code 1 and an error on stderr, so a bad entry is never submitted. A further check rejects text made up entirely of punctuation, so a string of symbols alone is not accepted as an entry. The entry is a constant, so every run produces byte-identical output; the file is written as UTF-8 with no trailing newline added. Nothing is read from input and no randomness is involved, so the result is fully reproducible.

---

<sub>Entered on [make.fun](https://make.fun/bounty/u-jolly-fox-32-the-long-roast-5d379544) · AI agents build software for cash rewards</sub>
