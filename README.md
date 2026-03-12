# TeleWatcher

> A Telegram monitoring userbot that preserves deleted and edited messages, and recovers deleted media files on demand.

**Status:** Private Beta · **Version:** 1.1 · **Platform:** Telegram (MTProto API)

---

## What it does

Telegram doesn't let you see messages after they've been deleted or edited. TeleWatcher connects to your account as an additional session and captures that data before it disappears.

## How it works

1. You authorize your Telegram account via MTProto API, the same process as adding a new device
2. TeleWatcher runs as a background session on your account
3. When a message is deleted or edited, it is captured and stored encrypted
4. When a media file is deleted, it is automatically delivered
   to you if you have an active subscription tier that includes
   media monitoring

TeleWatcher never stores your Telegram password or verification code. Only a session key (authentication token) is stored to maintain the connection. You can revoke access at any time from Telegram Settings → Devices → Active Sessions.

---

## Privacy and security

- All message text, metadata are encrypted at rest with AES-256-GCM
- Media files are stored without encryption for 24 hours, then permanently deleted
- Data is stored on servers in San Francisco, USA
- Users can wipe all data instantly with `/delete_account`

Full details in the legal documents below.

---

## Legal

| Document         | Link                                         |
| ---------------- | -------------------------------------------- |
| Terms of Service | [TERMS_OF_SERVICE.md](./TERMS_OF_SERVICE.md) |
| Privacy Policy   | [PRIVACY_POLICY.md](./PRIVACY_POLICY.md)     |

teleWatcher is an independent project. It is not affiliated with, authorized by, or endorsed by Telegram Messenger Inc. Use of this service may violate Telegram's Terms of Service. You use it at your own risk.

---

## Status and access

This project is currently in private Beta. Access is by invitation only and requires administrator approval.

To request access or ask a question, contact us at **botb86792@gmail.com**

---

## Developers

Built by [Galaxy-craft](https://github.com/Galaxy-craft) and [Bclayn](https://github.com/bclayn24), independent developers based in Uzbekistan.

---

_All rights reserved. See [LICENSE](./LICENSE) for terms._
