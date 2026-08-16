# TableGrab

English | [中文](languages/README_zh.md) | [Español](languages/README_es.md) | [Deutsch](languages/README_de.md) | [日本語](languages/README_ja.md) | [Français](languages/README_fr.md)

A lightweight browser extension that extracts HTML tables from any webpage and exports them as CSV files with one click.

> Chromium-based · Manifest V3 · Minimal Permissions · Privacy-First

---

## Why TableGrab?

Ever tried to copy a table from a government website or data platform, only to get messy formatting? TableGrab reads the HTML table structure directly and exports clean CSV data — no copy-paste errors, no format loss.

| Advantage | Detail |
|-----------|--------|
| 📊 **Auto-Detect** | Scans all HTML tables on the page, shows row × column count |
| 🔗 **Merged Cells** | Properly handles rowspan/colspan, preserves table structure |
| 📦 **Batch Export** | Export single, selected, or all tables at once |
| 🔤 **No Garbled** | UTF-8 BOM encoding fixes Chinese/CJK character issues |
| ⚡ **One-Click** | Instant download, no page refresh needed |
| 🔒 **Private** | Minimal permissions, table data never uploaded |

---

## Features

### 🆓 Free

| Feature | Description |
|---------|-------------|
| 📊 **Auto Table Detection** | Finds all valid HTML tables, filters hidden/layout tables |
| 🔗 **Merged Cell Support** | Parses rowspan/colspan, reconstructs proper grid layout |
| 📋 **Single Export** | Export any one table as CSV |
| ✅ **Multi Select** | Check multiple tables, export selected together |
| 📦 **Batch Export** | One-click export all tables on the page |
| 🔤 **UTF-8 BOM** | Default-on encoding fix for Chinese/CJK characters |
| 🧹 **Whitespace Cleanup** | Removes extra newlines, spaces, HTML fragments from cells |
| 💡 **Table Highlight** | Hover over table list to highlight corresponding table on page |
| 📁 **Smart Naming** | Auto-generates filename: PageTitle_tables_timestamp.csv |
| 🔒 **Up to 5 tables/page** | Free tier exports the first 5 tables detected on each page |

### ⭐ Premium (License)

| Feature | Description |
|---------|-------------|
| 📦 **Unlimited Exports** | No 5-table limit — export every table on any page |
| 🔄 **All Free Features** | Everything above, no restrictions |

---

## Preview

<p align="center">
  <img src="icons/icon128.png" alt="TableGrab Icon" width="80">
</p>

---

## Supported Browsers

| Browser | Status |
|---------|--------|
| Google Chrome | ✅ Fully supported |
| Microsoft Edge | ✅ Fully supported |

---

## Installation

1. Open `chrome://extensions/` or `edge://extensions/`
2. Enable **Developer mode**
3. Click **Load unpacked** and select the project folder

---

## Usage

1. Visit any page with HTML tables
2. Click the **TableGrab** icon
3. Tables are auto-detected and listed with row × col info
4. Hover to highlight, check to select
5. Click **Export All** or **Export Selected**
6. CSV file downloads automatically

---

## Known Limitations

- Only supports HTML `<table>` elements — image tables, Canvas tables, virtual JS tables not supported
- Cross-origin iframe tables cannot be accessed (browser security restriction)
- Complex dynamically encrypted tables may not parse correctly

---

## Pricing

| Plan | Price | Details |
|------|-------|--------|
| 🆓 Free | $0 | Up to 5 tables per page |
| ⭐ Single Tool | $2.99/mo or $9.99 lifetime | Unlimited TableGrab exports |
| 🏆 Full Suite | $3.99/mo or $19.99 lifetime | All VKT extensions premium |

See [VKT Pricing](https://www.annmax1983.com/pricing.html) for details.

## Privacy

- ✅ No table data or page content is ever uploaded — parsing and CSV export happen locally
- ✅ No analytics, no tracking
- ✅ Permissions: `activeTab` + `scripting` + `downloads` + `storage`, plus host access to the official license server
- ✅ `storage` is used only for license key and settings — no browsing data
- 🔑 Premium license activation/validation connects only to the official license server (api.annmax1983.com) — no table data is ever transmitted

---

## Copyright Disclaimer

This extension only reads HTML table structures already loaded on web pages and converts them to CSV format for local download. All table data and web page content copyright belong to the original website. Users shall not use exported data for commercial reproduction, unauthorized redistribution or other copyright-infringing behaviors. All legal liabilities arising from improper use shall be borne solely by the user.

---

## ❤️ Support

**[👉 Ko-fi — Buy Me a Coffee](https://ko-fi.com/annmax?ref=tablegrab)**

---

> **Note:** This repository is for **project showcase purposes only**. Full source code will **not** be published here.
