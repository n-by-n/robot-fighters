# Robot Fighters Lab

A learning project about building two distinctive robot fighters and teaching them to spar in simulation.

The visual concept has two clear styles:

- **Red fighter:** Muay Thai inspired stance, guard, and strikes.
- **Blue fighter:** MMA inspired movement, defense, and combinations.

The goal is to make the exchange readable and intentional. A fighter should choose when to move, defend, or attack instead of producing random collisions. We will start in simulation and validate each small step before adding complexity.

## Current status

This repository is at the planning and setup stage. No working fight simulation or trained policy is included yet. The first technical milestone is to run and understand a minimal reference motion in a free, local setup on Apple Silicon, then decide which parts are practical to adapt.

## Learning approach

We will build in small pieces. Each piece should have an observable result, a short explanation of how it works, and a chance for the learner to rewrite or modify it by hand before moving on.

The intended progression is:

1. Inspect the reference humanoid, its joints, and its motion data.
2. Reproduce one reference movement and understand the simulation loop.
3. Map the visual robot designs onto controllable articulated bodies.
4. Build stable stance, footwork, guard, and individual strikes.
5. Add tactical choices such as blocking, evading, and countering.
6. Let the fighters spar, first against scripted behavior and later through self-play.

This is a direction, not a promise that every stage will work unchanged. Hardware performance, model compatibility, and motion quality need experiments.

## Development

The initial target is macOS on Apple Silicon. Use Python 3.12 in an isolated environment. The starter setup intentionally has no third-party dependencies; we will add a free dependency only when a verified step needs it.

```bash
python3.12 -m venv .venv
source .venv/bin/activate
python --version
```

See [the learning path](docs/learning-path.md) for the staged experiments and what each one should teach.

## License and assets

The source license has not been selected yet. Reference repositories, motion data, robot artwork, and other third-party assets will be tracked separately with their terms checked before reuse or redistribution.
