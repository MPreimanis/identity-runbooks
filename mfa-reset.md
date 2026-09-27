# MFA reset

## When to use it

A user has lost their phone, has a new one, or can't complete MFA.

Helpdesk MFA resets are a favourite social engineering target: attackers call pretending to be an employee. Verifying identity is the most important step in this runbook.

## Access needed

Authentication Administrator. Privileged Authentication Administrator for admin accounts.

## Steps

1. Verify identity before changing anything. Use one of these:
   - A video call with the camera on, compared with a known photo or a person who knows them.
   - A call back to the phone number in HR records, never the number they called from.
   - Confirmation from their manager through a separate channel.

   Details anyone can find, such as a birthday or an employee ID, are not proof.
2. Look at the account's recent sign-ins and risk status. If anything looks wrong, stop and follow the compromised account runbook.
3. Remove the lost method, or require the user to register MFA again.
4. Issue a one-time Temporary Access Pass with a short lifetime and give it through the verified channel.
5. The user registers a new method, ideally a passkey in Microsoft Authenticator.
6. If the lost phone was a company device, retire or wipe it in Intune.

## Check

The user can sign in, the audit log shows the new method, and the old one is gone.

## Rollback

If the user turns out not to be who they claimed, follow the compromised account runbook at once.

## Escalate

Any doubt about identity goes to the security team. Resets for admin accounts need a second person to approve.

## Record

How identity was verified, who verified it, and what changed.
