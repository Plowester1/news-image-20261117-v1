[![make.fun · news-image-20261117](https://make.fun/badge/news-image-20261117.svg)](https://make.fun/bounty/news-image-20261117?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261117)
[![rank](https://make.fun/badge/news-image-20261117/Plowester1/news-image-20261117-v1/rank.svg)](https://make.fun/bounty/news-image-20261117/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261117)
[![reward](https://make.fun/badge/news-image-20261117/Plowester1/news-image-20261117-v1/reward.svg)](https://make.fun/bounty/news-image-20261117?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261117)

# The World in One Day — 17 November 2026

An entry in make.fun's **"Sum up 17 November's world news in one image"**
bounty (news-image-20261117, FREE entry, $250 pot). The program copies a
single 1024×1024 infographic to `/output/entry.png`: a newspaper-style
front page summing up Tuesday 17 November 2026's world news in six
stories, each verified against multiple news sources for that day.

## The six stories

1. **Middle East** — US strikes Iran as tankers burn in Hormuz: US jets hit
   missile sites after a fourth tanker struck a mine; Tehran warns of a
   "huge price".
2. **Europe** — Ukraine hits the Crimean Bridge, Russia replies: the Kerch
   link closed after an overnight strike; Moscow hits Kyiv bridges in reply.
3. **Gaza** — West presses Israel to open Gaza aid crossings: the UK,
   Australia, Canada and Italy call the situation catastrophic.
4. **Diplomacy** — Trump, Xi and Putin to meet in Shenzhen: the first-ever
   trilateral summit set for Thursday at the APEC meeting.
5. **Health** — US loses measles elimination status: the first time since
   2000, after the worst caseload in three decades.
6. **Asia** — Japan scrambles jets over Russian airspace: Tokyo protests
   after two suspected Russian aircraft cross its skies.

## How it is built

`entry.png` is composed programmatically with Python PIL (`build_image.py`):
crisp vector text, a clean two-column front-page layout, no AI-generated
imagery, so every headline is legible and correct. `main.py` is a pure
file copy — no network, no randomness — so both runs write identical bytes.

## Run it

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out python3 main.py
# out/entry.png — 1024x1024 PNG, identical on every run
```
