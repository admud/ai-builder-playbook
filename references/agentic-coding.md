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

## Entry Template

- **Author / publication date:**
- **Original source:**
- **Idea to try:**
- **Proposed pilot / scope:**
- **Status:** Reference
- **Evidence / decision:** Not run. Add an evidence link and date after a trial.
