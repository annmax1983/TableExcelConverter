# TableGrab

[English](../README.md) | [中文](README_zh.md) | [Español](README_es.md) | Deutsch | [日本語](README_ja.md) | [Français](README_fr.md)

Eine schlanke Browser-Erweiterung, die native HTML-Tabellen und ARIA/Div-Datengrids von jeder Webseite extrahiert und sie mit einem Klick als CSV- oder Excel-Dateien (XLSX) exportiert.

> Chromium-basiert · Manifest V3 · Minimale Berechtigungen · Datenschutz zuerst

---

## Warum TableGrab?

Schon mal versucht, eine Tabelle von einer Behörden-Website oder Datenplattform zu kopieren, und nur ein chaotisches Format bekommen? TableGrab liest die Tabellenstruktur direkt aus und exportiert saubere CSV- oder XLSX-Daten — keine Kopierfehler, kein Formatverlust.

| Vorteil | Details |
|---------|---------|
| 📊 **Auto-Erkennung** | Scannt alle nativen Tabellen und ARIA/Div-Grids (role=grid/treegrid/table) der Seite, zeigt Zeilen × Spalten |
| 📗 **Excel-Export** | Echte verbundene Zellen, gestaltete/eingefrorene Kopfzeilen, automatische Spaltenbreiten, ein Blatt pro Tabelle |
| 🔗 **Zusammengefasste Zellen** | Behandelt rowspan/colspan korrekt, erhält die Tabellenstruktur |
| 🧱 **Div-Grids** | Liest Grids wie MUI DataGrid / AG Grid und führt duplizierte Fixspalten zusammen |
| 👁️ **Vorschau & Spalten** | Tabelle vor dem Export prüfen und nicht benötigte Spalten abwählen |
| 📋 **Als TSV / Markdown kopieren** | Direkt in Excel, Notion, GitHub oder Chat-Apps einfügen |
| 📦 **Batch-Export** | Einzelne, ausgewählte oder alle Tabellen auf einmal exportieren |
| 🔤 **Keine Zeichenfehler** | UTF-8 BOM-Kodierung behebt Probleme mit chinesischen/CJK-Zeichen |
| ⚡ **Ein Klick** | Sofortiger Download, kein Seiten-Neuladen nötig |
| 🔒 **Privat** | Minimale Berechtigungen, Tabellendaten werden nie hochgeladen |

---

## Funktionen

### 🆓 Kostenlos

| Funktion | Beschreibung |
|----------|--------------|
| 📊 **Auto-Tabellenerkennung** | Findet gültige native Tabellen und ARIA/Div-Grids, filtert versteckte/Layout-Tabellen |
| 📗 **XLSX-Export** | Arbeitsmappe mit mehreren Blättern, echten Verbindungen, eingefrorener Kopfzeile, automatischen Breiten |
| 🔗 **Zusammengefasste Zellen** | Parst rowspan/colspan, rekonstruiert korrektes Rasterlayout |
| 🧱 **ARIA / Div-Grids** | Liest role=grid/treegrid/table-Strukturen (inkl. MUI und AG Grid) und führt Fixspalten-Duplikate zusammen |
| 👁️ **Vorschau vor dem Export** | Scrollbare Vorschau (bis 50 Zeilen) mit Auswahlkästchen pro Spalte |
| ☑️ **Spaltenauswahl** | Nur ausgewählte Spalten exportieren; die Auswahl wird pro Tabelle gemerkt |
| 📋 **TSV / Markdown kopieren** | Ein Klick für Excel, Notion, GitHub oder Chat, unter Beachtung der Leerzeichen-Bereinigung |
| ✅ **Mehrfachauswahl** | Mehrere Tabellen ankreuzen, Auswahl zusammen exportieren |
| 📦 **Batch-Export** | Ein-Klick-Export aller Tabellen auf der Seite |
| 🔤 **UTF-8 BOM** | Standardmäßig aktivierte Kodierungskorrektur für chinesische/CJK-Zeichen |
| 🧹 **Whitespace-Bereinigung** | Entfernt überflüssige Zeilenumbrüche, Leerzeichen und HTML-Fragmente aus Zellen |
| 💡 **Tabellen-Hervorhebung** | Beim Überfahren der Tabellenliste wird die entsprechende Tabelle auf der Seite hervorgehoben |
| 📁 **Intelligente Benennung** | Dateiname wird automatisch generiert: Seitentitel_tabellen_zeitstempel.csv / .xlsx |
| 🔒 **Bis zu 5 Tabellen/Seite** | Kostenlose Stufe exportiert die ersten 5 erkannten Tabellen pro Seite |

