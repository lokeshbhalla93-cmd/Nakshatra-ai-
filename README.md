# 🌙 Nakshatra AI — Deploy Guide

AI-powered Vedic Astrology app. Deploy free on Vercel in 5 minutes.

---

## Step 1 — Upload to GitHub

1. Go to https://github.com and sign in (create account if needed)
2. Click **New repository** → name it `nakshatra-ai` → Create
3. Upload these files/folders:
   - `api/reading.js`
   - `public/index.html`
   - `vercel.json`
   - `package.json`

---

## Step 2 — Deploy on Vercel

1. Go to https://vercel.com and sign in with GitHub
2. Click **Add New → Project**
3. Select your `nakshatra-ai` repository → click **Import**
4. Leave all settings as default → click **Deploy**

---

## Step 3 — Add your Anthropic API Key

1. In Vercel dashboard → your project → **Settings → Environment Variables**
2. Add:
   - **Name:** `ANTHROPIC_API_KEY`
   - **Value:** your key from https://console.anthropic.com
3. Click **Save**
4. Go to **Deployments** → click **Redeploy** (so key takes effect)

---

## Step 4 — Share!

Vercel gives you a free URL like:
`https://nakshatra-ai.vercel.app`

Share this with anyone — works in Chrome, Safari, mobile, everywhere ✦

---

## Files in this project

```
nakshatra-ai/
├── api/
│   └── reading.js      ← Secure backend (hides your API key)
├── public/
│   └── index.html      ← The app frontend
├── vercel.json         ← Routing config
├── package.json        ← Project info
└── README.md           ← This file
```

---

## How it works

Browser → `/api/reading` (your Vercel server) → Anthropic API

Your API key never touches the browser. Safe to share publicly.
