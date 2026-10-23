# TableGrab

[English](../README.md) | [中文](README_zh.md) | [Español](README_es.md) | [Deutsch](README_de.md) | [日本語](README_ja.md) | Français

Une extension légère qui extrait les tableaux HTML natifs et les grilles de données ARIA/div de n'importe quelle page web, et les exporte en fichiers CSV ou Excel (XLSX) en un clic.

> Chromium · Manifest V3 · Permissions minimales · Confidentialité avant tout

---

## Pourquoi TableGrab ?

Vous avez déjà essayé de copier un tableau depuis un site gouvernemental ou une plateforme de données, pour obtenir une mise en forme brouillée ? TableGrab lit directement la structure du tableau et exporte des données CSV ou XLSX propres — pas d'erreur de copier-coller, pas de perte de format.

| Avantage | Détail |
|-----------|--------|
| 📊 **Détection automatique** | Scanne tous les tableaux natifs et grilles ARIA/div (role=grid/treegrid/table) de la page, affiche lignes × colonnes |
| 📗 **Export Excel** | Vraies cellules fusionnées, en-têtes stylés/figés, largeurs automatiques, une feuille par tableau |
| 🔗 **Cellules fusionnées** | Gère correctement rowspan/colspan, préserve la structure du tableau |
| 🧱 **Grilles div** | Lit les grilles MUI DataGrid / AG Grid et fusionne les colonnes figées dupliquées |
| 👁️ **Aperçu et colonnes** | Inspectez le tableau avant l'export et décochez les colonnes inutiles |
| 📋 **Copier en TSV / Markdown** | Collez directement dans Excel, Notion, GitHub ou une messagerie |
| 📦 **Export par lot** | Exportez un tableau unique, une sélection, ou tous les tableaux d'un coup |
| 🔤 **Pas de caractères corrompus** | L'encodage UTF-8 BOM corrige les problèmes de caractères chinois/CJK |
| ⚡ **Un clic** | Téléchargement instantané, aucun rafraîchissement de page nécessaire |
| 🔒 **Privé** | Permissions minimales, les données des tableaux ne sont jamais envoyées |

---

## Fonctionnalités

### 🆓 Gratuit

