# Cartographie du dépôt — OptimasProtect_Blog

Dernière mise à jour : 2026-08-22 (premier run de l'agent).

## État constaté au premier run

Le dépôt `KhalidBougria/OptimasProtect_Blog` était **entièrement vide** à ce run (0 commit, 0 branche, `size: 0`). Aucun générateur de site, aucun thème, aucun contenu existant. Conformément au §7.1 point 5 du prompt de référence, j'établis donc moi-même les conventions ci-dessous ; le premier article devient la référence.

**Accès constaté :** authentifié en tant que `KhalidBougria` (propriétaire du compte), pas `obougria` comme prévu au prompt de référence — probablement parce que le connecteur GitHub MCP de cette session est configuré sur le compte propriétaire directement. Permissions confirmées : `push: true`, `admin: true`. L'écriture fonctionne. Voie technique utilisée : connecteur MCP GitHub local (`local_unpacked_qunfei-wu_github-mcp-server-js`), appels REST standard (`create_or_update_file`, etc.), pas d'appel direct à l'API GitHub hors MCP.

Branche par défaut du dépôt (`default_branch` renvoyé par l'API) : `main`. Elle n'existait pas avant le premier commit (`.seo/agent-prompt.md`) de ce run ; elle a été créée à cette occasion.

## Générateur de site

**Aucun générateur n'est présent dans le dépôt.** Aucun fichier de config (`astro.config.*`, `next.config.*`, `hugo.toml`, `config.yml`, `gatsby-config.*`, `package.json`) trouvé, pour cause de dépôt vide. Le dépôt sert pour l'instant uniquement de dépôt de contenu (Markdown) et de suivi (`.seo/`). Voir alerte haute dans le rapport du jour : sans générateur ni pipeline de build/déploiement, aucun des fichiers Markdown produits par cet agent ne peut devenir une page live tant qu'un humain n'a pas branché un générateur de site statique sur ce dépôt (ou pointé le générateur existant du site `optimasprotect.ma` vers ce dépôt, s'il existe ailleurs).

## Conventions établies par cet agent (à respecter ensuite à la lettre)

- **Dossier de contenu :** `content/blog/`
- **Nom de fichier :** `{slug}.md`, où `{slug}` est le slug court de l'article (identique au champ `slug` du frontmatter).
- **URL publique visée :** `https://optimasprotect.ma/blog/{slug}` (à confirmer/ajuster une fois qu'un générateur sera branché ; convention posée par défaut en cohérence avec le prompt de référence §3.2).
- **Liens internes :** relatifs, `/blog/{slug}`.

### Schéma de frontmatter YAML (référence)

```yaml
---
title: "Titre 50 à 60 caractères"
description: "Meta description 140 à 160 caractères"
slug: "slug-court"
tags: ["Tag 1", "Tag 2", "Tag 3"]
date: "2026-08-22"
author: "Team Optimas"
draft: true
focus_keyword: "mot-clé focus"
pillar: "1"
score: 18
---
```

Champs additionnels possibles selon besoin (`updated`, `canonical`). Jamais de champ image.

### Corps de l'article

Markdown standard (H1 unique en première ligne du corps sous forme `# Titre`, puis H2/H3). Pas de classes CSS spécifiques à respecter puisqu'aucun thème n'existe encore : dès qu'un thème sera branché, ce fichier `repo-map.md` devra être mis à jour avec les classes réelles (règle §7.1).

### JSON-LD

En l'absence de thème, le JSON-LD est inclus en fin de corps d'article dans un bloc ```` ```json-ld ```` (à adapter à la convention réelle du générateur une fois choisi). Types utilisés : `SoftwareApplication` + `Offer` pour les articles pilier 1 avec prix, `Article` avec `author.@type: Organization`, `FAQPage` pour le bloc FAQ.

## Hubs (à constituer au fil des publications)

- Hub pilier 1 (traçabilité / contrôle de ronde) : premier article candidat `controle-de-ronde-nfc-gardiennage-maroc`.
- Hub prix (« prix logiciel de gardiennage / sécurité privée ») : premier article candidat `prix-logiciel-gardiennage-maroc`.
- Hub conformité (Loi n°35-09 / cahiers des charges) : **en attente**, voir alerte réglementaire ci-dessous.

## Veille concurrentielle — URLs identifiées ce run

- **Cercle 1 (Maroc) :** SEKUR Africa — `https://sekur-africa.com/logiciel/logiciel-securite-privee-gardiennage-maroc/`, `https://sekur-africa.com/logiciel/` (page produit générique), `https://sekur-africa.com/meilleurs-logiciels-securite-privee-2025/` (comparatif publié par le concurrent lui-même). Pas de prix affiché publiquement constaté sur ces pages — point d'opacité exploitable pour Optimas Protect (prix affichés).
- **Cercle 2 (international) :** Trackforce Valiant — `https://www.trackforce.com/fr/solutions/gestion-des-gardiens-de-securite/`. Pricing non public (sur devis), confirmé par plusieurs comparateurs tiers (Capterra, GetApp).
- Pas de nouvel acteur marocain non identifié détecté ce run.

## Alerte haute n°1 — site optimasprotect.ma non indexé / non accessible en fetch

`https://optimasprotect.ma/` a été interrogé deux fois via web fetch : réponse vide (aucun contenu HTML/texte récupérable), ni en page d'accueil ni via une recherche `site:optimasprotect.ma` (zéro résultat indexé sur Google). Impossible de vérifier `robots.txt`, le rendu statique vs SPA, ou l'existence effective d'un `/blog/` public. Combiné à l'absence totale de générateur dans le dépôt (voir plus haut), ceci suggère que le site public n'est pas encore construit à partir de ce dépôt, ou n'est pas encore en ligne, ou est bloqué aux robots/fetchers. **À vérifier par un humain avant toute attente de résultat SEO.** Voir rapport du jour.

## Alerte haute n°2 — écart factuel sur la loi citée dans le prompt de référence — RÉSOLUE le 2026-08-22

Le prompt de référence (et donc les gabarits d'articles réglementaires) citait systématiquement la « Loi n°35-09 » comme texte régissant les activités privées de sécurité au Maroc. La recherche web de ce run (sources : Bulletin Officiel, SGG, plusieurs cabinets et blogs juridiques marocains) indiquait de façon convergente que la loi réellement en vigueur sur le gardiennage et le transport de fonds au Maroc est la **loi n° 27-06** (promulguée par le dahir n° 1-07-155, 2007).

**L'utilisateur a confirmé le 2026-08-22 que la loi n° 27-06 est bien celle en vigueur.** Le prompt de référence (`.seo/agent-prompt.md`) a été corrigé en conséquence (PR #3, mergée) : toutes les occurrences de « Loi n°35-09 » remplacées par « Loi n°27-06 », y compris le tag `Conformité 27-06`, le cluster 8, la tête de requête Â§4.3.6, les garde-fous §8.1 et la source primaire §8.3.

**Le hub conformité et le cluster 8 (Loi n°27-06 et cahiers des charges) sont désormais débloqués** et peuvent être produits aux prochains runs, dans le respect du régime renforcé §3.3 (article réglementaire toujours en PR, jamais en publication automatique, chaque affirmation datée et sourcée par lien primaire officiel).

## Mise à jour 2026-08-25 — Alerte haute n°1 partiellement résolue + nouvelle alerte marque

**Le site `https://optimasprotect.ma/` est maintenant accessible en fetch** (il ne l'était pas aux runs précédents). Contenu HTML complet récupéré : page d'accueil marketing avec 6 modules (Planning & Pointage, Rondes & Sécurité, RH & Administration, Incidents & Rapports, Portail Client, Équipements & Sites), tarifs conformes au prompt (99 MAD/smartphone/mois Opérations, 179 MAD/smartphone/mois Business, Enterprise sur devis), CTA WhatsApp vers +212 7 24 80 13 72.

**Cependant :**
- **Aucun lien ni section `/blog/` visible dans la navigation ou le footer du site live.** Les assets (images, meta og:image) pointent vers `storage.googleapis.com/gpt-engineer-file-uploads/...`, ce qui suggère un site généré par un outil tiers (type GPT Engineer / Lovable) et non par un générateur de site statique consommant ce dépôt Git. **Ceci confirme l'hypothèse de l'alerte haute n°1 initiale : le dépôt `OptimasProtect_Blog` n'est very probablement pas connecté au site live.** Aucun des articles produits par cet agent (7 PR au 2026-08-25) ne peut donc devenir une page consultable sans intervention humaine pour brancher un générateur ou intégrer une section blog au site existant.
- `robots.txt` n'a pas pu être vérifié ce run : l'outil de fetch de cette session a bloqué l'URL `https://optimasprotect.ma/robots.txt` (restriction technique de provenance, pas un problème du site). À revérifier au prochain run si l'outil le permet.
- Recherche `site:optimasprotect.ma` toujours à 0 résultat indexé sur Google au 2026-08-25 (cohérent avec un site sans blog et/ou récemment mis en ligne).

**Nouvelle alerte haute — écart d'orthographe de marque sur le site live lui-même :** le site utilise systématiquement **« OptImasProtect »** (un seul mot, I majuscule médian) dans le `<title>`, les meta OG/Twitter, le footer et l'alt du logo — alors que le prompt de référence (§1) impose **« Optimas Protect » en deux mots** comme orthographe non négociable, avec l'exemple explicite Â« jamais OptImasProtect Â». Il y a donc une contradiction directe entre la charte éditoriale de cet agent et le nom réel affiché sur le site en production. Je continue d'appliquer la règle du prompt (« Optimas Protect », deux mots) dans les articles produits, en attendant un arbitrage humain : soit le prompt est corrigé pour refléter le nom réel du produit (« OptImasProtect »), soit le site doit être corrigé pour se conformer à la charte. Voir rapport du 2026-08-25 pour le signalement complet.

**Confirmation positive :** le format de frontmatter et le dossier `content/blog/{slug}.md` établis au premier run fonctionnent sans ajustement — le commit de l'article `cahier-des-charges-gardiennage-maroc.md` (PR #8) a été réalisé sans erreur avec ces conventions.

## Mise à jour 2026-08-26 — Alerte haute critique : un workflow GitHub Actions contourne la Phase 1

Découverte ce run en investiguant pourquoi `content/blog/*.md` apparaissait déjà sur `main` alors que les PR #1, #2, #4, #5, #6, #7, #8 restent toutes affichées comme **non mergées** côté GitHub (`state: open`, `merged_at: null`).

**Cause identifiée :** le dépôt contient `.github/workflows/main.yml` (job `copie-repo`), déclenché **chaque jour à 10:00 UTC** (et manuellement via `workflow_dispatch`). Ce workflow fait un `git fetch --all`, puis pour **chaque branche `article/*`**, la rebase sur `main` et la **force-pousse directement sur `main`** (`git push origin HEAD:main --force`), indépendamment de l'état de review ou de `draft` de la pull request associée. C'est ce qui explique que les 7 articles produits entre le 2026-08-22 et le 2026-08-25 sont déjà lisibles sur `main` (confirmé par `list_commits` : auteur `KhalidBougria` à la date de rédaction, committer `GitHub Actions` daté du 2026-08-25T11:41 UTC, tous en une seule rafale de commits séquentiels), alors que leurs PR n'ont jamais été mergées via l'interface GitHub.

**Pourquoi c'est une alerte haute :**
- Ce workflow contredit directement la consigne explicite de la tâche planifiée : *« reste en Phase 1 (relecture par PR) jusqu'à nouvel ordre explicite de l'utilisateur… n'active jamais la Phase 2 (commit direct) de ta propre initiative »*. L'agent respecte cette consigne à la lettre (branche + PR, jamais de push direct), mais une automatisation tierce republie tout de même chaque article sur `main` sans relecture humaine.
- Cela touche même l'article réglementaire `cahier-des-charges-gardiennage-maroc.md` (PR #8), pour lequel le §3.3 du prompt de référence impose une **exception permanente** : *« reste en PR même en phase 2, ne sera jamais mergé automatiquement »*. Ce garde-fou est aujourd'hui contourné dans les faits par le workflow, malgré `draft: true` dans le frontmatter (le workflow ne lit pas ce champ, il copie le contenu Git brut).
- Le champ `draft: true` du frontmatter n'a par ailleurs aucun effet de blocage connu côté génération de site tant qu'aucun générateur n'est branché (voir alerte n°1 plus haut) — donc même si un site venait à être connecté à ce dépôt sans traiter `draft`, tout partirait en ligne sans filtre.

**Action humaine requise :** décider si ce workflow doit être désactivé, modifié pour respecter l'état des PR (ne copier que les branches dont la PR est mergée et non-brouillon), ou si la Phase 1 doit être abandonnée au profit d'un ordre explicite de passage en Phase 2. Tant qu'aucune décision n'est prise, cette note documente que **le contenu produit par cet agent est en pratique déjà répliqué sur `main` en quelques heures**, même si le processus déclaré (branche + PR) reste respecté à la lettre par l'agent lui-même.

Ce workflow ne modifie en rien la question ouverte de la connexion entre ce dépôt et le site live `optimasprotect.ma` (toujours pas de section `/blog/` visible ni de générateur de site dans ce dépôt) : il republie uniquement sur la branche `main` de ce même dépôt, sans build ni déploiement associé constaté.
