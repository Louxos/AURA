# AURA

> **Personal AI assistant for Windows — archived**

**Archived on 6 November 2026.** Development has stopped permanently: no new features, no fixes, no
releases, no support. This repository is left as it was, as an archive of what was specified.

📄 **Archive page: <https://louxos.github.io/AURA/>**

## 🗄️ Status

AURA was designed as a private, local-first AI assistant and control center for Windows: voice
interaction, AI conversations, Google services and Windows system tools in a single local
application. It was never released — not a single version, not an installer, no binaries.

What is left in this repository is the intent: this README and the static archive site in `docs/`.

## 🔐 Credentials and secrets

AURA was built around secrets that were never supposed to live in Git: API keys, OAuth tokens and
account identifiers all belonged in a local `.env` file.

The specification document that used to sit at the root of this repository (`prompt`) contained API
keys in plaintext. **It was deleted when the project was archived**, and no key is reproduced on the
archive page.

- Those keys must be treated as compromised and revoked at the provider.
- Deleting the file does not remove it from Git history (see commit `a6e6706`). If this repository is
  ever made public, the history has to be purged or rewritten first — a redacted version of the
  document is the only safe way to republish it.
- A `.gitignore` now keeps local `.env` files and key material out of the repository.

## ✨ What was planned

Kept as history — none of it was released.

* 🎙️ Voice interaction
* 🧠 AI-powered conversations
* 📧 Gmail integration
* 📅 Google Calendar integration
* 💻 Windows system control
* 📁 Local file management
* 🧠 Local memory
* 🔔 Windows notifications
* 🌐 Web capabilities
* 🔐 Secure Google OAuth authentication
* ⚙️ Custom tools and commands

## 🏗️ Technology

* Python
* Gemini API / Groq / OpenRouter
* Google APIs
* Google OAuth 2.0
* SQLite
* Windows APIs
* Local speech technologies

## 📄 Archive site

The GitHub Pages site lives in [`docs/`](docs/):

| File | Role |
| --- | --- |
| `docs/index.html` | Archive page: state, intent, why it stopped, what remains |
| `docs/404.html` | Not-found page |
| `docs/assets/site.css` | Single stylesheet, red charte, no external resource |
| `docs/assets/favicon.svg` | AURA mark |

Publish it with **Settings → Pages → Deploy from a branch**, branch `main`, folder `/docs`.
Note that this repository is private: a site published from a private repository is only reachable
with a plan that allows it, or by making the repository public.

## 🔒 Privacy

AURA was designed primarily for private, personal use. Sensitive credentials, API keys and
authentication tokens were meant to stay local and never be committed to the repository.
