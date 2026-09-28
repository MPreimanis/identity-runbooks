# Compromised account

## When to use it

Someone else may be using an account. Typical signs are a risk alert, a user reporting an MFA prompt they didn't start, sign-ins from unexpected places, or a new forwarding rule.

Work through the sections in order.

## Access needed

Security Administrator or Global Administrator through PIM, plus Exchange Administrator for mailbox checks.

## Steps

### Contain (first 15 minutes)

1. Disable the account (in Active Directory if it's synced) and revoke its sessions.
2. If it's an admin account, check straight away what it changed.

### Investigate

3. Sign-in logs for the last 30 days: successful sign-ins, IP addresses, apps and devices.
4. Audit logs: new MFA methods, consent grants, app credentials, role changes, Conditional Access changes.
5. Mailbox: inbox rules, forwarding, and sent items.

### Evict

6. Remove what the attacker added: MFA methods, consent grants, app credentials, mailbox rules and forwarding, role assignments.
7. Rotate secrets the user could reach.

### Recover

8. Reset the password, issue a Temporary Access Pass through a verified channel, and have the user register a phishing-resistant method.
9. Re-enable the account and watch its sign-ins for a few days.

### Learn

10. Find the root cause (phishing, password reuse, missing MFA), close the gap for everyone, and add a detection.

## Escalate

- If personal data may have been accessed, involve the data protection officer at once: under GDPR the authority must normally be told within 72 hours of becoming aware of a breach.
- Organisations in scope of NIS2 must send an early warning to their national authority within 24 hours of a significant incident.

## Record

A timeline of what happened and what you did, with times. You'll need it for the post-incident review, and possibly for legal or audit.
