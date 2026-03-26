# GitPump 🚀

**Launch Solana tokens on Pump.fun directly from a GitHub comment.**

No dashboards. No API keys. Just drop a comment with your logo and go live.

---

## How It Works

1. Open an issue in this repo
2. Post a comment using the format below
3. The bot launches your token on Pump.fun
4. Your token appears on [gitpump.com](https://gitpump.com)

---

## Launch Command

```
/launch name=YourToken symbol=TICKER
description=Your token description here.
twitter=https://x.com/yourhandle
telegram=https://t.me/yourgroup
website=https://yourwebsite.com
```

**Attach a logo image** (JPG/PNG/GIF/WEBP, max 5MB) to the comment.

### Fields

| Field | Required | Notes |
|---|---|---|
| `name` | ✅ | Token name |
| `symbol` | ✅ | Ticker (e.g. SUS) |
| `description` | ✅ | Short description |
| `twitter` | ❌ | Optional |
| `telegram` | ❌ | Optional |
| `website` | ❌ | Optional |
| Logo image | ✅ | Attached to comment |

---

## Rules

- Max **1 launch per hour** per GitHub user
- Logo must be attached directly to the comment (drag & drop)
- Wallet must have SOL for transaction fees

---

## Live Feed

All launched tokens are visible at **[gitpump.com](https://gitpump.com)**

---

## Self-Hosting

Clone this repo, set the required environment variables, and point your GitHub webhook to your server.

**Required environment variables:**
- `GITHUB_TOKEN` — GitHub personal access token
- `GITHUB_WEBHOOK_SECRET` — Webhook secret
- `SOLANA_PRIVATE_KEY` — Base58 encoded private key
- `DATABASE_URL` — PostgreSQL connection string