# TableGrab

English | [中文](languages/README_zh.md) | [Español](languages/README_es.md) | [Deutsch](languages/README_de.md) | [日本語](languages/README_ja.md) | [Français](languages/README_fr.md)

A lightweight browser extension that extracts HTML tables from any webpage and exports them as CSV files with one click.

> Chromium-based · Manifest V3 · Minimal Permissions · Local Only

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
| 🔒 **Private** | Only3 permissions, zero data upload |

---

## Features

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

## Privacy

- ✅ Zero data upload — all processing happens locally
- ✅ No analytics, no tracking, no network requests
- ✅ Only `activeTab` + `scripting` + `downloads` permissions

---

## Copyright Disclaimer

This extension only reads HTML table structures already loaded on web pages and converts them to CSV format for local download. All table data and web page content copyright belong to the original website. Users shall not use exported data for commercial reproduction, unauthorized redistribution or other copyright-infringing behaviors. All legal liabilities arising from improper use shall be borne solely by the user.

---

## ❤️ Support

**[👉 Click here to support](https://annmax1983.github.io/TableGrab/)**

---

> **Note:** This repository is for **project showcase purposes only**. Full source code will **not** be published here.
