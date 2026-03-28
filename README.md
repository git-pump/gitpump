# GitPump 🚀

**Launch tokens on Solana, Base, and BSC directly from a GitHub comment.**

No dashboards. No API keys. Just drop a comment with your logo and go live.

---

## How It Works

1. [Install the GitPump app](https://github.com/apps/gitpump-bot) on your repo
2. Post a comment using the format below
3. The bot launches your token on your chosen platform
4. Your token appears on [gitpump.com](https://gitpump.com)

---

## Launch Command

```
/launch name=YourToken symbol=TICKER
description=Your token description here.
platform=pumpfun
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
| `platform` | ✅ | See supported platforms below |
| `twitter` | ❌ | Optional |
| `telegram` | ❌ | Optional |
| `website` | ❌ | Optional |
| Logo image | ✅ | Attached to comment |

### Supported Platforms

| platform= | Platform | Network |
|---|---|---|
| `pumpfun` | pump.fun | Solana |
| `bags` | bags.fm | Solana |
| `clanker` | clanker.world | Base |
| `fourmeme` | four.meme | BSC |

---

## Claiming Fees

Trading fees accumulate in your token's launch wallet. To claim:

```
/claim <your_wallet_address>
```

**75% goes to you · 25% goes to GitPump** (after operational costs)

---

## Rules

- Max **1 launch per hour** per GitHub user (failed launches don't count)
- Logo must be attached directly to the comment (drag & drop)
- The bot funds a fresh wallet per launch — no need to send funds yourself

---

## Live Feed

All launched tokens are visible at **[gitpump.com](https://gitpump.com)**
