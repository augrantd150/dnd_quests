# Repository Agent Rules

These instructions apply to humans and coding agents working in this repository.

## Authority order

1. Explicit current user instruction.
2. This repository's design docs.
3. Current Augrant design principles where referenced.
4. SRD 5.2.1 for any 5E-compatible material.
5. Implementation convenience.

Implementation must not silently override higher-authority design rules.

## Non-negotiables

- The game is a **solo-first, dark-medieval, high-skill RPG**.
- Death must be genuinely possible.
- Do not secretly scale threats down to preserve the player.
- Lethality must be paired with readable evidence and fair causality.
- Player mastery and character mastery both matter.
- Magic must have mechanisms, costs, requirements, limits, counterplay, and failure behavior.
- Avoid canned "press button to win" spell design when a composable systemic effect can work.
- Progress comes primarily from meaningful use, deliberate practice, instruction, study, difficult work, and informative failure.
- Trivial repetition must not grant unlimited advancement.
- Persistent consequences are canonical.
- Do not copy proprietary characters, names, lore, text, or audiovisual assets from other games.
- League of Legends' Bard is a **design reference for mastery structure**, not a content source to reproduce.

## Engineering direction

Prefer:
- deterministic simulations where practical;
- explicit state;
- save/load stability;
- data-driven rules;
- testable resolution;
- small vertical slices;
- useful debug visibility.

Avoid:
- hidden rubber-banding;
- unlogged state changes;
- random outcomes that ignore established causes;
- content generation that rewrites established world facts;
- large frameworks before the core loop is proven.

## First implementation target

A command-line or simple browser combat/exploration prototype with:
- one player character;
- one small region;
- persistent state;
- turn-based or time-sliced combat;
- terrain/position;
- wounds and death;
- the first Wayfarer techniques;
- visible skill progress;
- deterministic save/load.
