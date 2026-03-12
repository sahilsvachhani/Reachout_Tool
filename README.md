# Reachout Tool (MailBlast UI)

This project now serves your existing `mailblast` HTML as the main app.

## What it does
- Sign in with Google
- Load recipients (paste or CSV)
- Compose email with merge tags
- Attach one PDF
- Send emails individually via Gmail API

## Run locally
1. Create and activate a virtual environment:
   ```bash
   python3 -m venv .venv
   source .venv/bin/activate
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Start server:
   ```bash
   python app.py
   ```
4. Open:
   [http://localhost:5001](http://localhost:5001)

If you want a different port:
```bash
PORT=5050 python app.py
```

## Google OAuth setup
In Google Cloud Console:
1. Create/select a project.
2. Enable Gmail API.
3. Create OAuth Client ID (`Web application`).
4. Add `http://localhost:5001` to Authorized JavaScript origins.
5. Paste that Client ID into the app setup screen.
