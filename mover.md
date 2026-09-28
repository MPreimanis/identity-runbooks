# Mover

## When to use it

HR records a change of department, role, manager or location.

## Access needed

User Administrator, Groups Administrator, and the owners of any application roles involved.

## Steps

1. Confirm the effective date with HR.
2. Update the attributes at the source: in HR, or in Active Directory for hybrid users. Dynamic groups and group-based licences recalculate on their own.
3. List the person's current access and compare it with what the new role needs.
4. Add access for the new role through the normal request and approval process.
5. Remove access the new role doesn't need. If a handover needs overlap, agree an end date (two weeks at most) and put it in the ticket.
6. Review privileged roles and PIM eligibility. A new role means a new justification.
7. Ask application owners to update roles held inside their applications.

## Check

After the overlap ends, the person's access matches the new role and nothing from the old one remains.

## Rollback

If the move is cancelled, restore the previous attributes and access from the ticket record.

## Escalate

Access nobody can explain goes to the security team as a finding.

## Record

What was added, what was removed, who approved it, and the end date of any overlap.

## Common mistake

Adding the new access and forgetting to remove the old. After a few moves, someone can end up with the access of three different roles.
