# How to Report an Issue

Author: iDevOpsLLC

This repository is the public issue tracker for [Agentic Copilot](https://ai.nowidevops.com). It contains **no application source code** — the product is proprietary. Contributions here take the form of clear issue reports and feature requests.

**Pull requests are not accepted.** There is nothing to change in code; if you spot an error in this repository's own documentation or templates, open an issue and we'll fix it.

## Before you open an issue

1. **Search [existing issues](../../issues)**, including closed ones. If you find yours, add a comment with your details instead of opening a duplicate — it helps us gauge how many people are affected.
2. **Reload and retry once.** Hard-refresh with `Ctrl+F5`. Transient failures during a deploy resolve on their own, and knowing whether it persists is useful information for your report.
3. **Sanitize.** This repo is public — no passwords, API keys, instance URLs, real `sys_id`s, customer data, or employer-proprietary code. See [SECURITY.md](SECURITY.md).
4. **Security flaw? Stop.** Report it privately — see [SECURITY.md](SECURITY.md). Never post exploit details publicly.

## What makes a report we can act on

- **A specific title.** "Story Pointing returns empty result when the description exceeds ~5000 characters" beats "doesn't work".
- **Exact steps** from opening the app to seeing the problem — the shortest path you can find.
- **Expected vs. actual**, stated plainly.
- **The exact error text**, if there was one. Browser console errors (`F12` → Console) are especially useful; scan them for tokens before pasting.
- **When it happened**, with your timezone. It lets us line your report up against server logs.
- **How often** — every time, intermittently, or once.
- **Browser and device.**

Reports missing the steps to reproduce get the `needs-info` label and stall until someone can fill in the gap, so it's worth the extra two minutes up front.

## What happens next

| Label | Meaning |
|-------|---------|
| `needs-triage` | Received, not yet reviewed |
| `needs-info` | We need more detail from you before we can proceed |
| `confirmed` | Reproduced on our side |
| `cannot-reproduce` | We couldn't trigger it with the steps given |
| `in-progress` | Being worked on |
| `fixed-pending-release` | Fixed, not yet deployed to production |
| `duplicate` / `wont-fix` | Closed, with a reason and a link where relevant |

We close issues once a fix is live. If it's still happening for you after a fix ships, say so on the issue and we'll reopen it.

## Feature requests

Feature requests are genuinely welcome, and are read. They're weighed against the roadmap and against how many people are affected — a request being accepted, and its timing, is never guaranteed. Describing the **problem** rather than the solution you have in mind usually produces a better outcome.

## Conduct

Be respectful — see [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md).

## Rights in what you post

By posting, you confirm you have the right to share the content, and that it contains no confidential information belonging to your employer or clients. Feature suggestions may be implemented without obligation or compensation, and posting here grants you no rights in Agentic Copilot, which remains proprietary software owned by iDevOps LLC.
