# Leaver

## When to use it

HR confirms a leaving date. For a dismissal, act immediately: the account should be disabled before or during the meeting where the person is told.

## Access needed

User Administrator, Exchange Administrator for the mailbox, and Intune Administrator for devices. For hybrid users, rights to disable accounts in Active Directory.

## Steps

1. Confirm with HR: last day, normal or immediate, manager, and what should happen to mail and files.
2. Disable the account. For hybrid users, disable it in Active Directory; a change made only in Entra ID is overwritten by the next sync.
3. Revoke sessions. Apps that support continuous access evaluation react almost at once; in other apps an existing token stays valid until it expires, typically within 60 to 90 minutes.
4. Reset the password (in Active Directory for hybrid users).
5. Remove group memberships, app assignments, directory roles and PIM eligibility. Keep a list of what you removed.
6. Convert the mailbox to a shared mailbox, or give the manager access, according to policy. Set an automatic reply.
7. Give the manager access to OneDrive files that need to be kept, before the retention period ends.
8. Retire or wipe company devices in Intune, and collect the hardware.
9. Remove licences once the mailbox is converted.
10. Rotate shared credentials the person knew: service accounts, vault entries, Wi-Fi keys.
11. Remove accounts in applications that don't use single sign-on. Check the application inventory.
12. Delete the account after the agreed retention period.

## Check

- No successful sign-ins in the logs after the account was disabled.
- No group memberships or role assignments remain.
- Devices show as retired or wiped.

## Rollback

If the wrong account was disabled or the date moves, re-enable it (in Active Directory for hybrid users) and restore access from the list made in step 5.

## Escalate

A dismissal with a risk of data theft goes to the security team before step 2.

## Record

Each step with its time. The leaver script in identity-automation writes this log for you.
