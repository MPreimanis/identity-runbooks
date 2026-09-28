# identity-runbooks

Runbooks for identity and access work in Microsoft Entra ID, for hybrid or cloud-only setups. Each one says when to use it and what access you need, then gives the steps in order, how to check the result, how to roll back, when to escalate and what to write down.

| Runbook | Use it when |
|---|---|
| [Joiner](joiner.md) | HR confirms a new starter |
| [Mover](mover.md) | Someone changes role, department or manager |
| [Leaver](leaver.md) | Someone leaves, including immediate dismissals |
| [MFA reset](mfa-reset.md) | A user lost their phone or can't complete MFA |
| [Break-glass access](break-glass.md) | Normal admin access has failed |
| [Conditional Access change](conditional-access-change.md) | Any new, changed or deleted policy |
| [Compromised account](compromised-account.md) | Signs that someone else is using an account |
| [Sign-in outage](sign-in-outage.md) | Many users can't sign in (P1) |

Names, tools and approvers are kept generic, so adapt them to your organisation before using them.

## Licence

MIT
