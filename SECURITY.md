# Security & Privacy Policy

Author: iDevOpsLLC

This repository is the **public issue tracker** for [Agentic Copilot](https://ai.nowidevops.com). Anything posted here is world-readable, indexed by search engines, and retained in the GitHub API and event archives even after deletion.

## Reporting a security vulnerability — privately

**Do not open a public issue for a suspected vulnerability.**

If you believe you have found a security flaw in Agentic Copilot (authentication bypass, data exposure between accounts, injection, privilege escalation, exposed keys, etc.):

1. Use **[GitHub private vulnerability reporting](https://github.com/nowidevops/issues/security/advisories/new)** — reports there are visible only to the maintainers.
2. Or contact iDevOps LLC through [ai.nowidevops.com](https://ai.nowidevops.com) and state that the message concerns a security issue.

Please include: what you observed, the steps to reproduce it, the impact you believe it has, and the date/time of your test. Do not post proof-of-concept payloads, tokens, or captured data publicly.

**What we ask of you:** test only against your own account, do not access or modify other users' data, do not run denial-of-service or automated scanning against the production service, and give us reasonable time to fix the issue before disclosing it.

**What you can expect:** acknowledgement of your report, an assessment, and credit in the fix notes if you'd like it. This is a good-faith process, not a paid bug bounty program.

Vulnerabilities in the **ServiceNow platform itself** are not ours to fix — report those to [ServiceNow Support](https://support.servicenow.com).

## Never post sensitive data in issues

| Category | Examples | Post this instead |
|----------|----------|-------------------|
| Credentials | passwords, API keys, OAuth secrets, session tokens, any key you pasted into the app | *(omit entirely)* |
| Instance identity | `acme.service-now.com`, instance sys IDs | `<instance>.service-now.com` |
| Record data | real `sys_id`s, INC/CHG/RITM numbers, customer records | `<sys_id>`, `INC0000000` |
| People | your account email, employee or customer names, phone numbers | *(omit — we'll ask privately)* |
| Proprietary code | scripts belonging to your employer or client | a minimal, rewritten example |
| Network | internal hostnames, IPs, VPN or proxy details | `<internal-host>` |

Screenshots and browser-console dumps are the most common leak source — crop them and check for tokens in URLs before uploading.

## If you posted something sensitive

1. **Edit or delete the comment immediately.** This limits exposure but does **not** guarantee removal from caches or GitHub's event archive.
2. **Rotate the secret.** If an API key, password, or token was exposed, treat it as compromised and rotate it now. Deleting the post is not a substitute.
3. **Tell us** through the private channels above so we can remove the content and, if needed, ask GitHub Support to purge cached views. Don't repeat the sensitive value in your message.

## Scope

No Agentic Copilot source code is published in this repository. Reports about this repository's own content (templates, documentation) are welcome as normal public issues.
