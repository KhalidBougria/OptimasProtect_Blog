# Cartographie du dépôt — OptimasProtect_Blog

Dernière mise à jour : 2026-08-29. Ce fichier est un document de travail vivant ; pour l'historique détaillé jour par jour, voir `.seo/rapports/`.

## Accès au dépôt

Authentifié en tant que `KhalidBougria` (propriétaire du compte), pas `obougria` comme prévu au prompt de référence — le connecteur GitHub MCP de cette session est configuré sur le compte propriétaire directement. Permissions confirmées : `push: true`, `admin: true`. Voie technique : connecteur MCP GitHub local (`local_unpacked_qunfei-wu_github-mcp-server-js`). Visibilité du dépôt : `public` côté API (reconfirmé le 2026-08-29 ; le prompt de référence le décrit comme privé ; à noter, pas bloquant pour l'écriture). Branche par défaut : `main`.

## Générateur de site

Aucun générateur n'est présent dans le dépôt (aucun `astro.config.*`, `next.config.*`, `hugo.toml`, `package.json`, etc.). Le dépôt sert uniquement de dépôt de contenu (Markdown) et de suivi (`.seo/`). **Alerte haute permanente :** sans générateur ni pipeline de build/déploiement connu sur ce dépôt, aucun article produit par cet agent ne peut devenir une page live tant qu'un humain n'a pas branché un générateur de site statique sur ce dépôt (ou relié le générateur existant du site `optimasprotect.ma` à ce dépôt).

## Conventions établies par cet agent (à respecter à la lettre, sous réserve de la nouvelle alerte ci-dessous)

- **Dossier de contenu :** `content/blog/` (dans les branches `article/*` uniquement à ce jour ; absent de `main`).
- **Nom de fichier :** `{slug}.md`, où `{slug}` est le slug court (identique au champ `slug` du frontmatter).
- **URL publique visée :** `https://optimasprotect.ma/blog/{slug}` (hypothèse du prompt de référence — **remise en question le 2026-08-29, voir alerte critique ci-dessous**).
- **Liens internes :** relatifs, `/blog/{slug}`.

### Schéma de frontmatter YAML (référence)

```yaml
---
title: "Titre 50 à 60 caractères"
description: "Meta description 140 à 160 caractères"
slug: "slug-court"
tags: ["Tag 1", "Tag 2", "Tag 3"]
date: "2026-08-28"
author: "Team Optimas"
draft: true
focus_keyword: "mot-clé focus"
pillar: "1"
score: 18
---
```

Aucun champ image. Champs additionnels possibles : `updated`, `canonical`.

### Corps de l'article

Markdown standard (H1 unique en première ligne du corps sous forme `# Titre`, puis H2/H3). Pas de classes CSS spécifiques tant qu'aucun thème n'est branché.

### JSON-LD

En fin de corps d'article dans un bloc ```json-ld```. Types : `SoftwareApplication` + `Offer` pour les articles pilier 1 avec prix, `Article` avec `author.@type: Organization`, `FAQPage` pour le bloc FAQ.

## Hubs en constitution

- Hub pilier 1 (traçabilité / contrôle de ronde) : `controle-de-ronde-nfc-gardiennage-maroc`.
- Hub prix : `prix-logiciel-gardiennage-maroc`.
- Hub conformité (Loi n°27-06 / cahiers des charges) : un seul article à ce jour (`cahier-des-charges-gardiennage-maroc`) ; deuxième article planifié (obligations Loi n°27-06 employeur, voir backlog).

## Veille concurrentielle — URLs de référence

- **Cercle 1 (Maroc) :** SEKUR Africa — `sekur-africa.com/logiciel/logiciel-securite-privee-gardiennage-maroc/` (page produit Maroc, aucun prix inline), `sekur-africa.com/tarifs/` (page tarifs globale non localisée, prix en EUR uniquement, dégressifs selon engagement). La page d'accueil `sekur-africa.com/` annonce par ailleurs un prix d'appel « à partir de 99,99 € / mois pour 6 utilisateurs » (chiffre distinct de la page `/tarifs/`, à recouper). SEKUR Africa a publié un article comparatif « Les 5 meilleurs logiciels de planning pour agences de sécurité privée & de gardiennage » (`sekur-africa.com/meilleurs-logiciels-securite-privee-2025/`) — un format de contenu (comparatif sectoriel) qu'Optimas Protect n'a pas encore produit, à garder en tête comme idée de contenu future (avec prudence sur le garde-fou §8.2, pas de dénigrement nominal). Opacité tarifaire MAD reconfirmée le 2026-08-29 : toujours aucun prix en dirhams publié pour le marché marocain.
- **Cercle 2 (international) :** Trackforce Valiant — `trackforce.com/fr/solutions/gestion-des-gardiens-de-securite/`. Pricing toujours non public (sur devis), reconfirmé le 2026-08-29.
- Ne pas confondre SEKUR Africa avec SEKUR France (`sekur.fr` / `logiciel.sekur.fr`), hors périmètre Maroc.

## ✅ Alerte critique du 2026-08-26 (workflow `copie-repo`) — RÉSOLUE, close depuis le 2026-08-28

Un workflow GitHub Actions `.github/workflows/main.yml` (job `copie-repo`, cron quotidien 10:00 UTC) force-poussait chaque branche `article/*` directement sur `main`, contournant la Phase 1 (relecture par PR). Découvert le 2026-08-26, supprimé le jour même. Les 7 fichiers d'articles concernés ont été retirés de `main` le 2026-08-27. `list_workflows` renvoie `total_count: 0` (reconfirmé le 2026-08-28). Non revérifié spécifiquement ce run (2026-08-29) car considéré clos ; à ressurveiller uniquement en cas de réapparition d'un workflow.

## 🔴 NOUVELLE ALERTE CRITIQUE DU 2026-08-29 : le site live expose désormais une page `/articles`, incompatible avec l'hypothèse `/blog/`

En vérifiant le site live `https://optimasprotect.ma/` ce run, le footer affiche désormais un lien « Ressources → Articles » pointant vers **`https://optimasprotect.ma/articles`** (et non `/blog/`). C'est un changement par rapport au dernier contrôle disponible (2026-08-25), où aucune section blog n'était visible du tout.

Faits constatés :
- La page `/articles` existe, avec son propre titre (« Articles | OptImasProtect ») et sa propre meta description (« Découvrez nos articles sur le gardiennage, la sécurité et la gestion des agents au Maroc. »).
- Son contenu affiche uniquement le texte « Chargement des articles... » (loading state), ce qui indique un rendu **côté client** (JavaScript), chargeant probablement une liste d'articles depuis une source externe (CMS headless, API, ou autre) — pas un rendu statique pré-généré comme le prompt de référence le présuppose (§7, « un générateur de site statique reconstruit et déploie les pages en HTML pré-rendu »).
- Aucun lien vers `/blog/` n'apparaît nulle part sur le site (page d'accueil ni page `/articles`). Le chemin `/blog/{slug}` utilisé comme URL canonique dans les 9 articles déjà produits (frontmatter, JSON-LD) et dans les conventions de ce fichier n'a donc aucune preuve d'existence sur le site live à ce jour.
- Tentative de navigation via le navigateur intégré pour inspecter la requête réseau derrière « Chargement des articles... » : bloquée (accès au site non autorisé dans ce contexte non supervisé). Impossible de confirmer si cette page est destinée à être connectée un jour à ce dépôt Git, ou si elle provient d'un système de contenu totalement distinct (cohérent avec l'hypothèse déjà documentée d'un site généré par un outil tiers type GPT Engineer / Lovable, assets hébergés sur `storage.googleapis.com/gpt-engineer-file-uploads/...`).

