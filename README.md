# Bridgestone AV Room Portal

Mobile-first room portal prototype for Bridgestone Americas managed AV services. Scan a QR code in any conference room to view room info, check system status, and submit support tickets.

## Features

- **Room Info**: Equipment list, connection instructions, technology available
- **Live Status**: Device-level green/amber/red health indicators
- **Support Tickets**: Photo capture, voice memo, text — under 30 seconds
- **Zero Friction**: No login, no app install, room auto-populated from QR code

## Deploy to Vercel

1. Push this repo to GitHub
2. Go to [vercel.com](https://vercel.com) → New Project → Import this repo
3. Deploy (zero config needed — `vercel.json` handles it)
4. Your portal is live at `your-project.vercel.app`

## QR Code Setup

Each room gets a unique URL with the room ID as a parameter:

```
https://your-project.vercel.app/?room=1204
https://your-project.vercel.app/?room=1505
https://your-project.vercel.app/?room=0301
```

Generate QR codes for each URL and print on vinyl stickers for desk placement.

## Room Configuration

Room data is currently hardcoded in `public/index.html` for the prototype demo. In production, this would pull from a SharePoint list or API on Bridgestone's Microsoft tenant.

## Built For

Systems Innovation by LMG — Bridgestone Americas managed AV services proposal.

---

*Confidential — Internal Use Only*
