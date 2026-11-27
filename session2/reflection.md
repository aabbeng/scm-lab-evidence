# Session 2 Reflection

## Q1. How do Issues and pull requests together support change control?

An Issue records why a change is needed, its expected result, and checkable acceptance criteria before implementation begins. The pull request then presents the exact change from a branch, gives reviewers a place to discuss it, and records how feedback was handled. In this session, pull request #2 referenced and closed issue #1, so the reason, implementation, review, and merge remain connected in one traceable chain.

## Q2. Why did the conflict happen, and how could a team reduce such conflicts?

The local conflict happened because `branch-a` and `branch-b` started from the same base and changed the only line in `session2/conflict-demo.md` to different values. Git could not infer whether staging or production was correct, so I kept staging with a note that production requires approval. A team can reduce conflicts by pulling before starting work, coordinating ownership of frequently edited files, using short-lived branches, and merging small changes regularly.

## Q3. What would be lost if people merged straight into main without a pull request?

Merging directly into `main` would remove the review checkpoint where scope, quality, secrets, and acceptance criteria can be checked before integration. It would also weaken the durable record of discussion, suggested changes, responses, and the relationship between an Issue and its implementation. Problems would be harder to catch early and future maintainers would have less evidence explaining why the change was accepted.
