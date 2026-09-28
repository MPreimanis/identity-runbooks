# Joiner

## When to use it

HR has confirmed a new starter. Start at least three working days before the start date.

## Access needed

User Administrator (or the joiner automation), Groups Administrator for access groups, and Authentication Administrator to issue a Temporary Access Pass.

## Steps

1. Check that the request comes from HR and includes the employee ID, start date, department, job title, manager and location.
2. Search for an existing account with the same employee ID. A rehire gets the old account back, not a second one.
3. Create the account.
   - Hybrid: create it in Active Directory in the right OU. It reaches Entra ID with the next sync, within about 30 minutes.
   - Cloud-only: create it in Entra ID or run the joiner script.
   - Use the naming convention for the UPN, and set the usage location, or licences can't be assigned.
4. Birthright access comes from department and role: dynamic groups pick the user up automatically, and licences come from group-based licensing.
5. Anything beyond birthright goes through an access request approved by the resource owner. Don't copy access from a colleague's account.
6. Prepare the device and assign it to the user.
7. On day one, issue a one-time Temporary Access Pass and give it to the manager through the agreed channel. The user signs in with it and registers a passkey in Microsoft Authenticator.

## Check

- The user can sign in and has registered MFA.
- Licences, mailbox and group memberships match the role.

## Rollback

If the start is cancelled, disable the account, remove its access, and delete it after the retention period.

## Escalate

Sync errors go to the identity team. Licence shortages go to the licence owner.

## Record

In the ticket: employee ID, account, groups, licences, and that a TAP was issued. Don't write down the pass itself.
