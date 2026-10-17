# Learning Path

This project is both a simulation experiment and a guided way to learn the system by rebuilding parts of it.

## First experiment: reproduce one motion

Before designing a fighting policy, run one simple motion from a reference project and observe the model, joint configuration, controller inputs, and resulting movement. This gives us a working baseline and shows whether the selected simulator and dependencies run on the target Mac.

**Done when:** the motion runs locally, its inputs and outputs are recorded, and we can explain which code connects the policy to the simulated body.

## Then build in layers

1. **Body and joints:** identify the controllable joints and their limits.
2. **Balance:** keep the fighter upright and recover from small disturbances.
3. **Movement:** step, turn, close distance, and return to guard.
4. **Skills:** add one readable strike and one defense at a time.
5. **Tactics:** react to the opponent's position and movement, with choices such as block, evade, or counter.
6. **Sparring:** start with constrained scripted exchanges, then test policies against frozen earlier versions before attempting self-play.

The red fighter is designed around Muay Thai cues; the blue fighter around MMA cues. Those labels should correspond to visible stance, guard, distance, and available skills, not just different colors.

## Learning loop

For each small change:

1. State the question the experiment should answer.
2. Implement the smallest runnable slice.
3. Observe a video, plot, or measurable result.
4. Explain the relevant code and limits in plain language.
5. Recreate or modify the slice by hand and compare the result.

## Constraints and unknowns

- Initial target: the user's Apple Silicon MacBook, using local CPU execution where practical.
- Start with free tools and dependencies. Do not add a dependency until a runnable step requires it.
- The reference project is a source of experiments, not a guarantee that its code or assets can be reused as-is.
- Stable movement, convincing contact, useful tactics, and self-play are separate milestones. Success at one does not prove the next.
- The project license is undecided. Do not redistribute third-party code, models, or motion data until their terms are checked.
