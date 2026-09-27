# identity-runbooks

Operational runbooks for identity and access work in a Microsoft Entra ID environment, hybrid or cloud-only. They are written to be followed during real work, including at 3 a.m.: when to use each one, what access you need, the steps in order, how to check the result, how to roll back, and when to escalate.

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

Every runbook has the same sections: when to use it, access needed, steps, check, rollback, escalate, and record. Adapt names, tools and approvers to your organisation before using them.

## Licence

MIT
