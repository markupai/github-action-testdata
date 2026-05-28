# Demo: v2 PR-comment rendering

This file was added to show off how the v2 action renders its PR summary and inline review comments. The point is to give the style agent something concrete to flag so that reviewers can see all four output surfaces at once.

## Why this exists

We will be checking how the inline review comments are placed, whether the summary table is rendered correctly, and that the new agent-attribution lines appear in both the inline-comment header and the footer of the summary comment.

## What you should see

- A single summary comment from the action with the risk table, the per-file breakdown, and the new "Detected by: Style Agent" line in the footer.
- Inline review comments anchored to lines in this file, each headed with "Markup AI / Style Agent detected issues:" and listing the issues the agent picked up.
- A clean PR — no stale comments from prior runs (the reconciler deletes outdated comments automatically).
