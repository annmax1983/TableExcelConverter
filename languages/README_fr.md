# TableGrab

[English](../README.md) | [中文](README_zh.md) | [Español](README_es.md) | [Deutsch](README_de.md) | [日本語](README_ja.md) | Français

Une extension légère qui extrait les tableaux HTML de n'importe quelle page web et les exporte en fichiers CSV en un clic.

> Chromium · Manifest V3 · Permissions minimales · Confidentialité avant tout

---

## Pourquoi TableGrab ?

Vous avez déjà essayé de copier un tableau depuis un site gouvernemental ou une plateforme de données, pour obtenir une mise en forme brouillée ? TableGrab lit directement la structure HTML du tableau et exporte des données CSV propres — pas d'erreur de copier-coller, pas de perte de format.

| Avantage | Détail |
|-----------|--------|
| 📊 **Détection automatique** | Scanne tous les tableaux HTML de la page, affiche le nombre de lignes × colonnes |
| 🔗 **Cellules fusionnées** | Gère correctement rowspan/colspan, préserve la structure du tableau |
| 📦 **Export par lot** | Exportez un tableau unique, une sélection, ou tous les tableaux d'un coup |
| 🔤 **Pas de caractères corrompus** | L'encodage UTF-8 BOM corrige les problèmes de caractères chinois/CJK |
| ⚡ **Un clic** | Téléchargement instantané, aucun rafraîchissement de page nécessaire |
| 🔒 **Privé** | Permissions minimales, les données des tableaux ne sont jamais envoyées |

---

## Fonctionnalités

### 🆓 Gratuit

| Fonctionnalité | Description |
|---------|-------------|
| 📊 **Détection automatique des tableaux** | Trouve tous les tableaux HTML valides, filtre les tableaux cachés/de mise en page |
| 🔗 **Support des cellules fusionnées** | Analyse rowspan/colspan, reconstruit la grille correctement |
| 📋 **Export unique** | Exportez un tableau au format CSV |
| ✅ **Sélection multiple** | Cochez plusieurs tableaux, exportez la sélection ensemble |
| 📦 **Export par lot** | Exportez tous les tableaux de la page en un clic |
| 🔤 **UTF-8 BOM** | Correction d'encodage activée par défaut pour les caractères chinois/CJK |
| 🧹 **Nettoyage des espaces** | Supprime les sauts de ligne, espaces et fragments HTML superflus des cellules |
| 💡 **Surbrillance des tableaux** | Survolez la liste des tableaux pour mettre en surbrillance le tableau correspondant sur la page |
| 📁 **Nommage intelligent** | Génère automatiquement le nom de fichier : TitreDeLaPage_tables_horodatage.csv |
| 🔒 **5 tableaux/page max** | Le niveau gratuit exporte les 5 premiers tableaux détectés sur chaque page |

### ⭐ Premium (Licence)

| Fonctionnalité | Description |
|---------|-------------|
| 📦 **Exports illimités** | Pas de limite de 5 tableaux — exportez chaque tableau de n'importe quelle page |
| 🔄 **Toutes les fonctionnalités gratuites** | Tout ce qui précède, sans restriction |

---

## Aperçu

<p align="center">
  <img src="icons/icon128.png" alt="Icône TableGrab" width="80">
</p>

---

## Navigateurs compatibles

| Navigateur | Statut |
|---------|--------|
| Google Chrome | ✅ Entièrement pris en charge |
| Microsoft Edge | ✅ Entièrement pris en charge |

---

## Installation

1. Ouvrez `chrome://extensions/` ou `edge://extensions/`
2. Activez le **mode Développeur**
3. Cliquez sur **Charger le package décompressé** et sélectionnez le dossier du projet

---

## Utilisation

1. Visitez une page contenant des tableaux HTML
2. Cliquez sur l'icône **TableGrab**
3. Les tableaux sont détectés automatiquement et listés avec les infos lignes × colonnes
4. Survolez pour mettre en surbrillance, cochez pour sélectionner
5. Cliquez sur **Tout exporter** ou **Exporter la sélection**
6. Le fichier CSV se télécharge automatiquement

---

## Limitations connues

- Seuls les éléments HTML `<table>` sont supportés — tableaux image, tableaux Canvas, tableaux JS virtuels non supportés
- Les tableaux dans des iframes cross-origin ne sont pas accessibles (restriction de sécurité du navigateur)
- Les tableaux dynamiques complexes ou chiffrés peuvent ne pas être analysés correctement

---

## Tarifs

| Plan | Prix | Détails |
|------|-------|--------|
| 🆓 Gratuit | 0 $ | Jusqu'à 5 tableaux par page |
| ⭐ Outil individuel | 2,99 $/mois ou 9,99 $ à vie | Exports TableGrab illimités |
| 🏆 Suite complète | 4,99 $/mois ou 29,99 $ à vie | Toutes les extensions VKT en Premium |

Voir les [tarifs VKT](https://www.annmax1983.com/pricing.html) pour plus de détails.

## Confidentialité

- ✅ Aucune donnée de tableau ni contenu de page n'est jamais envoyé — l'analyse et l'export CSV se font en local
- ✅ Pas d'analytics, pas de suivi
- ✅ Permissions : `activeTab` + `scripting` + `downloads` + `storage`, plus l'accès au serveur de licences officiel
- ✅ `storage` est utilisé uniquement pour la clé de licence et les paramètres — aucune donnée de navigation
- 🔑 L'activation/validation de la licence Premium se connecte uniquement au serveur de licences officiel (api.annmax1983.com) — aucune donnée de tableau n'est transmise

---

## Avertissement relatif au droit d'auteur

Cette extension lit uniquement les structures de tableaux HTML déjà chargées sur les pages web et les convertit au format CSV pour un téléchargement local. Tous les droits d'auteur des données de tableaux et du contenu des pages web appartiennent aux sites originaux. Les utilisateurs ne doivent pas utiliser les données exportées à des fins de reproduction commerciale, de redistribution non autorisée ou de toute autre activité portant atteinte au droit d'auteur. Toute responsabilité juridique découlant d'une utilisation inappropriée incombe exclusivement à l'utilisateur.

---

## ❤️ Soutenir

**[👉 Ko-fi — Offrez-moi un café](https://ko-fi.com/annmax?ref=tablegrab)**

---

> **Note :** Ce dépôt est destiné à la **présentation du projet uniquement**. Le code source complet ne sera **pas** publié ici.
