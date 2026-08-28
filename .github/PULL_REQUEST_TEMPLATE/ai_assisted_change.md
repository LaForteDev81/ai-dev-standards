## Summary
<!-- What does this change do, and why? -->

## AI Tools Used
<!-- e.g., GitHub Copilot, Claude, ChatGPT — which tool(s) generated or assisted this change -->

---

## Pre-Commit Review Checklist (AI-Assisted Code)

### Core Four

- [ ] **Tested against actual test cases** — not just skimmed the code.
  > Reading AI-generated code and thinking "this looks right" isn't the same as running it. Confirm this was exercised against real scenarios, including edge cases — not just the happy path.

- [ ] **Matches our architecture and standards.**
  > AI output can be functionally correct while still violating team conventions. The model doesn't know your team's standards unless you told it — confirm this would pass review as if a teammate wrote it.

- [ ] **I can explain and debug this myself.**
  > If you can't explain what the code does or why it works, you're not in a position to maintain it. Could you walk a teammate through this line by line?

- [ ] **New dependencies verified as real.**
  > Models can invent plausible-sounding package names — attackers register the fakes. Source control protects against losing working code; it does nothing to protect against installing a malicious package.

### Optional: Cross-Check
- [ ] **Reviewed by a different model or fresh session** (if applicable).
  > A model tends to defend its own prior reasoning within a conversation. A fresh session (or different model) has no earlier answer to protect, and is more likely to catch a mismatch. Treat as a backup check.

### Team Hygiene
- [ ] **Change is small and single-purpose.**
  > Generating a large diff is cheap; reviewing it properly still takes time. If this PR is sprawling, consider splitting it (stacked PRs work well for this).

- [ ] **Reviewed any commands/installs the AI tool proposed** before approving them.
  > Don't approve unfamiliar commands or extensions by default — this is the same risk category as the fake-package check above, just at the tooling level.

## Additional Context
<!-- Anything reviewers should know: known limitations, follow-up work, related tickets -->
