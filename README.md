# Family Zoo — v11: Characters

Sam the zookeeper. A person is created like anything else, but carries conversation and reacts to the player being in the room.

Step 11 of sixteen in the [Family Zoo](https://github.com/Johnesco/familyzoo) tutorial for [Chord](https://sharpee.net/chord/), the authoring language of the [Sharpee](https://sharpee.net) interactive fiction engine.

## What this step adds

- `a person` and where they stand
- `on the player talking to` for conversation
- Describing someone doing something, not just standing there
- Why the room description mentions them separately

## The source

The whole step is one file: [`familyzoo-v11.story`](./familyzoo-v11.story) — the step before it plus the ideas above. Where it sits in the trail is on the [group page](https://johnesco.github.io/familyzoo/#familyzoo-v11).

## Playing and testing

```bash
npx sharpee play
npx sharpee test          # replays familyzoo-v11.tests/
python ../tools/build.py familyzoo-v11 --force
```

## Engine

Pinned in `package.json`, held across the whole `@sharpee/*` scope by an `overrides` block.

The 0.9.x TypeScript edition this replaced is kept in [`legacy/`](./legacy).
