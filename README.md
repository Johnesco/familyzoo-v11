# Family Zoo — v11: Characters

Sam the zookeeper. A person is created like anything else, but carries conversation and reacts to the player being in the room.

Step 11 of sixteen in the [Family Zoo](https://github.com/Johnesco/familyzoo) tutorial for [Chord](https://sharpee.net/chord/), the authoring language of the [Sharpee](https://sharpee.net) interactive fiction engine.

## What this step adds

- `a person` and where they stand
- `on the player talking to` for conversation
- Describing someone doing something, not just standing there
- Why the room description mentions them separately

## The source

The whole step is one file: [`familyzoo-v11.story`](./familyzoo-v11.story) — the step before it plus the ideas above. The chapter that walks through it is [`docs/v11-characters.md`](./docs/v11-characters.md).

## Playing and testing

```bash
npx sharpee play
npx sharpee test          # replays familyzoo-v11.tests.json
python ../tools/build.py familyzoo-v11 --force
```

## Engine

Pinned to `@sharpee/*` **5.3.0** (Chord 3.6.0), held there by an `overrides` block: 5.3.1 publishes broken subpath exports and breaks `sharpee test`.

The 0.9.x TypeScript edition this replaced is kept in [`legacy/`](./legacy).
