# Spyne · Delivery Appraisal Dashboard 2025–26

Live performance dashboard for the Delivery department, powered by Google Sheets.

## 🔗 Live Dashboard
**https://YOUR-USERNAME.github.io/spyne-appraisal-dashboard/**

## ✨ Features
- 📊 Overview with KPIs + charts
- 📋 All Employees — filter by name, eligibility, rating; sort any column
- 👤 Employee Cards — individual profiles with photos
- 📈 Analytics — 6 chart dimensions
- 🔍 Drill Down — by rating, factor, eligibility, leaves
- ↺ One-click data refresh (re-fetches from Google Sheets live)

## 🔄 How data stays live
The dashboard fetches from your **published Google Sheets CSV** on every page load.
No backend needed — pure HTML + JavaScript.

## 📋 Setup

### 1. Deploy to GitHub Pages
```
1. Fork or create repo
2. Upload index.html
3. Settings → Pages → Deploy from main branch
4. Visit https://YOUR-USERNAME.github.io/REPO-NAME/
```

### 2. Update the Google Sheet URL
If you change the sheet, update line ~270 in `index.html`:
```javascript
var APPRAISAL_CSV = 'YOUR_NEW_PUBLISHED_CSV_URL';
```

### 3. Publish your sheet
Google Sheets → **File → Share → Publish to web**
→ Choose sheet tab → CSV → Publish → Copy URL → paste into index.html

## 📁 Files
| File | Purpose |
|------|---------|
| `index.html` | The entire dashboard (single file) |
| `README.md` | This file |

## 🛠️ Local development
Open `index.html` via a local server (not `file://`):
```bash
# Python
python3 -m http.server 8080
# then open http://localhost:8080
```

---
Built with ❤️ for Spyne.ai Delivery team
