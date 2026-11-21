# Verify an Agent-Built Change

Build a repeatable evidence trail before calling an agent-built change done.

## What You Will Make

A small change with acceptance criteria, runnable checks, and a PR proof summary.
This is a proposed workflow, not a claim that a particular product has passed it.

## Tools

- Your coding agent and repository's existing check commands
- The relevant local or staging runtime: browser, simulator, CLI, or API
- A fresh reviewer when the risk warrants independent review

## Steps

1. **Define done before coding.** State the user flow or API behavior, what must stay unchanged, and one observable failure case. Decide what evidence will count.
2. **Run the cheap checks first.** Use the repo's own lint, typecheck, targeted tests, and build as applicable. Record the exact commands and outcomes. For a bug fix, capture a regression check that fails before the fix when practical.
3. **Exercise the built change.** Use the real local or staging app, browser, simulator, CLI, or API. Check a normal path and the most relevant negative path with synthetic or approved test data. A screenshot alone is not proof of persistence, access control, or side effects.
4. **Choose stronger checks when warranted.** Use end-to-end tests for user journeys, property tests for invariants (like retries not creating duplicates), and differential tests for migrations or rewrites that must preserve behavior. Record intentional differences instead of treating the old system as infallible.
5. **Review the exact commit.** For changes that need independent review, give a fresh reviewer the original acceptance criteria and base-branch review rules. Report failures with evidence. Do not weaken assertions, skip failing tests, or rewrite the gate to pass its own change. Material new commits invalidate stale evidence.
6. **Stop and learn.** As a starting stop rule, after three unsuccessful fix-and-check rounds, stop and explain the root-cause hypothesis, last result, and what needs a human. Turn a real miss into a regression test or narrow repo rule. Run proposed gates in report-only mode before making them blocking.

## Proof in the PR

- **Commit / environment:** exact SHA, environment, and fixture or account type
- **Acceptance:** expected behavior, observed behavior, and evidence link
- **Checks:** command, result, and what was not tested
- **Risk / rollback:** what could go wrong, how to undo it, and who must review

Use stronger independent human review for auth, permissions, billing, migrations, CI, or release changes. Never turn a local mock into a claim about production. Mark blocked checks as **not verified**.

## Suggested First Pilot

This is a generic example, not a completed test. In an n8n staging workflow with synthetic data, assert that a normal enquiry reaches the intended review queue, a CRM timeout causes no outbound customer message or final write, and replayed inputs do not duplicate the final action. If the last assertion is only checked within one run, say so.

## Prompt

```text
Implement [CHANGE] in [REPOSITORY]. Read the repository's instructions first.
Before editing, list the acceptance criteria, key failure case, and checks.
Use synthetic or approved test data and the existing check commands.
Exercise the affected behavior in the appropriate local or staging runtime.
Do not weaken checks to pass this change or alter security/CI settings.
At the final commit, report commands, results, evidence, gaps, and rollback.
If blocked, say what is not verified rather than claiming completion.
```

## What to Learn from Each Run

- Which observable check caught a real failure?
- What did the test environment fail to represent?
- Which narrow regression test would prevent the same mistake?

The three-round stop rule and PR proof format here are starting conventions,
not claims about another team's exact policy. Adjust them explicitly to the
project and risk. Use the [reference log](../references/agentic-coding.md) to
track ideas, trials, and evidence before marking a practice adopted.
