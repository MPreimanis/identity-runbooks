# Break-glass access

## When to use it

Normal admin access has failed: a Conditional Access policy locked admins out, MFA is down, or federation or sync broke sign-in.

## The accounts

Two cloud-only accounts on the `onmicrosoft.com` domain with permanent Global Administrator. They sign in with FIDO2 security keys kept in two separate secure places, are excluded from Conditional Access (or covered by one dedicated policy), and every sign-in raises an alert.

## Steps

1. Open an incident ticket and tell the security lead that a break-glass account is about to be used.
2. Collect a security key according to the storage procedure. Two people, if your procedure allows it.
3. Sign in from a known, healthy device.
4. Do only what the emergency needs, such as switching a faulty policy to report-only. Note every action as you go.
5. Sign out and return the key.

## Check

The sign-in alert fired within minutes. If it didn't, fixing the alert is part of closing the incident.

## After use

- Review the account's audit log and match it against your notes.
- Replace the key if it left secure storage for longer than planned.
- Find out why normal access failed, and fix that.

## Testing

Every quarter, sign in with each account, confirm the access and the alert, and record the test.

## Record

Who used it, when, why, and every action taken.