| Fonctionnalité | Description |
|---------|-------------|
| 📊 **Détection automatique des tableaux** | Trouve les tableaux natifs et grilles ARIA/div valides, filtre les tableaux cachés/de mise en page |
| 📗 **Export XLSX** | Classeur multi-feuilles, vraies cellules fusionnées, en-tête figé, largeurs automatiques |
| 🔗 **Support des cellules fusionnées** | Analyse rowspan/colspan, reconstruit la grille correctement |
| 🧱 **Grilles ARIA / div** | Lit les structures role=grid/treegrid/table (dont MUI et AG Grid) et fusionne les colonnes figées dupliquées |
| 👁️ **Aperçu avant export** | Aperçu défilant (jusqu'à 50 lignes) avec cases à cocher par colonne |
| ☑️ **Choix des colonnes** | Exportez uniquement les colonnes choisies ; la sélection est mémorisée par tableau |
| 📋 **Copier TSV / Markdown** | Un clic pour Excel, Notion, GitHub ou une messagerie, selon le réglage d'espaces |
| ✅ **Sélection multiple** | Cochez plusieurs tableaux, exportez la sélection ensemble |
| 📦 **Export par lot** | Exportez tous les tableaux de la page en un clic |
| 🔤 **UTF-8 BOM** | Correction d'encodage activée par défaut pour les caractères chinois/CJK |
| 🧹 **Nettoyage des espaces** | Supprime les sauts de ligne, espaces et fragments HTML superflus des cellules |
| 💡 **Surbrillance des tableaux** | Survolez la liste des tableaux pour mettre en surbrillance le tableau correspondant sur la page |
| 📁 **Nommage intelligent** | Génère automatiquement le nom de fichier : TitreDeLaPage_tables_horodatage.csv / .xlsx |
| 🔒 **5 tableaux/page max** | Le niveau gratuit exporte les 5 premiers tableaux détectés sur chaque page |

### ⭐ Premium (Licence)

| Fonctionnalité | Description |
|---------|-------------|
| 📦 **Exports illimités** | Pas de limite de 5 tableaux — exportez chaque tableau de n'importe quelle page |
| 🔄 **Toutes les fonctionnalités gratuites** | Tout ce qui précède, sans restriction |

---

## Aperçu

<p align="center">
  <img src="../icons/icon128.png" alt="Icône TableGrab" width="80">
</p>

---

## Navigateurs compatibles

| Navigateur | Statut |
|---------|--------|
| Google Chrome | ✅ Entièrement pris en charge |
| Microsoft Edge | ✅ Entièrement pris en charge |

---

## Installation

| Store | Lien |
|---|---|
| Chrome Web Store | [Installer dans Chrome](https://chromewebstore.google.com/detail/mekelpcokmdjgoiikpedhojmjappfeji) |
| Microsoft Edge Add-ons | [Installer dans Edge](https://microsoftedge.microsoft.com/addons/detail/lhoelnklgfdihllglpjkpbinfkejceah) |

> Installez uniquement depuis les boutiques officielles ci-dessus — évitez les sites de téléchargement tiers.

---

## Utilisation

1. Visitez une page contenant des tableaux ou des grilles de données ARIA/div
2. Cliquez sur l'icône **TableGrab**
3. Les tableaux sont détectés automatiquement et listés avec les infos lignes × colonnes
4. Survolez pour mettre en surbrillance, cochez pour sélectionner ; utilisez **Aperçu** pour choisir les colonnes
5. Cliquez sur **Tout exporter**, **Exporter la sélection** ou **Copier en TSV / Markdown**
6. Le fichier CSV ou XLSX se télécharge automatiquement

---

## Limitations connues

- Les grilles div sont prises en charge lorsqu'elles exposent des rôles ARIA (`grid`/`treegrid`/`table` avec rôles de ligne/cellule), comme MUI DataGrid et AG Grid. Les grilles rendues en Canvas ou sans structure accessible de lignes/cellules ne peuvent pas être lues
- Les tableaux paginés ou à défilement virtuel n'exportent que les lignes et colonnes présentes dans le DOM
- Les tableaux dans des iframes cross-origin ne sont pas accessibles (restriction de sécurité du navigateur)
- Les tableaux dynamiques complexes ou chiffrés peuvent ne pas être analysés correctement
- Les cellules de plus de 32 767 caractères sont tronquées pour respecter la limite d'Excel

---

## Tarifs

Le plan gratuit exporte jusqu'à 5 tableaux par page. Une licence outil individuel supprime cette limite d'export et la suite complète couvre les fonctions Premium de toutes les extensions VKT.

Voir les [tarifs VKT](https://www.annmax1983.com/pricing.html) pour les options de licence et les prix.

## Confidentialité

- ✅ Aucune donnée de tableau ni contenu de page n'est jamais envoyé — l'analyse et l'export CSV/XLSX se font en local
- ✅ Pas d'analytics, pas de suivi
- ✅ Permissions : `activeTab` + `scripting` + `downloads` + `storage`, plus l'accès au serveur de licences officiel
- ✅ `storage` est utilisé uniquement pour la clé de licence et les paramètres — aucune donnée de navigation
- 🔑 L'activation/validation de la licence Premium se connecte uniquement au serveur de licences officiel (api.annmax1983.com) — aucune donnée de tableau n'est transmise

---

## Avertissement relatif au droit d'auteur

Cette extension lit uniquement les structures de tableaux déjà chargées sur les pages web et les convertit au format CSV ou XLSX pour un téléchargement local. Tous les droits d'auteur des données de tableaux et du contenu des pages web appartiennent aux sites originaux. Les utilisateurs ne doivent pas utiliser les données exportées à des fins de reproduction commerciale, de redistribution non autorisée ou de toute autre activité portant atteinte au droit d'auteur. Toute responsabilité juridique découlant d'une utilisation inappropriée incombe exclusivement à l'utilisateur.

---

## ❤️ Soutenir

**[👉 Ko-fi — Offrez-moi un café](https://ko-fi.com/annmax?ref=tablegrab)**

---

> **Note :** Ce dépôt est destiné à la **présentation du projet uniquement**. Le code source complet ne sera **pas** publié ici.
