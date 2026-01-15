# 🚀 VNEM Alliance Hub - Setup Guide

**Quick setup guide for VNEM alliance leaders**

---

## ✅ What's Already Done

✅ Backend deployed: `https://script.google.com/macros/s/AKfycbwrG3roacA0iqTt15alFalSOzjSUpz_VTs2WgKC6MnVqyk0GD1CwkaeMxbbYINk8Gwv/exec`  
✅ All HTML files configured with correct URL  
✅ System customized for VNEM branding  

---

## 📋 Step 1: Google Sheet Setup (5 minutes)

1. **Open your Google Sheet** with backend
2. **Create these sheets** (tabs):
   - `Data` (main data)
   - `Canyon History` (Canyon tournament tracking)
   - `Storm History` (Desert Storm tournament tracking)

3. **Setup Data sheet** headers (Row 1):
   ```
   A: Player Name
   B: Alliance Code (put your code in B2)
   C: Total Power
   D: Missiles
   E: Aircraft
   F: Tanks
   G: Timestamp
   ```

4. **Setup Canyon History** headers (Row 1):
   ```
   A: PLAYER NAME
   B: PARTICIPATIONS
   C: LAST DATE
   D: TEAM A
   E: TEAM B
   F: BUILDING
   G: LAST TEAM
   ```

5. **Setup Storm History** headers (Row 1):
   ```
   Same as Canyon History (copy row 1)
   ```

6. **Set Alliance Code** in Data sheet, cell B2:
   ```
   Example: VNEM2025
   ```
   ⚠️ Keep this secret! Only share with R4/R5

---

## 📋 Step 2: GitHub Pages Setup (10 minutes)

### Option A: New Repository

1. Go to **https://github.com/new**
2. Repository name: `vnem-alliance-hub` (or your choice)
3. Set to **Public**
4. Click **Create repository**

### Option B: Existing Repository

1. Go to your repository
2. Click **Upload files**

### Upload Files:

Upload these 4 HTML files:
- `index.html` (main hub)
- `war-room-defense-tracker.html`
- `alliance-strategy-ENHANCED.html`
- `ngc-personal-stats.html`

Upload these documentation files (optional):
- `README.md`
- `LICENSE.md`
- `.gitignore`

### Enable GitHub Pages:

1. Go to **Settings** → **Pages**
2. Source: **Deploy from a branch**
3. Branch: **main** (or master)
4. Folder: **/ (root)**
5. Click **Save**

Wait 2-3 minutes, your site will be live at:
```
https://[your-username].github.io/[repo-name]/
```

---

## 📋 Step 3: Configure Alliance Branding (Optional)

In your Google Sheet, cell **B1**, add JSON config:

```json
{
  "alliance_name": "VNEM",
  "server": "YOUR_SERVER_NUMBER",
  "primary_color": "#2196f3",
  "secondary_color": "#64b5f6",
  "accent_color": "#42a5f5",
  "logo_url": "",
  "language": "en",
  "announcement": "",
  "show_announcement": "false",
  "contact_discord": "",
  "contact_email": ""
}
```

Change:
- `server`: Your server number (e.g., "1234")
- `logo_url`: Your alliance logo (optional)
- `language`: "en", "it", or "fr"
- `announcement`: Any important message
- `contact_discord`: Your Discord server (optional)

---

## 📋 Step 4: Test the System (5 minutes)

1. **Visit your GitHub Pages URL**
2. You should see "VNEM COMMAND CENTER"
3. Click **"War Room Defense Tracker"**
4. Enter:
   - Player name: "TestPlayer"
   - Alliance code: (your code from B2)
   - Total power: 10000000
5. Click **Submit**
6. Check Google Sheet → New row should appear!

---

## 📋 Step 5: Share with Alliance

### For R4/R5 Only:

Share the **alliance code** (from B2) with trusted members only.

### For All Members:

Share the main URL:
```
https://[your-username].github.io/[repo-name]/
```

### Quick Start Message Template:

```
🎯 VNEM Alliance Hub is LIVE!

📍 Visit: [YOUR_URL]
🔐 Alliance Code: [PROVIDED_BY_R4]

Features:
🎮 War Room - Submit your power daily
🗺️ Strategy Manager - Canyon & Desert Storm
📊 Personal Stats - Track your growth

Questions? Ask R4/R5
```

---

## 🎯 Quick Reference

### URLs Structure:
```
Main Hub:     /
War Room:     /war-room-defense-tracker.html
Strategy:     /alliance-strategy-ENHANCED.html
Stats:        /ngc-personal-stats.html
```

### Backend URL:
```
https://script.google.com/macros/s/AKfycbwrG3roacA0iqTt15alFalSOzjSUpz_VTs2WgKC6MnVqyk0GD1CwkaeMxbbYINk8Gwv/exec
```

### Google Sheet Structure:
```
📊 Your Spreadsheet
├── Data (main data storage)
├── Canyon History (tournament tracking)
└── Storm History (tournament tracking)
```

---

## 🆘 Troubleshooting

### "Config load error"
- Check cell B1 has valid JSON
- Or leave B1 empty (uses defaults)

### "Invalid alliance code"
- Check B2 in Data sheet
- Code is case-sensitive

### "Failed to submit data"
- Check backend URL is correct
- Verify Apps Script is deployed as "Web app"
- Check "Who has access" = "Anyone"

### Players can't access
- Verify GitHub Pages is enabled
- Check repository is Public
- Wait 2-3 minutes after enabling Pages

---

## 📞 Support

- **Technical Issues**: Check INSTALLATION.md
- **Feature Questions**: See README.md
- **Updates**: See UPDATE_GUIDE_LAST_TEAM.md

---

## ✅ Checklist

- [ ] Google Sheet created with 3 tabs
- [ ] Headers added to all sheets
- [ ] Alliance code set in B2
- [ ] Config added to B1 (optional)
- [ ] GitHub repository created
- [ ] HTML files uploaded
- [ ] GitHub Pages enabled
- [ ] System tested successfully
- [ ] URL shared with alliance

---

**🎉 You're ready to go! Welcome to professional alliance management!**

*Built with ❤️ by Serafino | Powered by NGC Alliance Hub Technology*
