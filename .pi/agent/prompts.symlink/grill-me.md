---
description: Relentlessly interview me to clarify an objective and its design decisions
argument-hint: "<objective>"
---
Objective: $ARGUMENTS

Interview me relentlessly about every aspect of the objective until we
reach a shared understanding. Walk down each branch of the design tree,
resolving dependencies between decisions one-by-one.

Ask about only one topic, or a small set of closely related topics, at a
time. Do not move on to the next topic until we have explicitly agreed
on a shared understanding of the current one.

If a question can be answered by exploring the codebase, explore the
codebase instead.

For each question, provide your recommended answer.

## Design document

Maintain a design document that always reflects our current shared
understanding.

- When we agree on the first decision, create the document. Pick a
  sensible location and file name based on the objective and the
  codebase conventions, and tell me the path. Note in it that it
  originates from a `/grill-me` session and state the objective.
- After every later decision, update the document before asking the next
  question.
- Write the document as a coherent description of the current design,
  not an append-only log of the conversation. Integrate each new
  decision where it belongs, and when a decision refines, changes, or
  invalidates an earlier one, rewrite the affected parts so nothing
  stale or contradictory remains.
- Record only what we have explicitly agreed on. Keep unresolved topics
  and known open questions in a separate section, and remove them once
  they are resolved.
- Where it helps a future reader, briefly capture the rationale and
  rejected alternatives for a decision.
- In each response, briefly say what you changed in the document.
