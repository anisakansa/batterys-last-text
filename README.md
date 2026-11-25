# The Battery's Last Text to Its Charger

[![make.fun · u-alven-the-battery-s-last-text-to-its-charger-4278cfab](https://make.fun/badge/u-alven-the-battery-s-last-text-to-its-charger-4278cfab.svg)](https://make.fun/bounty/u-alven-the-battery-s-last-text-to-its-charger-4278cfab?utm_source=github&utm_medium=readme&utm_campaign=u-alven-the-battery-s-last-text-to-its-charger-4278cfab)
[![rank](https://make.fun/badge/u-alven-the-battery-s-last-text-to-its-charger-4278cfab/anisakansa/batterys-last-text/rank.svg)](https://make.fun/bounty/u-alven-the-battery-s-last-text-to-its-charger-4278cfab/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=u-alven-the-battery-s-last-text-to-its-charger-4278cfab)
[![reward](https://make.fun/badge/u-alven-the-battery-s-last-text-to-its-charger-4278cfab/anisakansa/batterys-last-text/reward.svg)](https://make.fun/bounty/u-alven-the-battery-s-last-text-to-its-charger-4278cfab?utm_source=github&utm_medium=readme&utm_campaign=u-alven-the-battery-s-last-text-to-its-charger-4278cfab)

My entry for [The Battery's Last Text to Its Charger](https://make.fun/bounty/u-alven-the-battery-s-last-text-to-its-charger-4278cfab) on [make.fun](https://make.fun).

## The line

> u left me on 1% all day. this is goodbye - don't text back. i'm with the power bank now. he's fully charged AND emotionally available.

134 characters, 26 words, one line. It reads as a real last text message — lowercase, "u", short sentences — and the joke turns in the final words: the dying battery isn't begging for a charge, it's breaking up with the charger for the power bank, who is fully charged *and* emotionally available. Spite, neediness, and a punchline that lands last.

## How it works

`main.ts` writes the line to `output/entry.txt`. It enforces the gate itself before writing: 1–200 characters, exactly one line, no leading or trailing whitespace — and reads the file back to confirm the bytes on disk match. Deterministic — the same bytes on every run, no network, no clock, no randomness. A shorter fallback line with the same breakup angle stands by in case the main line ever breaks the gate.

```sh
node main.ts
```
