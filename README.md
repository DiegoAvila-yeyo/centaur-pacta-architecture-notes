# Centaur Pacta Architecture Notes

This repository stores architecture notes for embedding Centaur into `pacta-web` as a Pacta workspace agent.

## Intent

This is not a traditional web IDE.

The target is a dashboard / control plane where Centaur can work on real repositories with human approvals at sensitive steps.

## Desired Flow

1. Enter a repo or section.
2. Request tickets.
3. Choose a ticket.
4. Plan with Centaur.
5. Let Centaur implement changes in the correct repo.
6. Review diff and validations.
7. Approve commit.
8. Approve push.
9. Approve PR.

## Design Constraints

- Iterative co-design, not a closed solution.
- Short, clear architectural discussion.
- No default push toward microservices.
- Focus on boundaries, responsibilities, and tradeoffs.
- Ask when ambiguity matters.
- Critique risks clearly.
- Avoid turning this into an implementation plan too early.

## Current Framing

The working metaphor is:

- `center`
- `shell`
- `rails`

The current interpretation from the session is captured in [docs/session-2026-07-01.md](/Users/eltitoyeyo/centaur-pacta-architecture-notes/docs/session-2026-07-01.md).

## Current Focus

For now, the exploration is centered on vanilla application architecture:

- architecture families
- code organization
- internal boundaries
- workflows
- movement/control inside the system

Explicitly de-emphasized for now:

- persistence
- memory subsystem
- distributed infrastructure
- cloud topology

