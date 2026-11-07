# AURA

![Statut : archivé](https://img.shields.io/badge/statut-archiv%C3%A9-b3122b?style=flat-square&labelColor=0a0607)
![Version : aucune](https://img.shields.io/badge/version-aucune-ff4a3a?style=flat-square&labelColor=0a0607)

> [!CAUTION]
> **Projet archivé le 6 novembre 2026.** Développement arrêté définitivement : aucune nouvelle
> fonctionnalité, aucun correctif, aucune version publiée, aucun support. Le dépôt reste figé, en
> lecture seule, comme archive de ce qui a été écrit.
> **Avis complet : [ARCHIVED.md](ARCHIVED.md) — page d'archive : <https://louxos.github.io/AURA/>.**

> **Assistant IA personnel pour Windows**

AURA était pensé comme un centre de contrôle personnel sur Windows : la voix, l'IA, les services
Google et les outils système réunis dans une seule application privée, local-first.
**Il n'a jamais été publié** — ni version, ni installateur, ni binaire.

## 🗄️ Statut

| | |
| --- | --- |
| Archivé le | 6 novembre 2026 |
| Version publiée | Aucune |
| Développement | Arrêté définitivement |
| Dépôt | Figé, en lecture seule |

Ce dépôt ne contient pas de code exécutable : il ne garde que l'intention du produit, ce README,
l'[avis d'archivage](ARCHIVED.md) et la page d'archive publiée par GitHub Pages.
Aucun service n'est en ligne, aucun exécutable n'est distribué.

## 📄 Page d'archive

<https://louxos.github.io/AURA/>

| Fichier | Rôle |
| --- | --- |
| [`docs/index.html`](docs/index.html) | Page d'archive : état du projet, ce qu'AURA devait être, pourquoi l'arrêt, ce qui reste |
| [`docs/404.html`](docs/404.html) | Page introuvable, dans la même charte |
| [`docs/assets/site.css`](docs/assets/site.css) | Feuille de styles unique, aucune ressource distante |
| [`docs/assets/favicon.svg`](docs/assets/favicon.svg) | Marque AURA |

Publication : **Settings → Pages → Deploy from a branch**, branche `main`, dossier `/docs`.
Le dépôt doit être public pour que le site soit accessible.

## 🔐 Identifiants et secrets

Les clés d'API, jetons OAuth et identifiants de compte n'auraient jamais dû vivre dans Git : leur
place était dans un `.env` local.

Le cahier des charges qui décrivait AURA (`prompt`) contenait des **clés d'API en clair**. Il a été
**supprimé du dépôt à l'archivage**, et aucune clé n'est reproduite dans ce dépôt.

- Ces clés doivent être considérées comme **compromises** et révoquées chez le fournisseur : aucune
  réécriture d'historique ne les invalide.
- **L'historique a été réécrit le 6 novembre 2026** (`git filter-repo --invert-paths --path prompt`) :
  le fichier n'existe plus dans aucun commit. L'ancien historique `a6e6706…bb1870e` est remplacé par
  `b243e61…80588f9`.
- GitHub garde les objets devenus inaccessibles pendant un certain temps, et `main` pointe encore sur
  l'ancien commit : le dépôt ne doit pas être passé en public avant que `main` ne soit forcé sur
  l'historique nettoyé.
- Le [`.gitignore`](.gitignore) empêche désormais qu'un `.env` ou du matériel de clé revienne ici.

## ✨ Ce qui était prévu

Conservé comme historique — rien de tout cela n'a été publié.

* 🎙️ Interaction vocale
* 🧠 Conversations IA
* 📧 Intégration Gmail
* 📅 Intégration Google Agenda
* 💻 Contrôle du système Windows
* 📁 Gestion de fichiers locaux autorisés
* 🧠 Mémoire locale
* 🔔 Notifications Windows
* 🌐 Capacités Web
* 🔐 Authentification Google OAuth sécurisée
* ⚙️ Outils et commandes personnalisés

## 🏗️ Technique

* Python
* API Gemini / Groq / OpenRouter
* API Google
* Google OAuth 2.0
* SQLite
* API Windows
* Technologies vocales locales

## 🔒 Confidentialité

AURA était conçu pour un usage privé et personnel. Les identifiants, clés d'API et jetons
d'authentification devaient rester en local et ne jamais être versionnés.
