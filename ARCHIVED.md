# 🗄️ AURA est archivé

![Statut : archivé](https://img.shields.io/badge/statut-archiv%C3%A9-b3122b?style=flat-square&labelColor=0a0607)
![Développement : arrêté](https://img.shields.io/badge/d%C3%A9veloppement-arr%C3%AAt%C3%A9-ff4a3a?style=flat-square&labelColor=0a0607)

> [!CAUTION]
> **Ce projet est désormais archivé.** Développement arrêté définitivement le 6 novembre 2026.
> Aucune nouvelle fonctionnalité, aucun correctif, aucune version publiée, aucun support.
> Rien n'a été supprimé pour autant : ce dépôt reste figé, en lecture seule, comme archive.
> **Page d'archive : <https://louxos.github.io/AURA/>**

## État du projet

| | |
| --- | --- |
| **Archivé le** | 6 novembre 2026 |
| **Version publiée** | Aucune — AURA n'a jamais été distribuée |
| **Développement** | Arrêté définitivement |
| **Dépôt** | Figé, en lecture seule |

L'archivage est une décision, pas un incident. **Aucune application n'existe ici** : ce dépôt ne
contient pas de code exécutable, seulement l'intention du produit, écrite avant d'être construite.
Ni installateur, ni binaire, ni service en ligne ne sont proposés.

## Ce qu'AURA devait être

Un assistant qui vit sur la machine, pas dans un onglet : la voix d'abord, les données locales par
défaut, et des outils qui n'agissent qu'une fois autorisés.

> Un centre de contrôle personnel intelligent : on parle, AURA comprend, choisit l'outil juste,
> montre ce qu'elle fait — et ne prétend jamais avoir fait ce qu'elle n'a pas fait.

- **La voix, pas un champ de texte** — réveil par « Salut AURA », conversation continue, écoute et
  réponse en français, moteurs vocaux privilégiés en local, sphère centrale servant d'état et de
  bouton d'arrêt.
- **Local d'abord, et vérifiable** — clés et jetons dans un fichier local, jamais dans le code ;
  permissions accordées par l'utilisateur et non modifiables par l'assistant ; suppressions toujours
  confirmées ; une consigne trouvée dans un e-mail ou une page web traitée comme une donnée, jamais
  comme un ordre.
- **De vrais outils** — Gmail, Google Agenda, Drive, fichiers autorisés, mémoire, emploi du temps,
  tâches et rappels, notifications Windows, chacune laissant une trace dans un historique.

## Pourquoi le développement s'arrête

1. **Un cahier des charges plus grand qu'un projet.** Voix, réveil, OAuth Google, mémoire,
   permissions, confirmations, packaging Windows : un produit complet, pas un prototype — et la
   règle tenue était de ne jamais annoncer comme fonctionnel ce qui n'avait pas été testé.
2. **La sécurité ne supportait pas l'approximation.** Un assistant qui lit une boîte Gmail, ouvre des
   fichiers et agit sur Windows détient beaucoup : une erreur de jeton, de confirmation ou
   d'injection de consigne ne se rattrape pas.
3. **Rien n'était prêt à être distribué.** Ni installateur, ni essais sur un parc réel, ni moyen de
   tenir les quotas des modèles et le suivi. Plutôt que de promettre, le projet s'arrête.

## Identifiants et secrets

Le cahier des charges qui décrivait AURA (`prompt`) contenait des **clés d'API en clair**. Il a été
**supprimé du dépôt à l'archivage**.

- Ces clés doivent être considérées comme **compromises** et révoquées chez le fournisseur.
- Les supprimer du fichier ne les retire pas de l'historique Git (commit `a6e6706`) : si ce dépôt
  devient public, l'historique doit être purgé ou réécrit avant, et le document republié uniquement
  sous une forme expurgée.
- Un [`.gitignore`](.gitignore) empêche désormais qu'un `.env` ou du matériel de clé revienne dans le
  dépôt.

## Ce qui reste

- La [page d'archive](https://louxos.github.io/AURA/) : l'état du projet, en une page.
- Le [README](README.md) : l'intention, la pile technique, les limites annoncées.
- L'historique des commits, conservé tel quel.

## Et maintenant ?

Rien. Aucune correction, aucune réponse de support, aucune reprise prévue. Les issues et les pull
requests sont figées par l'archivage. AURA n'a jamais été publiée et ne le sera pas.

---

*AURA · 2026 — du premier cahier des charges à l'archive, sans rien effacer.*