### ⭐ Premium (Lizenz)

| Funktion | Beschreibung |
|----------|--------------|
| 📦 **Unbegrenzte Exporte** | Kein 5-Tabellen-Limit — jede Tabelle auf jeder Seite exportieren |
| 🔄 **Alle kostenlosen Funktionen** | Alles oben, ohne Einschränkungen |

---

## Vorschau

<p align="center">
  <img src="icons/icon128.png" alt="TableGrab Symbol" width="80">
</p>

---

## Unterstützte Browser

| Browser | Status |
|---------|--------|
| Google Chrome | ✅ Vollständig unterstützt |
| Microsoft Edge | ✅ Vollständig unterstützt |

---

## Installation

1. Öffne `chrome://extensions/` oder `edge://extensions/`
2. Aktiviere den **Entwicklermodus**
3. Klicke auf **Entpackte Erweiterung laden** und wähle den Projektordner

---

## Verwendung

1. Besuche eine beliebige Seite mit Tabellen oder ARIA/Div-Datengrids
2. Klicke auf das **TableGrab**-Symbol
3. Tabellen werden automatisch erkannt und mit Zeilen × Spalten-Info aufgelistet
4. Überfahren zum Hervorheben, ankreuzen zum Auswählen; mit **Vorschau** Spalten wählen
5. Klicke auf **Alle exportieren**, **Auswahl exportieren** oder **Als TSV / Markdown kopieren**
6. CSV- oder XLSX-Datei wird automatisch heruntergeladen

---

## Bekannte Einschränkungen

- Div-Grids werden unterstützt, wenn sie ARIA-Rollen offenlegen (`grid`/`treegrid`/`table` mit Zeilen-/Zellrollen), wie MUI DataGrid und AG Grid. Canvas-Grids und Div-Grids ohne barrierefreie Zeilen-/Zellstruktur können nicht gelesen werden
- Tabellen mit Paginierung oder virtuellem Scrollen exportieren nur die aktuell im DOM befindlichen Zeilen und Spalten
- Cross-Origin-Iframe-Tabellen können nicht zugegriffen werden (Browser-Sicherheitsbeschränkung)
- Komplex dynamisch verschlüsselte Tabellen werden möglicherweise nicht korrekt geparst
- Zellen mit mehr als 32.767 Zeichen werden auf das Excel-Limit gekürzt

---

## Preise

Die kostenlose Version exportiert bis zu 5 Tabellen pro Seite. Eine Einzellizenz hebt dieses Exportlimit auf, das Komplettpaket deckt die Premium-Funktionen aller VKT-Erweiterungen ab.

Details zu Lizenzoptionen und Preisen: [VKT Preise](https://www.annmax1983.com/pricing.html).

## Datenschutz

- ✅ Es werden nie Tabellendaten oder Seiteninhalte hochgeladen — Parsing und CSV-/XLSX-Export passieren lokal
- ✅ Keine Analytik, kein Tracking
- ✅ Berechtigungen: `activeTab` + `scripting` + `downloads` + `storage`, plus Host-Zugriff auf den offiziellen Lizenzserver
- ✅ `storage` wird nur für Lizenzschlüssel und Einstellungen verwendet — keine Browserdaten
- 🔑 Premium-Lizenzaktivierung/-validierung verbindet sich nur mit dem offiziellen Lizenzserver (api.annmax1983.com) — es werden nie Tabellendaten übertragen

---

## Urheberrechtshinweis

Diese Erweiterung liest nur Tabellenstrukturen, die bereits auf Webseiten geladen sind, und konvertiert sie ins CSV- oder XLSX-Format für den lokalen Download. Alle Tabellendaten und Webseiteninhalte unterliegen dem Urheberrecht der ursprünglichen Website. Nutzer dürfen exportierte Daten nicht für kommerzielle Vervielfältigung, unbefugte Weiterverbreitung oder andere urheberrechtsverletzende Handlungen verwenden. Alle rechtlichen Folgen aus missbräuchlicher Nutzung trägt allein der Nutzer.

---

## ❤️ Support

**[👉 Ko-fi — Kauf mir einen Kaffee](https://ko-fi.com/annmax?ref=tablegrab)**

---

> **Hinweis:** Dieses Repository dient ausschließlich der **Projektpräsentation**. Der vollständige Quellcode wird hier **nicht** veröffentlicht.
