# Development Roadmap

## Goal

Turn the campaign into a real game gradually, proving one difficult system at a time.

## Phase 0 — Repository + live text campaign

**Now.**

Goals:
- lock design principles;
- play the campaign in chat;
- record state;
- observe what decisions are actually fun;
- refine the Wayfarer;
- collect edge cases for combat and magic.

Deliverables:
- docs;
- campaign state;
- play log;
- acceptance tests derived from play.

## Phase 1 — Deterministic CLI prototype

Build:
- character state;
- inventory;
- locations;
- travel/time;
- d20 resolution;
- HP/wounds/death;
- basic enemy behavior;
- save/load;
- three Wayfarer systems: Waymark, Vector Knot, simple stored momentum.

No graphics.

Success criteria:
- the same scenario can be replayed with different decisions;
- state is inspectable;
- death and wounds persist;
- tests can reproduce outcomes with seeded randomness.

## Phase 2 — Small browser game

Add:
- readable combat UI;
- map/room geometry;
- inventory UI;
- skill progress panel;
- event log;
- clickable actions plus free-text/advanced commands where useful.

Still use a tiny world.

## Phase 3 — High-skill combat simulation

Deepen:
- reach;
- facing;
- balance;
- commitment;
- recovery;
- stamina;
- wounds;
- shields;
- projectile travel;
- momentum transfer;
- terrain;
- enemy adaptation.

Create encounter tests specifically for expert play.

## Phase 4 — Persistent regional simulation

Add:
- NPC schedules/goals;
- economy-lite;
- factions;
- rumors;
- travel state;
- quest-worthy events caused by simulation;
- persistent building/location changes.

## Phase 5 — Spatial/3D prototype decision

Only after the text/browser combat is demonstrably fun, choose whether the project should:
- remain a deep text/isometric game;
- become a 2D tactical game;
- materialize into a 3D first-person/third-person combat game.

Do not choose the heaviest engine before the mechanical loop earns it.

## Phase 6 — Production

Only after a vertical slice:
- content pipeline;
- art direction;
- audio;
- accessibility;
- save compatibility;
- mod/data format;
- performance;
- packaging;
- distribution.

## Testing priorities

Every major mechanic should have:
- deterministic unit tests where possible;
- adversarial "can this be cheesed?" tests;
- save/load tests;
- failure-state tests;
- player-information tests;
- lethal encounter tests;
- "expert uses tiny effect creatively" tests.

## First coding milestone

A single fight in a muddy roadside clearing against one competent knife fighter.

The player can:
- inspect;
- move;
- guard;
- thrust;
- kick;
- retreat;
- place/use one Waymark;
- attempt a small Vector Knot.

The encounter must be winnable through skill, escapable, and lethal when played badly.
