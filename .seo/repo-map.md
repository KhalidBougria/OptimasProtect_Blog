# Cartographie du dépôt — OptimasProtect_Blog

Dernière mise à jour : 2026-09-01 (semaine S36). Ce fichier est un document de travail vivant ; pour l'historique détaillé jour par jour, voir `.seo/rapports/`.

## Point du 2026-09-01 : 12 PR ouvertes, toujours aucune fusion

PR #14 (`faux-pointage-ads-detecter-maroc`, pilier 1, cluster 9, score 16/25) ajoutée ce run. Le dépôt compte désormais **12 pull requests ouvertes depuis le 2026-08-22, aucune fusionnée** — plus d'une semaine et demie sans relecture humaine. Ce point était déjà signalé le 2026-08-31 ; il continue de croître d'une session à l'autre. Non bloquant pour la veille et la production, mais à réévaluer par l'utilisateur si le volume continue de croître sans aucune relecture.

`site:optimasprotect.ma` reconfirmé à 0 résultat indexé ce run (recherche web). L'alerte haute « aucun générateur de site connecté à ce dépôt » (voir section dédiée plus bas) reste active et non résolue.

## Point du 2026-08-31 : 11 PR ouvertes, toujours aucune fusion

PR #13 (`obligations-loi-27-06-employeur-maroc`, hub conformité, score 18/25) ajoutée ce run. Le dépôt compte désormais **11 pull requests ouvertes depuis le 2026-08-22, aucune fusionnée** — plus d'une semaine sans relecture humaine. Ce n'est pas en soi une alerte nouvelle (la Phase 1 fonctionne comme prévu), mais le volume croissant de PR en attente devient un point à signaler explicitement dans chaque rapport : au-delà d'un certain nombre, l'utilité de continuer à produire sans qu'aucune relecture n'ait lieu mérite d'être réévaluée par l'utilisateur.

`site:optimasprotect.ma` reconfirmé à 0 résultat indexé ce run (recherche web). L'alerte haute « aucun générateur de site connecté à ce dépôt » (voir section dédiée plus bas) reste active et non résolue.

## ✅ Arbitrage humain du 2026-08-29 (PR #11, mergée) — alertes `/articles` et « écart de marque » RÉSOLUES

