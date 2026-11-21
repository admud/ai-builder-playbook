# Agentic Coding Reference Log

[Taste Index](https://github.com/admud/taste-index) focuses on design taste.
This index tracks practical ideas for building and verifying software with agents.
Start with the [verification playbook](../tips/003-agentic-coding-verification.md).

## How to Track an Idea

Keep one entry per practical idea, with author, source publication date, original
link, what to try, where to try it, and evidence of the outcome. Use these states:
**Reference → Piloting → Adopted / Rejected**. Only mark an idea adopted after
running its check in a real project. Keep private project details and evidence
out of this public log; describe those trials generically or leave them private.

The trial proposals below are our synthesis, not verbatim source instructions.
None is marked adopted, and this log does not install or enforce repository gates.

| Source and publication date | Idea to try | Proposed pilot | Status / evidence |
| --- | --- | --- | --- |
| Addy Osmani, Nov 16, 2026: [How the Claude Code team thinks about verification](https://claude.dev/blog/how-the-claude-code-team-thinks-about-verification/); [X thread](https://x.com/addyosmani/status/2122590683055993308) | Make the real user flow runnable; preserve independent checks and commit-specific evidence. | Synthetic n8n workflow: success, CRM timeout, and replay cases from the verification playbook. | Reference; not run. |
| Addy Osmani, Morgan Westlee Lunt, Qing Wang, Oct 15, 2026: [How the Claude Code team does code review](https://claude.dev/blog/solving-code-review-at-anthropic/) | Run cheap checks before review, then scale human approval and rollback planning to risk. | A small change with the exact commit, command outcomes, untested paths, and rollback in its PR. | Reference; not run. |
| Lauren Tan, Nov 19, 2026: [Automate Anything with Grok Bot](https://x.com/poteto/status/2123159537016533493); [article mirror](https://www.teapawt.org/poteto/article/2123159537016533493); [secondary summary](https://thegrokbotguide.com/tips/automate-anything-goal-first/) | Specify the outcome, not just activity. Teach decisions with examples and exceptions; check the result through feedback before adding a trigger. | Define one synthetic booking workflow with a success case, conflicting times, and missing information. Require the agent to restate the goal, avoid duplicate bookings, and distinguish a sent message from a confirmed booking. Target repository: not selected. | Reference only; saved for workflow design. Proposed test, not run; no implementation or automation authorized. Original X could not be fetched directly; mirror and secondary summary retained for provenance. |
| Greg Isenberg, Nov 20, 2026 (UTC): [41 ideas for builders](https://x.com/gregisenberg/status/2123906584531304944) | Treat day-2 maintenance (#6), agent undo (#37), expert sign-off (#30), and agent spend limits and receipts (#12) as opportunity hypotheses, not demand evidence. Smaller applications include one-trip tools (#7) and trigger-based outreach drafts with our own human-review gate (#32). | Offline fixture only: stage a mock itinerary edit, block apply until approved, then apply once and restore the exact prior state on undo. Check that replay cannot duplicate the edit, an over-budget mock request is blocked, and the audit log records each decision. No live bookings, payments or messages; target repo not selected. | Reference saved; proposed pilot not run or authorized. Based on a user-supplied copy of the post; direct X access returned 403. |

## Entry Template

- **Author / publication date:**
- **Original source:**
- **Idea to try:**
- **Proposed pilot / scope:**
- **Status:** Reference
- **Evidence / decision:** Not run. Add an evidence link and date after a trial.

## Standing Intake Convention

This AI Builder Playbook index is the canonical home for shared links about
building with AI and agentic coding. Keep one record here rather than splitting
the tracker across brand repositories. For design/UI references, cross-link the
relevant Taste Index entry instead of duplicating its catalog.

1. **Read and deduplicate.** Prefer the original source; remove tracking parameters
   without dropping meaningful query parameters or anchors. Match canonical URLs
   and existing ideas before adding a record. Keep a useful shared-post link as
   context alongside its original article.
2. **Save and implement are separate decisions.** Save a useful reference, identify
   an implementation candidate, or do both. Default to **Reference** or
   **Candidate**, not adopted. A saved link or candidate is not permission to
   publish, deploy, spend money, or make risky repository changes.
3. **Make the next action clear.** Record a short takeaway, why it applies, the
   proposed next action and target repository (or “not selected”). An implementation
   follows the applicable authorization and review process. Move through Piloting
   to Adopted / Rejected only with a dated outcome and evidence.
4. **Keep public records safe.** Sensitive or internal sources, target repositories,
   and evidence stay in an appropriate private record. Do not expose their URLs
   or identifying details in this public index.

For new entries, use these fields in addition to the source attribution above:

- **Canonical URL / related shared link:**
- **Short takeaway / applicability:**
- **Save decision:** Save / Skip, with a short reason.
- **Implementation decision:** Reference only / Candidate / Authorized trial.
- **Next action / target repository:** Not selected until scoped.
- **Status / dated evidence:** Reference or Candidate initially; when implemented,
  link the public PR or commit and verification result, or keep the record private.
