# roblox-proxy
Creates a proxy server, utilizing HttpService to mask requests behind Roblox gameserver IPs.

This version is lazily thrown together for demo. purposes, expect a more efficient rewrite.

# Features
- Expandable IP pool, just open more gameservers using game.rbxlx

# TODO
- Randomization of game.rbxlx, to prevent future mass-bans based on hashes
- Reuse of previously generated games

# Setup
```bash
pip install -U git+https://github.com/h0nde/rockblox.git
pip install -r requirements.txt
```

# Usage
Port forward TCP :80

```bash
python3 proxy.py "yourrobloxcookie"
```

```bash
curl --proxy http://localhost:3337 -k http://ip-api.com/json
```
