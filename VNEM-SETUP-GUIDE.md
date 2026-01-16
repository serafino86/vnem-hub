# 🚀 VNEM Alliance Hub - Complete Setup Guide

**Version 1.2.0 - Updated with Latest Features**

Powered by NGC Alliance Hub Technology  
All latest fixes included!

---

## ✨ WHAT'S NEW IN THIS VERSION:

✅ **Multi-Building Assignments** - Players can be assigned to multiple buildings (IF START LEFT, etc)  
✅ **LAST TEAM Tracking** - Perfect team A/B separation  
✅ **4 Languages** - English, Italian, French, German support  
✅ **Multi-Language War Room** - Translations for all interfaces  
✅ **Multi-Language Personal Stats** - Complete i18n support  

---

## ✅ What's Already Done

✅ Backend deployed: `https://script.google.com/macros/s/AKfycbwrG3roacA0iqTt15alFalSOzjSUpz_VTs2WgKC6MnVqyk0GD1CwkaeMxbbYINk8Gwv/exec`  
✅ All HTML files configured with correct URL  
✅ System customized for VNEM branding  
✅ Latest bug fixes included  

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
   F: BUILDING           ← Can contain multiple buildings!
   G: LAST TEAM          ← NEW! Critical for team separation
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

Upload these documentation files (optional but recommended):
- `README.md`
- `LICENSE.md`
- `.gitignore`
- `UPDATE_GUIDE_LAST_TEAM.md`
- `UPDATE_MULTI_BUILDING_FIX.md`

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
- `language`: "en", "it", "fr", or "de"
- `announcement`: Any important message
- `contact_discord`: Your Discord server (optional)

---

## 📋 Step 4: Test the System (5 minutes)

### Test 1: Basic Functionality

1. **Visit your GitHub Pages URL**
2. You should see "VNEM COMMAND CENTER"
3. Click **"War Room Defense Tracker"**
4. Enter:
   - Player name: "TestPlayer"
   - Alliance code: (your code from B2)
   - Total power: 10000000
5. Click **Submit**
6. Check Google Sheet → New row should appear!

### Test 2: Multi-Language Support

1. Click language buttons: 🇬🇧 🇮🇹 🇫🇷 🇩🇪
2. Interface should change language
3. Test on all 4 apps!

### Test 3: Multi-Building Assignment (⭐ NEW!)

1. Go to **Strategy Manager**
2. Select **Canyon** + **Team A**
3. Assign **TESTPLAYER** to:
   - Building 1
   - Building 3
   - Reserves
4. Click **💾 Save Strategy**
5. Check Google Sheet → Canyon History
6. Column F should show: `"Building 1 (Data Center), Building 3 (Serum Factory), RESERVES"`
7. Click **📋 Load Last Battle**
8. Verify TESTPLAYER appears in ALL 3 positions! ✅

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
🌍 4 Languages - EN/IT/FR/DE

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
├── Canyon History (tournament tracking with LAST TEAM!)
└── Storm History (tournament tracking with LAST TEAM!)
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

### Load Last Battle shows wrong team
- Make sure Canyon History has column G (LAST TEAM)
- Re-save a strategy to populate LAST TEAM

### Multi-building not loading
- Check column F has comma-separated buildings
- Backend must be version 1.2.0+
- Clear browser cache (Ctrl+Shift+R)

---

## 🌟 NEW FEATURES GUIDE

### 1. Multi-Building Assignments

**What it does:**
Allows you to assign the same player to multiple buildings for complex tactics.

**Example:**
```
Building 1: PLAYER1 (main attack)
Building 5: PLAYER1 (IF START LEFT)
Reserves: PLAYER1 (backup)
```

**How it works:**
- System saves all assignments as: `"Building 1, Building 5, RESERVES"`
- Load Last Battle restores player to ALL positions
- Perfect for conditional strategies!

### 2. LAST TEAM Column

**What it does:**
Tracks which team (A or B) each player last played in.

**Why it matters:**
- Prevents confusion when player has history in both teams
- Load Last Battle loads ONLY correct team
- 100% accurate team separation

### 3. Multi-Language Support

**Languages:**
- 🇬🇧 English (EN)
- 🇮🇹 Italian (IT)
- 🇫🇷 French (FR)
- 🇩🇪 German (DE)

**Coverage:**
- Main Hub
- War Room Defense Tracker
- Strategy Manager (including building names!)
- Personal Stats Dashboard

**How to use:**
Click flag buttons at top of each page!

---

## ✅ Checklist

- [ ] Google Sheet created with 3 tabs
- [ ] Headers added to all sheets (including LAST TEAM!)
- [ ] Alliance code set in B2
- [ ] Config added to B1 (optional)
- [ ] GitHub repository created
- [ ] HTML files uploaded
- [ ] GitHub Pages enabled
- [ ] System tested successfully
- [ ] Multi-building assignment tested
- [ ] Language switching tested
- [ ] URL shared with alliance

---

## 📞 Support

For questions or issues:
- **Technical**: Check UPDATE_MULTI_BUILDING_FIX.md
- **Team Separation**: Check UPDATE_GUIDE_LAST_TEAM.md
- **Alliance Setup**: Contact your R4/R5
- **Bug Reports**: GitHub issues

---

## 🎉 You're Ready!

**Welcome to professional alliance management with:**
- ✅ Multi-building tactical support
- ✅ Perfect team separation
- ✅ 4-language support
- ✅ Zero monthly costs
- ✅ Complete data control

---

**Version**: 1.2.0  
**Last Updated**: January 2026  
**Built with ❤️ by Serafino**  
*Revolutionizing Alliance Coordination*
