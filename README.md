# Family Zoo — v11 — Non-Player Characters

A patrolling zookeeper and a chatty parrot bring the zoo to life. Walks through the three-part NPC system — trait, behavior, plugin — and how to write custom behavior reactions.

Step 11 of the [Family Zoo](https://github.com/Johnesco/familyzoo) tutorial — a progressive walkthrough of the [Sharpee](https://sharpee.net) TypeScript interactive fiction engine, from a single room to a full multi-file story.

## What this step teaches

- NpcTrait, ActorTrait with isPlayer false, and the NpcPlugin
- Built-in behaviors: patrol, wanderer, follower, guard, passive
- Custom NpcBehavior implementations with onTurn and onPlayerEnters hooks
- NpcAction types: move, speak, emote, wait, take, drop
- NpcContext giving behaviors access to world, npc, and player state

## Playing

Open `play.html`, or preview the folder:

```bash
python -m http.server 8000 --directory familyzoo-v11
```

## Building

This is a **frozen 0.9.x TypeScript version**. The built player in this folder is the published artifact; it is re-laid from `browser/` by the workspace build:

```bash
python ../tools/build.py familyzoo-v11
python C:/code/ifhub/tools/ship.py familyzoo-v11
```

The authoring tree for every version lives in the [familyzoo](https://github.com/Johnesco/familyzoo) repo.
