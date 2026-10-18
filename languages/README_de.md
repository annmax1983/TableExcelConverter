# TableGrab

[English](../README.md) | [中文](README_zh.md) | [Español](README_es.md) | Deutsch | [日本語](README_ja.md) | [Français](README_fr.md)

Eine schlanke Browser-Erweiterung, die HTML-Tabellen von jeder Webseite extrahiert und sie mit einem Klick als CSV-Dateien exportiert.

> Chromium-basiert · Manifest V3 · Minimale Berechtigungen · Datenschutz zuerst

---

## Warum TableGrab?

Schon mal versucht, eine Tabelle von einer Behörden-Website oder Datenplattform zu kopieren, und nur ein chaotisches Format bekommen? TableGrab liest die HTML-Tabellenstruktur direkt aus und exportiert saubere CSV-Daten — keine Kopierfehler, kein Formatverlust.

| Vorteil | Details |
|---------|---------|
| 📊 **Auto-Erkennung** | Scannt alle HTML-Tabellen auf der Seite, zeigt Zeilen × Spalten-Anzahl |
| 🔗 **Zusammengefasste Zellen** | Behandelt rowspan/colspan korrekt, erhält die Tabellenstruktur |
| 📦 **Batch-Export** | Einzelne, ausgewählte oder alle Tabellen auf einmal exportieren |
| 🔤 **Keine Zeichenfehler** | UTF-8 BOM-Kodierung behebt Probleme mit chinesischen/CJK-Zeichen |
| ⚡ **Ein Klick** | Sofortiger Download, kein Seiten-Neuladen nötig |
| 🔒 **Privat** | Minimale Berechtigungen, Tabellendaten werden nie hochgeladen |

---

## Funktionen

### 🆓 Kostenlos

| Funktion | Beschreibung |
|----------|--------------|
| 📊 **Auto-Tabellenerkennung** | Findet alle gültigen HTML-Tabellen, filtert versteckte/Layout-Tabellen |
| 🔗 **Zusammengefasste Zellen** | Parst rowspan/colspan, rekonstruiert korrektes Rasterlayout |
| 📋 **Einzeln exportieren** | Eine beliebige Tabelle als CSV exportieren |
| ✅ **Mehrfachauswahl** | Mehrere Tabellen ankreuzen, Auswahl zusammen exportieren |
| 📦 **Batch-Export** | Ein-Klick-Export aller Tabellen auf der Seite |
| 🔤 **UTF-8 BOM** | Standardmäßig aktivierte Kodierungskorrektur für chinesische/CJK-Zeichen |
| 🧹 **Whitespace-Bereinigung** | Entfernt überflüssige Zeilenumbrüche, Leerzeichen und HTML-Fragmente aus Zellen |
| 💡 **Tabellen-Hervorhebung** | Beim Überfahren der Tabellenliste wird die entsprechende Tabelle auf der Seite hervorgehoben |
| 📁 **Intelligente Benennung** | Dateiname wird automatisch generiert: Seitentitel_}_tabellen_zeitstempel.csv |
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

1. Besuche eine beliebige Seite mit HTML-Tabellen
2. Klicke auf das **TableGrab**-Symbol
3. Tabellen werden automatisch erkannt und mit Zeilen × Spalten-Info aufgelistet
4. Überfahren zum Hervorheben, ankreuzen zum Auswählen
5. Klicke auf **Alle exportieren** oder **Auswahl exportieren**
6. CSV-Datei wird automatisch heruntergeladen

---

## Bekannte Einschränkungen

- Unterstützt nur HTML `<table>`-Elemente — Bild-Tabellen, Canvas-Tabellen und virtuelle JS-Tabellen werden nicht unterstützt
- Cross-Origin-Iframe-Tabellen können nicht zugegriffen werden (Browser-Sicherheitsbeschränkung)
- Komplex dynamisch verschlüsselte Tabellen werden möglicherweise nicht korrekt geparst

---

## Preise

| Plan | Preis | Details |
|------|-------|---------|
| 🆓 Kostenlos | $0 | Bis zu 5 Tabellen pro Seite |
| ⭐ Einzellizenz | $2.99/Monat oder $9.99 lebenslang | Unbegrenzte TableGrab-Exporte |
| 🏆 Komplettpaket | $4.99/Monat oder $29.99 lebenslang | Alle VKT-Erweiterungen Premium |

Siehe [VKT Preise](https://www.annmax1983.com/pricing.html) für Details.

## Datenschutz

- ✅ Es werden nie Tabellendaten oder Seiteninhalte hochgeladen — Parsing und CSV-Export passieren lokal
- ✅ Keine Analytik, kein Tracking
- ✅ Berechtigungen: `activeTab` + `scripting` + `downloads` + `storage`, plus Host-Zugriff auf den offiziellen Lizenzserver
- ✅ `storage` wird nur für Lizenzschlüssel und Einstellungen verwendet — keine Browserdaten
- 🔑 Premium-Lizenzaktivierung/-validierung verbindet sich nur mit dem offiziellen Lizenzserver (api.annmax1983.com) — es werden nie Tabellendaten übertragen

---

## Urheberrechtshinweis

Diese Erweiterung liest nur HTML-Tabellenstrukturen, die bereits auf Webseiten geladen sind, und konvertiert sie ins CSV-Format für den lokalen Download. Alle Tabellendaten und Webseiteninhalte unterliegen dem Urheberrecht der ursprünglichen Website. Nutzer dürfen exportierte Daten nicht für kommerzielle Vervielfältigung, unbefugte Weiterverbreitung oder andere urheberrechtsverletzende Handlungen verwenden. Alle rechtlichen Folgen aus missbräuchlicher Nutzung trägt allein der Nutzer.

---

## ❤️ Support

**[👉 Ko-fi — Kauf mir einen Kaffee](https://ko-fi.com/annmax?ref=tablegrab)**

---

> **Hinweis:** Dieses Repository dient ausschließlich der **Projektpräsentation**. Der vollständige Quellcode wird hier **nicht** veröffentlicht.
