# Design direction

Minecraft: The Other Update begins with Minecraft Java Edition 1.0.0 and follows an alternative update history.

The project is not intended to backport modern Minecraft feature by feature. New content should feel like a plausible continuation of early Release Minecraft while still allowing larger mechanical and progression changes.

## Principles

- Preserve the readable, restrained style of early Release Minecraft
- Prefer features with a clear gameplay purpose
- Integrate additions into survival progression
- Avoid complexity that does not improve the core experience
- Keep new art compatible with the original low-resolution visual language
- Treat existing mechanics as open to revision when the result fits the project

## First feature: sleeping progression

The first gameplay feature is an adaptation of Beds, but Endgame for Minecraft 1.0.

Planned behavior:

- A Bedside Table must be placed beside the head of a bed before the player can sleep
- Using an invalid bed still sets the player's respawn point
- A Glowstone Lantern can protect the sleeping setup
- Sleeping without protection can trigger a nightmare

The first implementation will focus on the complete core loop before adding variants, configuration interfaces or additional decorative functions.

## Engine polish

Legacy engine issues may be corrected when they noticeably affect the project.

One tracked example is the thin color seam visible between strips of extruded held-item models. This should be investigated after the initial modification and patch workflow is stable.
