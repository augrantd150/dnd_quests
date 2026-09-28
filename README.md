# The Black Tithe

**Working title.** A lethal, high-skill, solo dark-medieval RPG that begins as a persistent text campaign and is intended to grow into a real game.

The project combines:

- a 5E-compatible rules chassis derived only from **SRD 5.2.1** when D&D-derived mechanics are used;
- **Augrant's causal-magic philosophy**: magic changes the same physical world as everything else and must have causes, requirements, limits, resistance, and failure states;
- **visible, use-based progression** rather than grindable global XP as the main source of mastery;
- a world that does not scale itself to the player;
- combat where information, positioning, preparation, terrain, timing, retreat, and resource control matter;
- an original high-skill wandering magic archetype inspired by the *design principles* that make League of Legends' Bard expressive, without cloning Bard's lore, names, or exact kit.

## Current status

**Phase 0 — playable design foundation.**

This repository currently holds the authoritative design contract and campaign state. The first playable implementation should be a small deterministic text/CLI prototype, not a giant engine.

## Core promise

> The game will kill a careless character, but it should rarely kill an attentive player without giving them information they could have acted on.

Death is possible. Plot armor is not.

Difficulty should come from reading the situation, making hard choices, spending limited resources, using geometry and causal magic well, and knowing when not to fight.

## Project map

- `docs/DESIGN_PILLARS.md` — non-negotiable design principles
- `docs/RULES_CORE.md` — base resolution and lethal-combat contract
- `docs/MAGIC_SYSTEM.md` — Augrant-derived causal magic
- `docs/PROGRESSION.md` — visible use/practice/instruction progression
- `docs/WAYFARER_ARCHETYPE.md` — original weird/high-ceiling player archetype
- `docs/WORLD.md` — dark-medieval setting direction
- `docs/DEVELOPMENT_ROADMAP.md` — path from chat campaign to real game
- `docs/SOURCES_AND_LICENSES.md` — external references and licensing notes
- `campaigns/state.json` — current canonical campaign state
- `campaigns/play-log.md` — append-only play history

## Relationship to Augrant

AUGRANT remains the upstream design source for causal magic and the philosophy that meaningful use, deliberate practice, instruction, difficult work, and informative failure drive skill development.

This project may simplify those ideas for a focused dark-medieval solo RPG, but it must not silently replace them with arbitrary spell effects or grindable skill spam.

## Design rule for future implementation

Build the smallest thing that proves the next piece of play is fun.

Do not start with multiplayer, a giant open world, hundreds of spells, or content volume. First prove:

1. fair lethal combat;
2. readable danger;
3. weird systemic magic;
4. visible progression;
5. persistent consequences;
6. a high-skill player kit that supports many solutions.
