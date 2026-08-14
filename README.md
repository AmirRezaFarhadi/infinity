# Telegram Auto-Post Bot — Legacy Security Notice

> **Do not deploy this version.** The current legacy code path requests account-access material in a chat flow, including login codes and two-factor credentials. Those values must never be collected, displayed, stored, or transmitted by a bot.

## Current status

This repository is retained as a legacy reference only. It is not a supported deployment target and must not be promoted until it has been redesigned and independently reviewed.

## Safe redesign direction

The replacement must remove in-chat account authentication entirely. It should use a user-controlled local authorization process, keep secrets outside the repository, require explicit confirmation before every forward or schedule action, and document retention and deletion of all user data.

## Immediate rule

Never send a Telegram login code, password, API hash, session file, bot token, or personal account information in a chatbot, issue, form, or public repository.

## Contributing

Do not add new production features to this legacy implementation. Contributions are limited to safety documentation, migration planning, test scaffolding for a new architecture, or a safe replacement that meets the requirements in [SECURITY.md](SECURITY.md).

## License

MIT.
