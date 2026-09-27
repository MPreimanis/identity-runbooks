# Sign-in outage

## When to use it

Many users can't sign in. Treat it as P1 until you know otherwise.

## First 15 minutes

1. Confirm the scope: one app or all, one site or all, cloud or on-premises.
2. Check Microsoft 365 service health and the Azure status page.
3. Check what changed recently: Conditional Access, certificates and secrets, federation, sync, network and proxy.
4. Open a P1 incident and send the first update.

## Diagnose

- Error codes in the sign-in logs point the way: 53003 is Conditional Access, 50126 wrong passwords, 500121 failed MFA, 50057 disabled accounts.
- The Conditional Access tab of a failed sign-in names the policy involved.

## Workaround

- Roll back the most recent change. For a policy, switch it to report-only.
- If admins are locked out too, follow the break-glass runbook.

## Updates

Send an update every 30 minutes, even when nothing has changed:

```text
Subject: [P1] Sign-in problems, update 2 (09:40)

What's affected: users can't sign in to Microsoft 365 from outside the office.
What we know: it started at 08:55, after a Conditional Access change.
What we're doing: the change has been rolled back and sign-ins are recovering.
Workaround: none needed now; sign out and back in if you're still blocked.
Next update: 10:10, or sooner if anything changes.
```

## After

- Confirm in the sign-in logs that failures are back to normal before closing.
- Hold a post-incident review within five working days: timeline, root cause, what helped, and actions with owners.
- Open a problem record if the root cause needs more work.
