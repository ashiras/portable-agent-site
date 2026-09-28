# Portable Agent Website Section Copy

## Eyebrow
ACTUAL TRAJECTORY REPLAY

## Headline
Not “the AI said it works.”
The trajectory proved it.

## Lead
Portable Agent does not treat a model response as success.
It creates isolated work, lets the LLM inspect and modify the repository,
measures the result with an external Guard, retries when necessary,
and only then advances to an Accepted Checkpoint.

## Four proof points

### Isolated Worktree
The human repository stays untouched while the agent works.

### External Guard
Success is measured outside the model.

### Checkpoint Ownership
The LLM may change artifacts. Portable Agent owns the commit transition.

### Explicit Lifecycle
Work is created, accepted, and closed as separate operations.

## Replay heading
A real v0.5.0 end-to-end run

## Replay note
The sequence below is based on an actual Portable Agent run.
The first attempt failed its Guard, the next attempt corrected the artifact,
and only then did the trajectory reach Gate ACCEPT.

## Key callout
The model says “done.”
The Guard says “not yet.”

## Core statement
The model generates.
Portable Agent decides whether the trajectory may advance.

## Closing
A full trajectory, not just a model response.

Portable Agent separates generation from acceptance:
Artifact, Guard, Gate, and Checkpoint are explicit runtime boundaries.
The LLM is a replaceable Engine. The trajectory is controlled outside the model.
