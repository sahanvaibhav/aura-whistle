# Aura — Whistle

Lifestyle super-app (single-file): **Whistle** social · Circles · Space · Pay · **Ask Aura** (Google Search + Gemini).

## Live URL (after you enable Pages)

https://sahanvaibhav.github.io/aura-whistle/

## One-time setup (2 minutes)

### 1. Enable GitHub Pages
1. Open https://github.com/sahanvaibhav/aura-whistle/settings/pages  
2. Under **Build and deployment** → Source → choose **GitHub Actions**  
3. Wait ~1 minute. The site will be live at the URL above.

### 2. Google (Sign-in + Search)
1. Open the live site → **Me** → **API & Google settings**  
2. Paste:
   - **OAuth Client ID** (Web application type)
   - **Custom Search API key**
   - **CX** (Programmable Search Engine ID)
   - Optional: Gemini API key for AI mode
3. In [Google Cloud Console](https://console.cloud.google.com/apis/credentials):
   - Create **OAuth 2.0 Client ID** → Application type: **Web application**
   - **Authorized JavaScript origins** → add exactly:
     ```
     https://sahanvaibhav.github.io
     ```
   - Enable **Custom Search API**
   - Create a search engine at https://programmablesearchengine.google.com (search the whole web) and copy the **cx**

Keys are stored only in your browser `localStorage`. Nothing is sent to any server we control.

## Features
- Whistle: Shorts (video) + Feed + Post (text/photo)
- Circles: messaging
- Space: device toggles + weather
- Aura Pay: local demo wallet
- Ask Aura: Google Custom Search or Gemini
- Google Sign-in (GSI) with profile photo
- Glass UI · no backend required

## Local / download
Open `index.html` in a browser. Google Sign-in will not work on `file://` or plain `http://localhost` until you host on HTTPS and add that origin in Google Cloud.
