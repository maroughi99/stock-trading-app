# Stock Trading Platform - Frontend

Deploy this to Netlify

## Before Deploying:

1. Make sure you've deployed the backend to Render.com first
2. Get your backend API URL (e.g., `https://stock-trading-api-xxxx.onrender.com`)
3. Update the API URL in ALL 4 HTML files (see below)

## Update API URLs:

Open each of these files and find the line with `YOUR_BACKEND_API_URL_HERE`:

- `index.html`
- `dashboard.html`
- `daytrading.html`
- `potential.html`

**Find this:**
```javascript
const API_BASE_URL = window.location.hostname === 'localhost' 
    ? 'http://localhost:5000' 
    : 'YOUR_BACKEND_API_URL_HERE';
```

**Replace with your Render URL:**
```javascript
const API_BASE_URL = window.location.hostname === 'localhost' 
    ? 'http://localhost:5000' 
    : 'https://stock-trading-api-xxxx.onrender.com';
```

## Deploy to Netlify:

1. Go to https://netlify.com
2. Sign up or login
3. Drag this entire folder onto Netlify
4. Wait 30 seconds
5. Your site is live!

## Files in this folder:

- `index.html` - Stock analysis page with charts
- `dashboard.html` - Trading dashboard (500 stocks + crypto)
- `daytrading.html` - Day trading scanner
- `potential.html` - Price potential calculator
- `netlify.toml` - Netlify configuration
- `_headers` - Security headers
