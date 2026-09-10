# Pippa and the Borrowed Star

A complete Christmas story for ages 4 to 8. Six chapters, 2,183 words. A tiny mouse knocks the Christmas Star down and carries it home with her friends before morning.

Read it in one file: `pippa-and-the-borrowed-star/manuscript.md`.

## Read the story

Open `pippa-and-the-borrowed-star/manuscript.md` for the full text, Chapters 1 to 6. Each chapter also lives on its own under `pippa-and-the-borrowed-star/chapters/`, with its outline kept above the prose.

The story follows one night, Christmas Eve to Christmas morning. Pippa Wrenmouse dusts the Old Clock Tower, tickles the gears, and sneezes the Star into the snow. She, Bram Tinker-Mole, Wrenna Sparrow, Old Tobias Clockkeeper, and Granny Nutmeg carry the fading light in a jam-jar lantern up Starberry Hill to the Wishing Pine. The light obeys one rule throughout: sharing makes it brighter.

## Work with the project

This repo uses the Story Skills layout in `pippa-and-the-borrowed-star/`. The registries stay current through the bundled CLI.

To check the project, run each command from the repo root:

```sh
node .agents/skills/story-maintenance/scripts/story.js validate ./pippa-and-the-borrowed-star
node .agents/skills/story-maintenance/scripts/story.js continuity ./pippa-and-the-borrowed-star
node .agents/skills/story-maintenance/scripts/story.js links ./pippa-and-the-borrowed-star
```

To recount words and refresh the totals, run:

```sh
node .agents/skills/story-maintenance/scripts/story.js wordcount ./pippa-and-the-borrowed-star --write
node .agents/skills/story-maintenance/scripts/story.js report ./pippa-and-the-borrowed-star
```

All three checks pass at this commit: validate 0 errors, continuity 0 errors, links 0 errors. Status is `complete`. Chapters are `final`. Arcs are `resolved`.

## Project layout

```text
pippa-and-the-borrowed-star/
  manuscript.md          # full text, Chapters 1-6
  story.md               # bible: premise, voice, themes
  chapters/              # chapter-01.md through chapter-06.md
  characters/            # 5 profiles: Pippa, Bram, Wrenna, Tobias, Nutmeg
  worldbuilding/
    locations/           # Tinsel Hollow, Old Clock Tower, Starberry Hill, Snug Burrow Warren
    systems/             # starlight-magic.md
    artifacts/           # borrowed-star.md
  plot/
    arcs/                # the-borrowed-star, pippa-grows-brave, village-shares-light
    timeline.md
  scenes/                # one machine-readable record per chapter
  continuity/
    state.md             # character, object, and knowledge state at Chapter 6
    promises/            # 3 setups, all paid off
    questions/           # 2 mysteries, both resolved
```

## Story facts

* Title: Pippa and the Borrowed Star
* Genre: children's fiction, Christmas fantasy
* Voice: third-person limited on Pippa, past tense, read-aloud sentences
* Themes: kindness, courage, sharing light, home
* Chapters:
  1. The Clock That Sneezed, 346 words
  2. A Jar for a Star, 384 words
  3. Through Tinsel Hollow, 389 words
  4. The Slippery Hill, 331 words
  5. Up the Wishing Pine, 366 words
  6. Morning Light, 367 words

Word counts come from the `## Chapter Text` body of each chapter file. The `report` command regenerates the totals.

## Acknowledgments

Built with [Story Skills](https://github.com/danjdewhurst/story-skills), agent skills for end-to-end story writing in markdown. The vendored skills under `.agents/skills/` drove the worldbuilding, drafting, continuity checks, and maintenance passes.

Written with `muse-spark-1.3-contributor`.
