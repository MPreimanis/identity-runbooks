# Conditional Access change

## When to use it

Any new, changed or deleted Conditional Access policy.

## Access needed

Conditional Access Administrator, activated through PIM.

## Steps

1. Raise a change: what changes, why, who is affected, and how to roll back.
2. Export the current policies so you have a backup.
3. Create or change the policy in report-only mode.
4. Leave it for at least a week, then read the impact in the Conditional Access insights and reporting workbook and in the report-only results in the sign-in logs.
5. Run What If for the edge cases: an admin, a guest, a synced account, a break-glass account.
6. Enforce it for a pilot group, starting with IT.
7. Tell people what changes and when, and where to get help.
8. Enforce in waves, watching sign-in failures and helpdesk tickets for 48 hours after each one.
9. Close the change and update the documentation.

## Rollback

Switch the policy back to report-only. Don't delete it: that loses the configuration and the history.

## Exclusions

Never exclude people one by one. Use an exclusion group with an owner, a reason and a review date.

## Escalate

If admins are locked out, follow the break-glass runbook.

## Record

The change record, the report-only findings, and the date each wave went live.
