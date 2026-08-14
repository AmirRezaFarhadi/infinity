# Security Policy

## Current status

The current legacy implementation is not approved for deployment because it includes flows that request sensitive Telegram authentication material through chat messages. Do not run the account-authentication flow and do not share any secret with it.

## Reporting

Report concerns through GitHub’s private security advisory flow. Never disclose tokens, login codes, passwords, session files, phone numbers, API IDs, API hashes, channel identifiers, or user messages in a public issue.

## Redesign requirements

Any replacement must avoid collecting login codes and passwords, keep secrets under the user’s local control, use explicit confirmation before actions, and document how user data is handled and deleted.
