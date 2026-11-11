# Workflow Audit

A short write-up on how the four pieces of a tidy GitHub workflow fit together: **branch → pull request**, **issue**, and **close-out**.

## Branch lifecycle

Branches are the factory for change. Every line of work starts on a dedicated branch off the default branch (e.g. `main`), keeps the working tree isolated, and is named in a `kebab-case` style that says what it does (`feature/audit-notes`, `hotfix/login-bug`). When the work is done, the branch has a *pull request*, not a magical in-place edit to `main` — that review gate is what keeps master clean.

## Pull request and review

A pull request describes the change from the feature branch into the default branch. It is the conversation surface of a GitHub workflow:

1. **Open a PR** from `feature/audit-notes` into `main`, with a short title and a descriptive description (why, what, impact).
2. **Review it** — comments on specific lines, approve, request changes, or request a re-run of CI on thesame base.
3. **Merge when satisfied.** Leaving a PR open (unmerged) after review is itself a signal of the workflow: pull requests stay as *open state* until they are merged or closed deliberately. For a demo artifact, an open, reviewed PR is a great thing to show — it proves the review step happened without destroying history.

## Issues and tracking

Issues are for *what* needs to happen, not *how* it happens. They are the task layer:

- The **checklist issue** ("Demo: workflow checklist") captures theRemaining action items.
- **Sub-issues** let one issue decompose into smaller, traceable pieces — each sub-issue is numbered under the parent in the same pull request's close-out.
- **Comments** add detail to a task without moving it out of the conversation.

## Close-out

A tidy workflow ends with a clean handoff: the checklist is marked as completed, the follow-up (if any) is attached or left as its own open issue, and the PR is either merged or explicitly closed. Status, owner, and review trail all live in the GitHub UI — no email thread required.

## Owner

Retrieved from the account on the demo date:

| Field | Value |
| --- | --- |
| Login | HeziLiu |
| Display name | Hezi Liu |
| Bio | treat me like a tree |
| Location | Beijing/Guiyang |
| Company | BUPT/GZU |
