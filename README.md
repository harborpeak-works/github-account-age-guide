# GitHub account age: why it matters and how to check it

Fresh GitHub accounts run into invisible walls. Actions minutes get
throttled, automation gets challenged, OAuth apps treat new accounts
with suspicion, and some programs quietly prefer identities that have
been around a while.

## What an aged account buys you

- Fewer anti-abuse challenges on CI and automation
- Smoother third-party OAuth integrations
- An identity that programs and marketplaces take seriously

## Check any account's age

The creation date is public — no login required:

```bash
curl -s https://api.github.com/users/USERNAME | grep created_at
```

```python
import requests
u = requests.get("https://api.github.com/users/USERNAME").json()
print(u["created_at"], u["public_repos"], u["followers"])
```

## Buying an aged account? Read this first

1. **Demand the full set**: username, password, email and the 2FA seed.
   Miss one and the account is never really yours.
2. **Rotate everything on day one**: new password, new authenticator,
   remove the seller's recovery methods.
3. **Warm it gently**: a few normal actions over the first days beat
   instant heavy automation.

## Where I get them

👉 https://shop.hailizi.de/ — GitHub accounts by age tier
(new / 15d+ / 30d+ / 120d+ / 180d+), plus Azure subscriptions.
Instant delivery, full credentials including email and 2FA seed.

---

*Useful? A star helps others find it.*