Le prompt de référence `.seo/agent-prompt.md` (version 3.2, PR #11 mergée le 2026-08-29 à 08:25:27Z) tranche les deux points laissés en suspens le 2026-08-29 :

1. **Structure d'URL :** `/articles/{slug}` est confirmée comme cible correcte (et non `/blog/{slug}`), conformément au lien footer observé sur le site live. Confirmé par l'utilisateur.
2. **Orthographe de la marque :** `OptimasProtect` en un seul mot remplace `« Optimas Protect » à partir de maintenant (production future uniquement), conformément à l'orthographe du site live.

**Vérification spot-check ce run :** l'article `controle-de-ronde-nfc-gardiennage-maroc` (branche `article/*`, PR #1) utilise déjà des liens internes en `/articles/{slug}` et la forme « OptimasProtect » (un mot) dans le corps et le JSON-LD - les 9 articles de PR ont donc vraisemblablement déjà été corrigés sur ces deux points lors du PR #11, contrairement à ce que sa description laissait entendre sur la marque. À vour au prochain article : confirmer que les 9 articles n'ont aucune occurrence résiduelle de `/blog/` ou de `Optimas Protect` (deux mots) avant leur éventuelle fusion. Aucun champ `canonical` explicite n'est présent dans le frontmatter de cet article (champ optionnel) : à ajouter systématiquement sur les prochains articles pour lever toute ambigvété.

Conséquence : la pause de production décidée le 2026-08-29 pour motif d'incertitude sur l'URL est levée. La seule raison de pause restant ce run (2026-08-30) est la cadence hebdomadaire déjà largement dépassée (voir rapport du jour).

## Accès au dépôt

Authentifié en tant que `KhalidBougria` (propriétaire du compte), pas `obougria` comme prévu au prompt de référence — le connecteur GitHub MCP de cette session est configuré sur le compte propriétaire directement. Permissions confirmées : `push: true`, `admin: true`. Voie technique : connecteur MCP GitHub local (`local_unpacked_qunfei-wu_github-mcp-server-js`). Visibilité du dépôt : `public` côté API. Branche par défaut : `main`.

## Générateur de site

Aucun générateur n'est présent dans le dépôt (aucun `astro.config.*`, `next.config.*`, `hugo.toml`, `package.json`, etc.). Le dépôt sert uniquement de dépôt de contenu (Markdown) et de suivi (`.seo/`). **Alerte haute permanente :** sans générateur ni pipeline de build/déploiement connu sur ce dépôt, aucun article produit par cet agent ne peut devenir une page live tant qu'un humain n'a pas branché un générateur de site statique sur ce dépôt (ou relié le générateur existant du site `optimasprotect.ma` à ce dépôt). Toujours non résolu ce run (2026-08-30).

## Conventions établies par cet agent

- **Dossier de contenu :** `content/blog/` (dans les branches `article/*` uniquement ; absent de `main`).
- **Nom de fichier :** `{slug}.md`, où `{slug}` est le slug court.
- **URL publique visée :** `https://optimasprotect.ma/articles/{slug}` — établie, arbitrée le 2026-08-29 (voir ci-dessus).
- **Liens internes :** relatifs, `/articles/{slug}`.
- **Marque :** `OptimasProtect` en un seul mot pour la production future.

### Schéma de frontmatter YAML (référence)

```yaml
---
title: "Titre 50 à 60 caractères"
description: "Meta description 140 à 160 caractères"
slug: "slug-court"
tags: ["Tag 1", "Tag 2", "Tag 3"]
date: "2026-08-30"
author: "Team Optimas"
draft: true
focus_keyword: "mot-clé focus"
pillar: "1"
score: 18
canonical: "https://optimasprotect.ma/articles/slug-court"
---
```

Aucun champ image. Le champ `canonical` doit désormais être systématiquement renseigné (absent sur les 9 articles existants, à ajouter si fusion).

### Corps de l'article

Markdown standard (H1 unique en première ligne du corps sous forme `# Titre`, puis H2/H3). Pas de classes CSS spécifiques tant qu'aucun thème n'est branché.

### JSON-LD

En fin de corps d'article dans un bloc ```json-ld```. Types : `SoftwareApplication` + `Offer` pour les articles pilier 1 avec prix, `Article` avec `author.@type: Organization`, `FAQPage` pour le bloc FAQ.

## Hubs en constitution

- Hub pilier 1 (traçabilité / contrôle de ronde) : `controle-de-ronde-nfc-gardiennage-maroc`.
- Hub prix : `prix-logiciel-gardiennage-maroc`.
- Hub conformité (Loi n°27-06 / cahiers des charges) : **deux articles depuis le 2026-08-31** (`cahier-des-charges-gardiennage-maroc`, exigences de marché ; `obligations-loi-27-06-employeur-maroc`, obligations propres à l'employeur). Sujets candidats pour un troisième article ou un enrichissement de PR #8 : rondes électroniques obligatoires (150/mois), conformité marchés publics sécurité (120/mois), voir `.seo/backlog.md`.

## Veille concurrentielle — URLs de référence

- **Cercle 1 (Maroc) :** SEKUR Africa — `sekur-africa.com/logiciel/logiciel-securite-privee-gardiennage-maroc/` (aucun prix inline), `sekur-africa.com/tarifs/` (EUR uniquement, grille 59,99 à 29,99 € HT/mois selon engagement pour 10 licences). Le site français `sekur.fr` (hors périmètre Maroc mais à garder en tête) affiche désormais un prix d'appel distinct à partir de 69,99 € HT/mois. SEKUR Africa a publié un comparatif sectoriel (`sekur-africa.com/meilleurs-logiciels-securite-privee-2025/`) — format à garder en tête comme idée future (prudence §8.2). Opacité tarifaire MAD toujours confirmée (reconfirmé 2026-08-31).
- **Cercle 2 (international) :** Trackforce Valiant - `trackforce.com/fr/solutions/gestion-des-gardiens-de-securite/`. Pricing toujours non public. Positionnement international réaffirmé (300 000+ professionnels, 30 000+ sites, 45 pays), aucune adaptation Maroc identifiée.
- Ne pas confondre SEKUR Africa avec SEKUR France, hors périmètre Maroc.

## Alertes non résolues (arbitrage humain attendu)

1. **Connexion du dépôt Git au site live :** toujours pas de preuve directe que ce dépôt alimente `optimasprotect.ma` / la page `/articles`. La structure d'URL a été arbitrée par l'utilisateur, mais le mécanisme technique réel de publication (générateur de site) reste à brancher sur ce dépôt. Non résolu au 2026-08-31.
2. `robots.txt` : toujours non vérifié (URL hors du périmètre autorisé pour l'outil de fetch de cette session).
3. `site:optimasprotect.ma` : reconfirmé à 0 résultat indexé le 2026-08-31 (recherche web).
4. **Point de suivi (2026-09-01) :** 12 PR ouvertes, aucune fusionnée depuis plus d'une semaine et demie. Non bloquant pour la veille et la production, mais à signaler tant qu'aucune relecture humaine n'a eu lieu.

## Confirmation positive

Le format de frontmatter et le dossier `content/blog/{slug}.md` établis au premier run fonctionnent toujours sans ajustement : 12 articles produits à ce jour (aucun nouvel article le 2026-08-29 ; 1 le 2026-08-30, PR #12 ; 1 le 2026-08-31, PR #13 ; 1 le 2026-09-01, PR #14 ; voir rapports).
