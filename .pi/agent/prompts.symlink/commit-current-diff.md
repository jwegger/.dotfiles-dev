---
description: "Review the current Git diff, write a concise commit message, and create the commit"
argument-hint: "[context]"
---

Review the current Git working-tree diff and create one focused Git commit for it.

Use the optional context below only when it clarifies the intent of the diff:

${@:-(no additional context provided)}

Workflow:

1. Inspect `git status`, the staged diff, the unstaged diff, and
   recent commits to understand the repository's commit-message convention.

2. Do not include unrelated changes. If the current diff contains unrelated
   changes, stage only the files and hunks that form the focused commit.

3. Write a precise commit message that explains the change at the
   appropriate behavioral level.

   The subject should state the primary outcome or action. The body
   should provide the context needed to understand the change without
   reading the diff: what motivated it, how behavior changes, and any
   important compatibility, operational, or user-facing implications.

   Prefer concrete statements over abstractions. Do not describe
   mechanical implementation details unless they are necessary to
   explain behavior, constraints, or risk.

4. The subject must be imperative, have no trailing period, and
   contain at most 50 characters. Follow the repository's established
   component-prefix, capitalization, and wording conventions. Do not
   capitalize first letter after 'module: ' colon.

5. Include a body when the subject alone does not adequately convey
   intent, impact, or rationale. Wrap every body line at 60 characters
   or fewer, with a blank line between subject and body.

6. Before committing, review the proposed message as though it were
   being read later in `git log` or a release investigation. It should
   make clear:
   - what changed from a caller, user, or system perspective;
   - why the change was needed; and
   - any material effects or constraints.
