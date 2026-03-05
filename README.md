{
  "name": "skillshub-backend",
  "version": "1.0.0",
  "main": "skillshub_server.js",
  "scripts": {
    "start": "node skillshub_server.js"
  },
  "dependencies": {
    "express": "^4.18.2",
    "cors": "^2.8.5"
  }
}
```

**Step 2 — Deploy on Railway**

1. Go to **railway.app** → Sign up with your GitHub account (free)
2. Click **New Project → Deploy from GitHub repo**
3. Select `skillshub-backend`
4. Railway auto-detects it's Node.js and deploys it
5. Click **Settings → Networking → Generate Domain**
6. You get a permanent URL like: `https://skillshub-backend-production.up.railway.app`

**Step 3 — Update the bot with the live URL**

Once you have that Railway URL, I update one line in the bot:
```
const API_URL = 'https://skillshub-backend-production.up.railway.app';
