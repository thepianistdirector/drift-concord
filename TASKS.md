# Drift Concord: proposed work packages

These are planning briefs. No task is complete or approved for automatic execution. Before implementation, maintainers must publish a scoped task revision with the actual repository, paths, tools and validation commands.

## W1-T1 — Script the derelict expedition

**Wave:** W1 · **Status:** Planned · **Prerequisites:** None; begin with maintainer scope review

Define preparation, discovery, salvage, a recoverable failure and the return home.

Start only after the listed prerequisites and scope are accepted by a maintainer. Work in the project's own repository. Document assumptions, unresolved questions and reproducible evidence. This is a proposed work package, not a claim that the implementation already exists.

Acceptance criteria:

- The mission includes a consequential decision for pilot, engineer and field crew.
- Document an alternate route to completion after one crew member disconnects.

## W1-T2 — Prototype physical crew interactions

**Wave:** W1 · **Status:** Planned · **Prerequisites:** W1-T1

Test piloting, power rerouting and handling salvage with minimal presentation.

Start only after the listed prerequisites and scope are accepted by a maintainer. Work in the project's own repository. Document assumptions, unresolved questions and reproducible evidence. This is a proposed work package, not a claim that the implementation already exists.

Acceptance criteria:

- New players can perform each interaction with visible feedback and remappable controls.
- A small group reports where coordination is enjoyable and where a role is idle.

## W2-T1 — Implement the ship systems model

**Wave:** W2 · **Status:** Planned · **Prerequisites:** W1-T1, W1-T2

Connect power, propulsion, doors and damage through explicit state and limits.

Start only after the listed prerequisites and scope are accepted by a maintainer. Work in the project's own repository. Document assumptions, unresolved questions and reproducible evidence. This is a proposed work package, not a claim that the implementation already exists.

Acceptance criteria:

- Recorded input sequences replay to the same authoritative system state.
- A broken subsystem has a visible diagnosis and a bounded recovery path.

## W2-T2 — Implement shared movement and objects

**Wave:** W2 · **Status:** Planned · **Prerequisites:** W1-T1, W1-T2

Synchronize players and portable cargo in and around one moving ship.

Start only after the listed prerequisites and scope are accepted by a maintainer. Work in the project's own repository. Document assumptions, unresolved questions and reproducible evidence. This is a proposed work package, not a claim that the implementation already exists.

Acceptance criteria:

- Cargo ownership and position remain consistent through boarding, docking and reconnect.
- Test interaction latency and collision behavior on documented network conditions.

## W3-T1 — Build the derelict and salvage objective

**Wave:** W3 · **Status:** Planned · **Prerequisites:** W2-T1, W2-T2

Author one readable destination with meaningful navigation and cargo choices.

Start only after the listed prerequisites and scope are accepted by a maintainer. Work in the project's own repository. Document assumptions, unresolved questions and reproducible evidence. This is a proposed work package, not a claim that the implementation already exists.

Acceptance criteria:

- The expedition has a complete start, salvage decision, return and debrief.
- Recoverable failures change the mission without silently deleting the crew's progress.

## W3-T2 — Run first-crew playtests

**Wave:** W3 · **Status:** Planned · **Prerequisites:** W2-T1, W2-T2

Observe complete expeditions by groups unfamiliar with the design.

Start only after the listed prerequisites and scope are accepted by a maintainer. Work in the project's own repository. Document assumptions, unresolved questions and reproducible evidence. This is a proposed work package, not a claim that the implementation already exists.

Acceptance criteria:

- Measure role downtime, onboarding failures and whether crews want another mission.
- Publish a prioritized revision of the mission based on observed play.

## W4-T1 — Persist the ship and expedition journal

**Wave:** W4 · **Status:** Planned · **Prerequisites:** W3-T1, W3-T2

Save configuration, cargo and completed expedition events with recoverable migrations.

Start only after the listed prerequisites and scope are accepted by a maintainer. Work in the project's own repository. Document assumptions, unresolved questions and reproducible evidence. This is a proposed work package, not a claim that the implementation already exists.

Acceptance criteria:

- A restarted server restores the ship and identifies incompatible content versions.
- A crew can export its ship history without exposing private account data.

## W4-T2 — Build the expedition authoring kit

**Wave:** W4 · **Status:** Planned · **Prerequisites:** W3-T1, W3-T2

Describe locations, hazards, objectives and outcomes as inspectable mission packages.

Start only after the listed prerequisites and scope are accepted by a maintainer. Work in the project's own repository. Document assumptions, unresolved questions and reproducible evidence. This is a proposed work package, not a claim that the implementation already exists.

Acceptance criteria:

- A contributor authors a second expedition without modifying core ship simulation.
- Malformed or malicious package inputs fail before affecting a persistent ship.

## W5-T1 — Package community hosting and moderation

**Wave:** W5 · **Status:** Planned · **Prerequisites:** W4-T1, W4-T2

Deliver host setup, access control, logs and a documented recovery procedure.

Start only after the listed prerequisites and scope are accepted by a maintainer. Work in the project's own repository. Document assumptions, unresolved questions and reproducible evidence. This is a proposed work package, not a claim that the implementation already exists.

Acceptance criteria:

- A second operator hosts a complete expedition from the documentation.
- Test abusive joins, role permissions, removal and recovery without giving moderators hidden player advantage.

## W5-T2 — Prototype explicit sector handoff

**Wave:** W5 · **Status:** Planned · **Prerequisites:** W4-T1, W4-T2

Design and test ownership transfer between two cooperating sector servers.

Start only after the listed prerequisites and scope are accepted by a maintainer. Work in the project's own repository. Document assumptions, unresolved questions and reproducible evidence. This is a proposed work package, not a claim that the implementation already exists.

Acceptance criteria:

- A failed handoff leaves ship and cargo owned in exactly one recoverable location.
- Players see connection and trust boundaries before transferring.

## W6-T1 — Build a varied expedition pilot

**Wave:** W6 · **Status:** Planned · **Prerequisites:** W5-T1, W5-T2

Add a bounded set of exploration, rescue and engineering missions using the kit.

Start only after the listed prerequisites and scope are accepted by a maintainer. Work in the project's own repository. Document assumptions, unresolved questions and reproducible evidence. This is a proposed work package, not a claim that the implementation already exists.

Acceptance criteria:

- Each mission offers a different crew decision instead of only changing scenery.
- Mixed-experience groups can complete the mission set and report meaningful role choice.

## W6-T2 — Publish performance and operations findings

**Wave:** W6 · **Status:** Planned · **Prerequisites:** W5-T1, W5-T2

Measure client performance, supported crew sizes, restoration and content moderation effort.

Start only after the listed prerequisites and scope are accepted by a maintainer. Work in the project's own repository. Document assumptions, unresolved questions and reproducible evidence. This is a proposed work package, not a claim that the implementation already exists.

Acceptance criteria:

- Results name hardware, network conditions and mission complexity.
- Set the next capacity target from measured constraints rather than a galaxy-sized launch promise.
