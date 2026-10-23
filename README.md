# TableGrab

English | [中文](languages/README_zh.md) | [Español](languages/README_es.md) | [Deutsch](languages/README_de.md) | [日本語](languages/README_ja.md) | [Français](languages/README_fr.md)

A lightweight browser extension that extracts native HTML tables and ARIA/div data grids from any webpage and exports them as CSV or Excel (XLSX) files with one click.

> Chromium-based · Manifest V3 · Minimal Permissions · Privacy-First

---

## Why TableGrab?

Ever tried to copy a table from a government website or data platform, only to get messy formatting? TableGrab reads the HTML table structure directly and exports clean CSV or XLSX data — no copy-paste errors, no format loss.

| Advantage | Detail |
|-----------|--------|
| 📊 **Auto-Detect** | Scans native `<table>` elements plus ARIA/div grids (role=grid/treegrid/table), shows row × column count |
| 📗 **Excel Export** | Real merged cells, styled/frozen headers, auto column widths, one sheet per table |
| 🔗 **Merged Cells** | Properly handles rowspan/colspan, preserves table structure |
| 🧱 **Div Grids** | Reads MUI DataGrid / AG Grid style grids and de-duplicates pinned-column clones |
| 👁️ **Preview & Columns** | Inspect a table before export, uncheck columns you don't need |
| 📋 **Copy as TSV / Markdown** | Paste straight into Excel, Notion, GitHub or chat apps |
| 📦 **Batch Export** | Export single, selected, or all tables at once |
| 🧩 **Split-Table Headers** | Reassembles Element Plus / Ant Design header+body table pairs |
| 🔤 **No Garbled** | UTF-8 BOM encoding fixes Chinese/CJK character issues in CSV |
| ⚡ **One-Click** | Instant download, no page refresh needed |
| 🔒 **Private** | Minimal permissions, table data never uploaded |

---

## Features

### 🆓 Free

| Feature | Description |
|---------|-------------|
| 📊 **Auto Table Detection** | Finds native tables and ARIA/div grids, filters hidden/layout/clone tables |
| 📗 **XLSX Export** | Multi-sheet workbook with real merged cells, frozen header, column widths |
| 🔗 **Merged Cell Support** | Parses rowspan/colspan, reconstructs proper grid layout |
| 🧩 **Widget-Aware Headers** | Detects split header/body tables used by Element Plus and Ant Design |
| 🧱 **ARIA / Div Grids** | Reads role=grid/treegrid/table structures, including MUI and AG Grid, and folds pinned-column clones back into one table |
| 👁️ **Preview Before Export** | Opens a scrollable preview (up to 50 rows) with per-column checkboxes |
| ☑️ **Column Selection** | Export only the columns you pick; selections are kept as a column mask per table |
| 📋 **Copy TSV / Markdown** | One click copies the table for Excel, Notion, GitHub or chat, honoring the trim setting |
| ✅ **Multi Select** | Check multiple tables, export selected together |
| 📦 **Batch Export** | One CSV per table, or one XLSX workbook with one sheet per table |
| 🔤 **UTF-8 BOM** | Default-on encoding fix for Chinese/CJK characters in CSV |
| 🧹 **Whitespace Cleanup** | Removes extra newlines, spaces, HTML fragments from cells |
| 💡 **Table Highlight** | Hover over table list to highlight corresponding table on page |
| 📁 **Smart Naming** | Auto-generates filename: PageTitle_tables_timestamp.csv / .xlsx |
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

| Store | Link |
|---|---|
| Chrome Web Store | [Install for Chrome](https://chromewebstore.google.com/detail/mekelpcokmdjgoiikpedhojmjappfeji) |
| Microsoft Edge Add-ons | [Install for Edge](https://microsoftedge.microsoft.com/addons/detail/lhoelnklgfdihllglpjkpbinfkejceah) |

> Install only from the official stores above — avoid third-party download sites.

---

## Usage

1. Visit any page with tables or ARIA/div data grids
2. Click the **TableGrab** icon
3. Tables are auto-detected and listed with row × col info
4. Hover to highlight, check to select; use **Preview** to inspect rows and choose columns
5. Click **Export All** or **Export Selected** — or **Copy as TSV / Markdown**
6. CSV or XLSX file downloads automatically

---

## Known Limitations

- Div grids are supported when they expose ARIA roles (`grid`/`treegrid`/`table` with row/cell roles), as MUI DataGrid and AG Grid do. Canvas-rendered grids and div grids without accessible row/cell structure cannot be read
- Tables rendered through pagination or virtual scrolling export only the rows and columns currently present in the DOM
- Cross-origin iframe tables cannot be accessed (browser security restriction)
- Complex dynamically encrypted tables may not parse correctly
- Cells longer than 32,767 characters are truncated to stay within the Excel cell limit

---

## Pricing

The free tier exports up to 5 tables per page. A single-tool license removes that export limit, and the full suite covers the premium features of all VKT extensions.

See [VKT Pricing](https://www.annmax1983.com/pricing.html) for license options and prices.

## Privacy

- ✅ No table data or page content is ever uploaded — parsing and file export happen locally
- ✅ No analytics, no tracking
- ✅ Permissions: `activeTab` + `scripting` + `downloads` + `storage`, plus host access to the official license server
- ✅ `storage` is used only for license key and settings — no browsing data
- 🔑 Premium license activation/validation connects only to the official license server (api.annmax1983.com) — no table data is ever transmitted

---

## Copyright Disclaimer

This extension only reads table structures already loaded on web pages and converts them to CSV or XLSX format for local download. All table data and web page content copyright belong to the original website. Users shall not use exported data for commercial reproduction, unauthorized redistribution or other copyright-infringing behaviors. All legal liabilities arising from improper use shall be borne solely by the user.

---

## ❤️ Support

**[👉 Ko-fi — Buy Me a Coffee](https://ko-fi.com/annmax?ref=tablegrab)**

---

> **Note:** This repository is for **project showcase purposes only**. Full source code will **not** be published here.