**Conséquence pratique :** il existe désormais un doute réel sur la structure d'URL cible. Deux hypothèses non tranchées :
1. `/articles` est le futur point d'entrée du blog et remplacera `/blog/` — auquel cas les 9 articles déjà produits en PR (canonical `https://optimasprotect.ma/blog/{slug}`) devront être corrigés avant toute mise en ligne.
2. `/articles` est une fonctionnalité indépendante (gérée par un CMS tiers, sans lien avec ce dépôt Git) et `/blog/` reste la cible correcte une fois ce dépôt effectivement branché à un générateur de site.

**Décision de cet agent :** ne pas modifier unilatéralement la convention d'URL (`/blog/{slug}`) tant qu'un humain n'a pas tranché laquelle des deux hypothèses est correcte — un changement non arbitré risquerait de corriger dans le mauvais sens. Les conventions existantes restent donc appliquées à l'identique pour l'instant, mais **aucun nouvel article n'a été produit ce run** en partie à cause de cette incertitude (voir rapport du jour pour la décision complète). Recommandation forte : qu'un humain inspecte le code source ou les requêtes réseau de `https://optimasprotect.ma/articles` pour identifier sa source de données avant la prochaine journée de production.

## Alertes non résolues (arbitrage humain attendu)

1. **Connexion du dépôt Git au site live** : toujours pas de preuve que ce dépôt alimente `optimasprotect.ma`. Voir la nouvelle alerte `/articles` ci-dessus, qui complexifie plutôt qu'elle ne résout ce point.
2. **Écart de marque :** le site live affiche systématiquement « OptImasProtect » (un mot, I majuscule médian) dans le `<title>`, les meta OG/Twitter, le footer et l'alt du logo — reconfirmé le 2026-08-29 — alors que le prompt de référence impose « Optimas Protect » en deux mots. L'agent continue d'appliquer la règle du prompt (deux mots) dans les articles, en attendant arbitrage.
3. `robots.txt` : tentative de vérification ce run bloquée par une restriction technique de l'outil de fetch (URL hors du périmètre autorisé). Non prioritaire tant que le point 1 n'est pas résolu.
4. `site:optimasprotect.ma` : toujours 0 résultat indexé sur Google (reconfirmé le 2026-08-29 via recherche web).

## Confirmation positive

Le format de frontmatter et le dossier `content/blog/{slug}.md` établis au premier run fonctionnent sans ajustement : 9 articles produits à ce jour, tous conformes. Aucun 10ᵉ article ce run (voir rapport du jour).
