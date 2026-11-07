# AURA

![Statut : archivé](https://img.shields.io/badge/statut-archiv%C3%A9-b3122b?style=flat-square&labelColor=0a0607)
![Version : aucune](https://img.shields.io/badge/version-aucune-ff4a3a?style=flat-square&labelColor=0a0607)

> [!CAUTION]
> **Projet archivé le 6 novembre 2026.** Développement arrêté définitivement : aucune nouvelle
> fonctionnalité, aucun correctif, aucune version publiée, aucun support. Le dépôt reste figé, en
> lecture seule, comme archive de ce qui a été écrit.
> **Avis complet : [ARCHIVED.md](ARCHIVED.md).**

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

Ce dépôt ne contient pas de code exécutable : il ne garde que l'intention du produit, ce README et
l'[avis d'archivage](ARCHIVED.md). Aucun site n'est publié et aucun service n'est en ligne.

## 🔐 Identifiants et secrets

Les clés d'API, jetons OAuth et identifiants de compte n'auraient jamais dû vivre dans Git : leur
place était dans un `.env` local.

Le cahier des charges qui décrivait AURA (`prompt`) contenait des **clés d'API en clair**. Il a été
**supprimé du dépôt à l'archivage**, et aucune clé n'est reproduite dans ce dépôt.

- Ces clés doivent être considérées comme **compromises** et révoquées chez le fournisseur.
- Les supprimer du fichier ne les retire pas de l'historique Git (commit `a6e6706`) : si ce dépôt
  devient public, l'historique doit être purgé ou réécrit avant, et le document republié uniquement
  sous une forme expurgée.
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
