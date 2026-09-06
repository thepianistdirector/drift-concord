# Drift Concord: task contracts

Twelve proposed work packages, with named waves and dependency order. None is completed by publishing this document. The linked Tanduna revision is the contribution authority; this repository records the maintainer's intended contract while Tanduna's structured requirement support is being updated.

Every task below names its repository, branch, verified planning commit, preferred model, allowed fallback, immutable public skills, task-specific testing procedure and maintainer acceptance flow. A later implementation task still needs its prerequisite code, a rebased execution revision, narrow file scope and real functional commands. Do not treat the current planning commit as if that future code exists.

The allowed model pair is GPT-6 Astra and Claude Fable 5.1, with the effort stated per task. A model declaration is not independent runtime evidence; unresolved proof remains visible to the maintainer. See [CONTRIBUTING.md](CONTRIBUTING.md) and [the machine-readable authored contracts](task-contracts.json).

## W1-T1 — Script the derelict expedition

**Wave:** W1 · **Prerequisites:** None; maintainer scope review first

Define preparation, discovery, salvage, a recoverable failure and the return home.

**Saved Tanduna task:** [W1-T1](https://tanduna.com/p/drift-concord/tasks/tsk_9259b242523e66a821f72e1be773d4ec)

**Repository:** [https://github.com/thepianistdirector/drift-concord](https://github.com/thepianistdirector/drift-concord) · **Branch:** `main`

**Planning base commit:** [`4554bc5fae2cd33a0da369b0fc288f62c8c0a881`](https://github.com/thepianistdirector/drift-concord/commit/4554bc5fae2cd33a0da369b0fc288f62c8c0a881)

**Execution gate:** Maintainer accepts the scoped design protocol; this is not product implementation.

**Preferred:** `gpt-6-astra` / medium. **Accepted fallback:** `claude-fable-5-1` / medium. Other models require a maintainer revision before work.

**Required skills:** [contribution protocol](https://raw.githubusercontent.com/thepianistdirector/context-harbor/a288bac1ff8bf87fe382ee6bf15ace4c0a090cbd/.agents/skills/tanduna-contribution/SKILL.md) and [Drift Concord validation](https://raw.githubusercontent.com/thepianistdirector/drift-concord/4554bc5fae2cd33a0da369b0fc288f62c8c0a881/.agents/skills/drift-concord-validation/SKILL.md), at the linked immutable versions.

### Acceptance criteria

- The mission includes a consequential decision for pilot, engineer and field crew.
- Document an alternate route to completion after one crew member disconnects.

### Testing procedure

Walk the derelict expedition from embarkation through salvage and return with four crew roles. Rehearse missing crew and a failed objective; document useful decisions, coordination points and a recoverable ending.

Record setup/fixtures, actions, expected and observed results, relevant logs or artifacts, and PASS / FAIL / NOT RUN for each criterion.

Existing baseline checks (repository root; identity and patch hygiene only):

```sh
git rev-parse HEAD
git status --short
git diff --check 4554bc5fae2cd33a0da369b0fc288f62c8c0a881
```

This task uses the saved reproducible manual protocol. Distinguish paper/synthetic exercises from actual participant or physical observations.

**Evidence artifact:** `docs/work/W1-T1/acceptance.md` plus the actual patch, fixtures and logs within the approved task scope.

### Acceptance workflow

1. Contributor identifies the saved Tanduna task revision, repository/base, accepted prerequisites, selected primary or fallback model and effort, and exact required skill versions.
2. Contributor performs the task-specific testing procedure and maps each original acceptance criterion to setup, expected result, observed result and reproducible evidence. Failed and unrun checks remain visible.
3. Maintainer reproduces the material checks, reviews the scoped patch or design artifact and verifies the stated model/skill evidence. Unsupported model claims or missing evidence remain unresolved rather than accepted automatically.
4. Maintainer records acceptance or requested changes against the reviewed revision. A passing format check, generated patch or completed model invocation does not by itself satisfy the task.

## W1-T2 — Prototype physical crew interactions

**Wave:** W1 · **Prerequisites:** W1-T1

Test piloting, power rerouting and handling salvage with minimal presentation.

**Saved Tanduna task:** [W1-T2](https://tanduna.com/p/drift-concord/tasks/tsk_2c17dabbd3fe6cfd158d43fd89ee3f1a)

**Repository:** [https://github.com/thepianistdirector/drift-concord](https://github.com/thepianistdirector/drift-concord) · **Branch:** `main`

**Planning base commit:** [`4554bc5fae2cd33a0da369b0fc288f62c8c0a881`](https://github.com/thepianistdirector/drift-concord/commit/4554bc5fae2cd33a0da369b0fc288f62c8c0a881)

**Execution gate:** Prerequisite results must be accepted and integrated. Maintainer publishes a new task revision against that integrated base before execution; runtime work also needs the real harness and exact allowed paths.

**Preferred:** `gpt-6-astra` / high. **Accepted fallback:** `claude-fable-5-1` / high. Other models require a maintainer revision before work.

**Required skills:** [contribution protocol](https://raw.githubusercontent.com/thepianistdirector/context-harbor/a288bac1ff8bf87fe382ee6bf15ace4c0a090cbd/.agents/skills/tanduna-contribution/SKILL.md) and [Drift Concord validation](https://raw.githubusercontent.com/thepianistdirector/drift-concord/4554bc5fae2cd33a0da369b0fc288f62c8c0a881/.agents/skills/drift-concord-validation/SKILL.md), at the linked immutable versions.

### Acceptance criteria

- New players can perform each interaction with visible feedback and remappable controls.
- A small group reports where coordination is enjoyable and where a role is idle.

### Testing procedure

Use a small physical interaction prototype to pick up, hand over, attach and release objects. Repeat with two actors reaching for the same object and one disconnecting; record ownership and usability failures.

Record setup/fixtures, actions, expected and observed results, relevant logs or artifacts, and PASS / FAIL / NOT RUN for each criterion.

Existing baseline checks (repository root; identity and patch hygiene only):

```sh
git rev-parse HEAD
git status --short
git diff --check 4554bc5fae2cd33a0da369b0fc288f62c8c0a881
```

Exact functional commands, fixtures and paths must be ratified in the execution revision once the prerequisite-selected stack/harness exists. Do not claim these future checks ran.

**Evidence artifact:** `docs/work/W1-T2/acceptance.md` plus the actual patch, fixtures and logs within the approved task scope.

### Acceptance workflow

1. Contributor identifies the saved Tanduna task revision, repository/base, accepted prerequisites, selected primary or fallback model and effort, and exact required skill versions.
2. Contributor performs the task-specific testing procedure and maps each original acceptance criterion to setup, expected result, observed result and reproducible evidence. Failed and unrun checks remain visible.
3. Maintainer reproduces the material checks, reviews the scoped patch or design artifact and verifies the stated model/skill evidence. Unsupported model claims or missing evidence remain unresolved rather than accepted automatically.
4. Maintainer records acceptance or requested changes against the reviewed revision. A passing format check, generated patch or completed model invocation does not by itself satisfy the task.

## W2-T1 — Implement the ship systems model

**Wave:** W2 · **Prerequisites:** W1-T1, W1-T2

Connect power, propulsion, doors and damage through explicit state and limits.

**Saved Tanduna task:** [W2-T1](https://tanduna.com/p/drift-concord/tasks/tsk_aa6b588a7fd0addb66cc4fa689394865)

**Repository:** [https://github.com/thepianistdirector/drift-concord](https://github.com/thepianistdirector/drift-concord) · **Branch:** `main`

**Planning base commit:** [`4554bc5fae2cd33a0da369b0fc288f62c8c0a881`](https://github.com/thepianistdirector/drift-concord/commit/4554bc5fae2cd33a0da369b0fc288f62c8c0a881)

**Execution gate:** Prerequisite results must be accepted and integrated. Maintainer publishes a new task revision against that integrated base before execution; runtime work also needs the real harness and exact allowed paths.

**Preferred:** `gpt-6-astra` / high. **Accepted fallback:** `claude-fable-5-1` / high. Other models require a maintainer revision before work.

**Required skills:** [contribution protocol](https://raw.githubusercontent.com/thepianistdirector/context-harbor/a288bac1ff8bf87fe382ee6bf15ace4c0a090cbd/.agents/skills/tanduna-contribution/SKILL.md) and [Drift Concord validation](https://raw.githubusercontent.com/thepianistdirector/drift-concord/4554bc5fae2cd33a0da369b0fc288f62c8c0a881/.agents/skills/drift-concord-validation/SKILL.md), at the linked immutable versions.

### Acceptance criteria

- Recorded input sequences replay to the same authoritative system state.
- A broken subsystem has a visible diagnosis and a bounded recovery path.

### Testing procedure

Run fixed power, damage and repair sequences, interrupt one repair and repeat its request. Compare subsystem state and consumed resources with the agreed ship-system rules.

Record setup/fixtures, actions, expected and observed results, relevant logs or artifacts, and PASS / FAIL / NOT RUN for each criterion.

Existing baseline checks (repository root; identity and patch hygiene only):

```sh
git rev-parse HEAD
git status --short
git diff --check 4554bc5fae2cd33a0da369b0fc288f62c8c0a881
```

Exact functional commands, fixtures and paths must be ratified in the execution revision once the prerequisite-selected stack/harness exists. Do not claim these future checks ran.

**Evidence artifact:** `docs/work/W2-T1/acceptance.md` plus the actual patch, fixtures and logs within the approved task scope.

### Acceptance workflow

1. Contributor identifies the saved Tanduna task revision, repository/base, accepted prerequisites, selected primary or fallback model and effort, and exact required skill versions.
2. Contributor performs the task-specific testing procedure and maps each original acceptance criterion to setup, expected result, observed result and reproducible evidence. Failed and unrun checks remain visible.
3. Maintainer reproduces the material checks, reviews the scoped patch or design artifact and verifies the stated model/skill evidence. Unsupported model claims or missing evidence remain unresolved rather than accepted automatically.
4. Maintainer records acceptance or requested changes against the reviewed revision. A passing format check, generated patch or completed model invocation does not by itself satisfy the task.

## W2-T2 — Implement shared movement and objects

**Wave:** W2 · **Prerequisites:** W1-T1, W1-T2

Synchronize players and portable cargo in and around one moving ship.

**Saved Tanduna task:** [W2-T2](https://tanduna.com/p/drift-concord/tasks/tsk_d9e28118f2dac98fb87e8af334f13de7)

**Repository:** [https://github.com/thepianistdirector/drift-concord](https://github.com/thepianistdirector/drift-concord) · **Branch:** `main`

**Planning base commit:** [`4554bc5fae2cd33a0da369b0fc288f62c8c0a881`](https://github.com/thepianistdirector/drift-concord/commit/4554bc5fae2cd33a0da369b0fc288f62c8c0a881)

**Execution gate:** Prerequisite results must be accepted and integrated. Maintainer publishes a new task revision against that integrated base before execution; runtime work also needs the real harness and exact allowed paths.

**Preferred:** `gpt-6-astra` / high. **Accepted fallback:** `claude-fable-5-1` / high. Other models require a maintainer revision before work.

**Required skills:** [contribution protocol](https://raw.githubusercontent.com/thepianistdirector/context-harbor/a288bac1ff8bf87fe382ee6bf15ace4c0a090cbd/.agents/skills/tanduna-contribution/SKILL.md) and [Drift Concord validation](https://raw.githubusercontent.com/thepianistdirector/drift-concord/4554bc5fae2cd33a0da369b0fc288f62c8c0a881/.agents/skills/drift-concord-validation/SKILL.md), at the linked immutable versions.

### Acceptance criteria

- Cargo ownership and position remain consistent through boarding, docking and reconnect.
- Test interaction latency and collision behavior on documented network conditions.

### Testing procedure

Control two clients independently while moving through the ship and manipulating shared objects. Add latency, competing grabs and reconnect; compare authoritative ownership and corrected positions.

Record setup/fixtures, actions, expected and observed results, relevant logs or artifacts, and PASS / FAIL / NOT RUN for each criterion.

Existing baseline checks (repository root; identity and patch hygiene only):

```sh
git rev-parse HEAD
git status --short
git diff --check 4554bc5fae2cd33a0da369b0fc288f62c8c0a881
```

Exact functional commands, fixtures and paths must be ratified in the execution revision once the prerequisite-selected stack/harness exists. Do not claim these future checks ran.

**Evidence artifact:** `docs/work/W2-T2/acceptance.md` plus the actual patch, fixtures and logs within the approved task scope.

### Acceptance workflow

1. Contributor identifies the saved Tanduna task revision, repository/base, accepted prerequisites, selected primary or fallback model and effort, and exact required skill versions.
2. Contributor performs the task-specific testing procedure and maps each original acceptance criterion to setup, expected result, observed result and reproducible evidence. Failed and unrun checks remain visible.
3. Maintainer reproduces the material checks, reviews the scoped patch or design artifact and verifies the stated model/skill evidence. Unsupported model claims or missing evidence remain unresolved rather than accepted automatically.
4. Maintainer records acceptance or requested changes against the reviewed revision. A passing format check, generated patch or completed model invocation does not by itself satisfy the task.

## W3-T1 — Build the derelict and salvage objective

**Wave:** W3 · **Prerequisites:** W2-T1, W2-T2

Author one readable destination with meaningful navigation and cargo choices.

**Saved Tanduna task:** [W3-T1](https://tanduna.com/p/drift-concord/tasks/tsk_6cd4ec3670859892b088588824c52ab6)

**Repository:** [https://github.com/thepianistdirector/drift-concord](https://github.com/thepianistdirector/drift-concord) · **Branch:** `main`

**Planning base commit:** [`4554bc5fae2cd33a0da369b0fc288f62c8c0a881`](https://github.com/thepianistdirector/drift-concord/commit/4554bc5fae2cd33a0da369b0fc288f62c8c0a881)

**Execution gate:** Prerequisite results must be accepted and integrated. Maintainer publishes a new task revision against that integrated base before execution; runtime work also needs the real harness and exact allowed paths.

**Preferred:** `gpt-6-astra` / high. **Accepted fallback:** `claude-fable-5-1` / high. Other models require a maintainer revision before work.

**Required skills:** [contribution protocol](https://raw.githubusercontent.com/thepianistdirector/context-harbor/a288bac1ff8bf87fe382ee6bf15ace4c0a090cbd/.agents/skills/tanduna-contribution/SKILL.md) and [Drift Concord validation](https://raw.githubusercontent.com/thepianistdirector/drift-concord/4554bc5fae2cd33a0da369b0fc288f62c8c0a881/.agents/skills/drift-concord-validation/SKILL.md), at the linked immutable versions.

### Acceptance criteria

- The expedition has a complete start, salvage decision, return and debrief.
- Recoverable failures change the mission without silently deleting the crew's progress.

### Testing procedure

Complete the authored derelict objective, abandon it midway and restart from the supported recovery state. Verify salvage requirements and crew return are achievable without an undocumented facilitator action.

Record setup/fixtures, actions, expected and observed results, relevant logs or artifacts, and PASS / FAIL / NOT RUN for each criterion.

Existing baseline checks (repository root; identity and patch hygiene only):

```sh
git rev-parse HEAD
git status --short
git diff --check 4554bc5fae2cd33a0da369b0fc288f62c8c0a881
```

Exact functional commands, fixtures and paths must be ratified in the execution revision once the prerequisite-selected stack/harness exists. Do not claim these future checks ran.

**Evidence artifact:** `docs/work/W3-T1/acceptance.md` plus the actual patch, fixtures and logs within the approved task scope.

### Acceptance workflow

1. Contributor identifies the saved Tanduna task revision, repository/base, accepted prerequisites, selected primary or fallback model and effort, and exact required skill versions.
2. Contributor performs the task-specific testing procedure and maps each original acceptance criterion to setup, expected result, observed result and reproducible evidence. Failed and unrun checks remain visible.
3. Maintainer reproduces the material checks, reviews the scoped patch or design artifact and verifies the stated model/skill evidence. Unsupported model claims or missing evidence remain unresolved rather than accepted automatically.
4. Maintainer records acceptance or requested changes against the reviewed revision. A passing format check, generated patch or completed model invocation does not by itself satisfy the task.

## W3-T2 — Run first-crew playtests

**Wave:** W3 · **Prerequisites:** W2-T1, W2-T2

Observe complete expeditions by groups unfamiliar with the design.

**Saved Tanduna task:** [W3-T2](https://tanduna.com/p/drift-concord/tasks/tsk_7f004380e2de86829cb283e7f37aea8b)

**Repository:** [https://github.com/thepianistdirector/drift-concord](https://github.com/thepianistdirector/drift-concord) · **Branch:** `main`

**Planning base commit:** [`4554bc5fae2cd33a0da369b0fc288f62c8c0a881`](https://github.com/thepianistdirector/drift-concord/commit/4554bc5fae2cd33a0da369b0fc288f62c8c0a881)

**Execution gate:** Prerequisite results must be accepted and integrated. Maintainer publishes a new task revision against that integrated base before execution; runtime work also needs the real harness and exact allowed paths.

**Preferred:** `gpt-6-astra` / high. **Accepted fallback:** `claude-fable-5-1` / high. Other models require a maintainer revision before work.

**Required skills:** [contribution protocol](https://raw.githubusercontent.com/thepianistdirector/context-harbor/a288bac1ff8bf87fe382ee6bf15ace4c0a090cbd/.agents/skills/tanduna-contribution/SKILL.md) and [Drift Concord validation](https://raw.githubusercontent.com/thepianistdirector/drift-concord/4554bc5fae2cd33a0da369b0fc288f62c8c0a881/.agents/skills/drift-concord-validation/SKILL.md), at the linked immutable versions.

### Acceptance criteria

- Measure role downtime, onboarding failures and whether crews want another mission.
- Publish a prioritized revision of the mission based on observed play.

### Testing procedure

Observe new crews through one full expedition. Record useful participation by role, communication failures, abandonment and discomfort; distinguish tested crew sizes and session lengths from the eventual multiplayer ambition.

Record setup/fixtures, actions, expected and observed results, relevant logs or artifacts, and PASS / FAIL / NOT RUN for each criterion.

Existing baseline checks (repository root; identity and patch hygiene only):

```sh
git rev-parse HEAD
git status --short
git diff --check 4554bc5fae2cd33a0da369b0fc288f62c8c0a881
```

This task uses the saved reproducible manual protocol. Distinguish paper/synthetic exercises from actual participant or physical observations.

**Evidence artifact:** `docs/work/W3-T2/acceptance.md` plus the actual patch, fixtures and logs within the approved task scope.

### Acceptance workflow

1. Contributor identifies the saved Tanduna task revision, repository/base, accepted prerequisites, selected primary or fallback model and effort, and exact required skill versions.
2. Contributor performs the task-specific testing procedure and maps each original acceptance criterion to setup, expected result, observed result and reproducible evidence. Failed and unrun checks remain visible.
3. Maintainer reproduces the material checks, reviews the scoped patch or design artifact and verifies the stated model/skill evidence. Unsupported model claims or missing evidence remain unresolved rather than accepted automatically.
4. Maintainer records acceptance or requested changes against the reviewed revision. A passing format check, generated patch or completed model invocation does not by itself satisfy the task.

## W4-T1 — Persist the ship and expedition journal

**Wave:** W4 · **Prerequisites:** W3-T1, W3-T2

Save configuration, cargo and completed expedition events with recoverable migrations.

**Saved Tanduna task:** [W4-T1](https://tanduna.com/p/drift-concord/tasks/tsk_e5cc9ee7456e10a216b1f5b54b74e03f)

**Repository:** [https://github.com/thepianistdirector/drift-concord](https://github.com/thepianistdirector/drift-concord) · **Branch:** `main`

**Planning base commit:** [`4554bc5fae2cd33a0da369b0fc288f62c8c0a881`](https://github.com/thepianistdirector/drift-concord/commit/4554bc5fae2cd33a0da369b0fc288f62c8c0a881)

**Execution gate:** Prerequisite results must be accepted and integrated. Maintainer publishes a new task revision against that integrated base before execution; runtime work also needs the real harness and exact allowed paths.

**Preferred:** `gpt-6-astra` / high. **Accepted fallback:** `claude-fable-5-1` / high. Other models require a maintainer revision before work.

**Required skills:** [contribution protocol](https://raw.githubusercontent.com/thepianistdirector/context-harbor/a288bac1ff8bf87fe382ee6bf15ace4c0a090cbd/.agents/skills/tanduna-contribution/SKILL.md) and [Drift Concord validation](https://raw.githubusercontent.com/thepianistdirector/drift-concord/4554bc5fae2cd33a0da369b0fc288f62c8c0a881/.agents/skills/drift-concord-validation/SKILL.md), at the linked immutable versions.

### Acceptance criteria

- A restarted server restores the ship and identifies incompatible content versions.
- A crew can export its ship history without exposing private account data.

### Testing procedure

Save after damage and salvage changes, stop the server and reload on the supported version. Compare ship, cargo, crew and journal, then exercise the documented older-save migration or refusal.

Record setup/fixtures, actions, expected and observed results, relevant logs or artifacts, and PASS / FAIL / NOT RUN for each criterion.

Existing baseline checks (repository root; identity and patch hygiene only):

```sh
git rev-parse HEAD
git status --short
git diff --check 4554bc5fae2cd33a0da369b0fc288f62c8c0a881
```

Exact functional commands, fixtures and paths must be ratified in the execution revision once the prerequisite-selected stack/harness exists. Do not claim these future checks ran.

**Evidence artifact:** `docs/work/W4-T1/acceptance.md` plus the actual patch, fixtures and logs within the approved task scope.

### Acceptance workflow

1. Contributor identifies the saved Tanduna task revision, repository/base, accepted prerequisites, selected primary or fallback model and effort, and exact required skill versions.
2. Contributor performs the task-specific testing procedure and maps each original acceptance criterion to setup, expected result, observed result and reproducible evidence. Failed and unrun checks remain visible.
3. Maintainer reproduces the material checks, reviews the scoped patch or design artifact and verifies the stated model/skill evidence. Unsupported model claims or missing evidence remain unresolved rather than accepted automatically.
4. Maintainer records acceptance or requested changes against the reviewed revision. A passing format check, generated patch or completed model invocation does not by itself satisfy the task.

## W4-T2 — Build the expedition authoring kit

**Wave:** W4 · **Prerequisites:** W3-T1, W3-T2

Describe locations, hazards, objectives and outcomes as inspectable mission packages.

**Saved Tanduna task:** [W4-T2](https://tanduna.com/p/drift-concord/tasks/tsk_39ea36f9eb20f41a47de4fe4be473989)

**Repository:** [https://github.com/thepianistdirector/drift-concord](https://github.com/thepianistdirector/drift-concord) · **Branch:** `main`

**Planning base commit:** [`4554bc5fae2cd33a0da369b0fc288f62c8c0a881`](https://github.com/thepianistdirector/drift-concord/commit/4554bc5fae2cd33a0da369b0fc288f62c8c0a881)

**Execution gate:** Prerequisite results must be accepted and integrated. Maintainer publishes a new task revision against that integrated base before execution; runtime work also needs the real harness and exact allowed paths.

**Preferred:** `gpt-6-astra` / high. **Accepted fallback:** `claude-fable-5-1` / high. Other models require a maintainer revision before work.

**Required skills:** [contribution protocol](https://raw.githubusercontent.com/thepianistdirector/context-harbor/a288bac1ff8bf87fe382ee6bf15ace4c0a090cbd/.agents/skills/tanduna-contribution/SKILL.md) and [Drift Concord validation](https://raw.githubusercontent.com/thepianistdirector/drift-concord/4554bc5fae2cd33a0da369b0fc288f62c8c0a881/.agents/skills/drift-concord-validation/SKILL.md), at the linked immutable versions.

### Acceptance criteria

- A contributor authors a second expedition without modifying core ship simulation.
- Malformed or malicious package inputs fail before affecting a persistent ship.

### Testing procedure

Have a second author create an expedition using the published kit. Load it on a clean server; then remove a required asset or use an unsupported version and inspect the diagnostic and preserved state.

Record setup/fixtures, actions, expected and observed results, relevant logs or artifacts, and PASS / FAIL / NOT RUN for each criterion.

Existing baseline checks (repository root; identity and patch hygiene only):

```sh
git rev-parse HEAD
git status --short
git diff --check 4554bc5fae2cd33a0da369b0fc288f62c8c0a881
```

Exact functional commands, fixtures and paths must be ratified in the execution revision once the prerequisite-selected stack/harness exists. Do not claim these future checks ran.

**Evidence artifact:** `docs/work/W4-T2/acceptance.md` plus the actual patch, fixtures and logs within the approved task scope.

### Acceptance workflow

1. Contributor identifies the saved Tanduna task revision, repository/base, accepted prerequisites, selected primary or fallback model and effort, and exact required skill versions.
2. Contributor performs the task-specific testing procedure and maps each original acceptance criterion to setup, expected result, observed result and reproducible evidence. Failed and unrun checks remain visible.
3. Maintainer reproduces the material checks, reviews the scoped patch or design artifact and verifies the stated model/skill evidence. Unsupported model claims or missing evidence remain unresolved rather than accepted automatically.
4. Maintainer records acceptance or requested changes against the reviewed revision. A passing format check, generated patch or completed model invocation does not by itself satisfy the task.

## W5-T1 — Package community hosting and moderation

**Wave:** W5 · **Prerequisites:** W4-T1, W4-T2

Deliver host setup, access control, logs and a documented recovery procedure.

**Saved Tanduna task:** [W5-T1](https://tanduna.com/p/drift-concord/tasks/tsk_aab13cbed84ea6c0ff573c30c10b0f2d)

**Repository:** [https://github.com/thepianistdirector/drift-concord](https://github.com/thepianistdirector/drift-concord) · **Branch:** `main`

**Planning base commit:** [`4554bc5fae2cd33a0da369b0fc288f62c8c0a881`](https://github.com/thepianistdirector/drift-concord/commit/4554bc5fae2cd33a0da369b0fc288f62c8c0a881)

**Execution gate:** Prerequisite results must be accepted and integrated. Maintainer publishes a new task revision against that integrated base before execution; runtime work also needs the real harness and exact allowed paths.

**Preferred:** `gpt-6-astra` / high. **Accepted fallback:** `claude-fable-5-1` / high. Other models require a maintainer revision before work.

**Required skills:** [contribution protocol](https://raw.githubusercontent.com/thepianistdirector/context-harbor/a288bac1ff8bf87fe382ee6bf15ace4c0a090cbd/.agents/skills/tanduna-contribution/SKILL.md) and [Drift Concord validation](https://raw.githubusercontent.com/thepianistdirector/drift-concord/4554bc5fae2cd33a0da369b0fc288f62c8c0a881/.agents/skills/drift-concord-validation/SKILL.md), at the linked immutable versions.

### Acceptance criteria

- A second operator hosts a complete expedition from the documentation.
- Test abusive joins, role permissions, removal and recovery without giving moderators hidden player advantage.

### Testing procedure

Have a second operator install, back up and recover the reference server. Rehearse a moderation action and its permitted appeal/recovery flow with test identities, documenting actual operator effort.

Record setup/fixtures, actions, expected and observed results, relevant logs or artifacts, and PASS / FAIL / NOT RUN for each criterion.

Existing baseline checks (repository root; identity and patch hygiene only):

```sh
git rev-parse HEAD
git status --short
git diff --check 4554bc5fae2cd33a0da369b0fc288f62c8c0a881
```

Exact functional commands, fixtures and paths must be ratified in the execution revision once the prerequisite-selected stack/harness exists. Do not claim these future checks ran.

**Evidence artifact:** `docs/work/W5-T1/acceptance.md` plus the actual patch, fixtures and logs within the approved task scope.

### Acceptance workflow

1. Contributor identifies the saved Tanduna task revision, repository/base, accepted prerequisites, selected primary or fallback model and effort, and exact required skill versions.
2. Contributor performs the task-specific testing procedure and maps each original acceptance criterion to setup, expected result, observed result and reproducible evidence. Failed and unrun checks remain visible.
3. Maintainer reproduces the material checks, reviews the scoped patch or design artifact and verifies the stated model/skill evidence. Unsupported model claims or missing evidence remain unresolved rather than accepted automatically.
4. Maintainer records acceptance or requested changes against the reviewed revision. A passing format check, generated patch or completed model invocation does not by itself satisfy the task.

## W5-T2 — Prototype explicit sector handoff

**Wave:** W5 · **Prerequisites:** W4-T1, W4-T2

Design and test ownership transfer between two cooperating sector servers.

**Saved Tanduna task:** [W5-T2](https://tanduna.com/p/drift-concord/tasks/tsk_ac12c2c4bafe59855e4de2dd28b402cc)

**Repository:** [https://github.com/thepianistdirector/drift-concord](https://github.com/thepianistdirector/drift-concord) · **Branch:** `main`

**Planning base commit:** [`4554bc5fae2cd33a0da369b0fc288f62c8c0a881`](https://github.com/thepianistdirector/drift-concord/commit/4554bc5fae2cd33a0da369b0fc288f62c8c0a881)

**Execution gate:** Prerequisite results must be accepted and integrated. Maintainer publishes a new task revision against that integrated base before execution; runtime work also needs the real harness and exact allowed paths.

**Preferred:** `gpt-6-astra` / high. **Accepted fallback:** `claude-fable-5-1` / high. Other models require a maintainer revision before work.

**Required skills:** [contribution protocol](https://raw.githubusercontent.com/thepianistdirector/context-harbor/a288bac1ff8bf87fe382ee6bf15ace4c0a090cbd/.agents/skills/tanduna-contribution/SKILL.md) and [Drift Concord validation](https://raw.githubusercontent.com/thepianistdirector/drift-concord/4554bc5fae2cd33a0da369b0fc288f62c8c0a881/.agents/skills/drift-concord-validation/SKILL.md), at the linked immutable versions.

### Acceptance criteria

- A failed handoff leaves ship and cargo owned in exactly one recoverable location.
- Players see connection and trust boundaries before transferring.

### Testing procedure

Interrupt sector departure, destination receipt and acknowledgement. Retry each case and reconcile ship/cargo/crew ownership; identify the supported recovery state without promising cross-region scale beyond the test.

Record setup/fixtures, actions, expected and observed results, relevant logs or artifacts, and PASS / FAIL / NOT RUN for each criterion.

Existing baseline checks (repository root; identity and patch hygiene only):

```sh
git rev-parse HEAD
git status --short
git diff --check 4554bc5fae2cd33a0da369b0fc288f62c8c0a881
```

Exact functional commands, fixtures and paths must be ratified in the execution revision once the prerequisite-selected stack/harness exists. Do not claim these future checks ran.

**Evidence artifact:** `docs/work/W5-T2/acceptance.md` plus the actual patch, fixtures and logs within the approved task scope.

### Acceptance workflow

1. Contributor identifies the saved Tanduna task revision, repository/base, accepted prerequisites, selected primary or fallback model and effort, and exact required skill versions.
2. Contributor performs the task-specific testing procedure and maps each original acceptance criterion to setup, expected result, observed result and reproducible evidence. Failed and unrun checks remain visible.
3. Maintainer reproduces the material checks, reviews the scoped patch or design artifact and verifies the stated model/skill evidence. Unsupported model claims or missing evidence remain unresolved rather than accepted automatically.
4. Maintainer records acceptance or requested changes against the reviewed revision. A passing format check, generated patch or completed model invocation does not by itself satisfy the task.

## W6-T1 — Build a varied expedition pilot

**Wave:** W6 · **Prerequisites:** W5-T1, W5-T2

Add a bounded set of exploration, rescue and engineering missions using the kit.

**Saved Tanduna task:** [W6-T1](https://tanduna.com/p/drift-concord/tasks/tsk_bf9be4fd5eaa5124438233002d616af4)

**Repository:** [https://github.com/thepianistdirector/drift-concord](https://github.com/thepianistdirector/drift-concord) · **Branch:** `main`

**Planning base commit:** [`4554bc5fae2cd33a0da369b0fc288f62c8c0a881`](https://github.com/thepianistdirector/drift-concord/commit/4554bc5fae2cd33a0da369b0fc288f62c8c0a881)

**Execution gate:** Prerequisite results must be accepted and integrated. Maintainer publishes a new task revision against that integrated base before execution; runtime work also needs the real harness and exact allowed paths.

**Preferred:** `gpt-6-astra` / high. **Accepted fallback:** `claude-fable-5-1` / high. Other models require a maintainer revision before work.

**Required skills:** [contribution protocol](https://raw.githubusercontent.com/thepianistdirector/context-harbor/a288bac1ff8bf87fe382ee6bf15ace4c0a090cbd/.agents/skills/tanduna-contribution/SKILL.md) and [Drift Concord validation](https://raw.githubusercontent.com/thepianistdirector/drift-concord/4554bc5fae2cd33a0da369b0fc288f62c8c0a881/.agents/skills/drift-concord-validation/SKILL.md), at the linked immutable versions.

### Acceptance criteria

- Each mission offers a different crew decision instead of only changing scenery.
- Mixed-experience groups can complete the mission set and report meaningful role choice.

### Testing procedure

Play the agreed varied expedition set with new and returning crews. Compare choices, repeated coordination patterns and replay willingness; record where different content still produces the same experience.

Record setup/fixtures, actions, expected and observed results, relevant logs or artifacts, and PASS / FAIL / NOT RUN for each criterion.

Existing baseline checks (repository root; identity and patch hygiene only):

```sh
git rev-parse HEAD
git status --short
git diff --check 4554bc5fae2cd33a0da369b0fc288f62c8c0a881
```

This task uses the saved reproducible manual protocol. Distinguish paper/synthetic exercises from actual participant or physical observations.

**Evidence artifact:** `docs/work/W6-T1/acceptance.md` plus the actual patch, fixtures and logs within the approved task scope.

### Acceptance workflow

1. Contributor identifies the saved Tanduna task revision, repository/base, accepted prerequisites, selected primary or fallback model and effort, and exact required skill versions.
2. Contributor performs the task-specific testing procedure and maps each original acceptance criterion to setup, expected result, observed result and reproducible evidence. Failed and unrun checks remain visible.
3. Maintainer reproduces the material checks, reviews the scoped patch or design artifact and verifies the stated model/skill evidence. Unsupported model claims or missing evidence remain unresolved rather than accepted automatically.
4. Maintainer records acceptance or requested changes against the reviewed revision. A passing format check, generated patch or completed model invocation does not by itself satisfy the task.

## W6-T2 — Publish performance and operations findings

**Wave:** W6 · **Prerequisites:** W5-T1, W5-T2

Measure client performance, supported crew sizes, restoration and content moderation effort.

**Saved Tanduna task:** [W6-T2](https://tanduna.com/p/drift-concord/tasks/tsk_cb87b359b8d6a0f5a3e3186ebc3eccc5)

**Repository:** [https://github.com/thepianistdirector/drift-concord](https://github.com/thepianistdirector/drift-concord) · **Branch:** `main`

**Planning base commit:** [`4554bc5fae2cd33a0da369b0fc288f62c8c0a881`](https://github.com/thepianistdirector/drift-concord/commit/4554bc5fae2cd33a0da369b0fc288f62c8c0a881)

**Execution gate:** Prerequisite results must be accepted and integrated. Maintainer publishes a new task revision against that integrated base before execution; runtime work also needs the real harness and exact allowed paths.

**Preferred:** `gpt-6-astra` / high. **Accepted fallback:** `claude-fable-5-1` / high. Other models require a maintainer revision before work.

**Required skills:** [contribution protocol](https://raw.githubusercontent.com/thepianistdirector/context-harbor/a288bac1ff8bf87fe382ee6bf15ace4c0a090cbd/.agents/skills/tanduna-contribution/SKILL.md) and [Drift Concord validation](https://raw.githubusercontent.com/thepianistdirector/drift-concord/4554bc5fae2cd33a0da369b0fc288f62c8c0a881/.agents/skills/drift-concord-validation/SKILL.md), at the linked immutable versions.

### Acceptance criteria

- Results name hardware, network conditions and mission complexity.
- Set the next capacity target from measured constraints rather than a galaxy-sized launch promise.

### Testing procedure

Run the same expedition workload on documented client/server hardware and network conditions. Publish frame/server timings, bandwidth and recovery incidents with the measured crew count and duration.

Record setup/fixtures, actions, expected and observed results, relevant logs or artifacts, and PASS / FAIL / NOT RUN for each criterion.

Existing baseline checks (repository root; identity and patch hygiene only):

```sh
git rev-parse HEAD
git status --short
git diff --check 4554bc5fae2cd33a0da369b0fc288f62c8c0a881
```

Exact functional commands, fixtures and paths must be ratified in the execution revision once the prerequisite-selected stack/harness exists. Do not claim these future checks ran.

**Evidence artifact:** `docs/work/W6-T2/acceptance.md` plus the actual patch, fixtures and logs within the approved task scope.

### Acceptance workflow

1. Contributor identifies the saved Tanduna task revision, repository/base, accepted prerequisites, selected primary or fallback model and effort, and exact required skill versions.
2. Contributor performs the task-specific testing procedure and maps each original acceptance criterion to setup, expected result, observed result and reproducible evidence. Failed and unrun checks remain visible.
3. Maintainer reproduces the material checks, reviews the scoped patch or design artifact and verifies the stated model/skill evidence. Unsupported model claims or missing evidence remain unresolved rather than accepted automatically.
4. Maintainer records acceptance or requested changes against the reviewed revision. A passing format check, generated patch or completed model invocation does not by itself satisfy the task.
