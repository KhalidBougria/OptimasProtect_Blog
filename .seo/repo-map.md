# Cartographie du dépôt — OptimasProtect_Blog

Dernière mise à jour : 2026-08-28. Ce fichier est un document de travail vivant ; pour l'historique détaillé jour par jour, voir `.seo/rapports/`.

## Accès au dépôt

Authentifié en tant que `KhalidBougria` (propriétaire du compte), pas `obougria` comme prévu au prompt de référence — le connecteur GitHub MCP de cette session est configuré sur le compte propriétaire directement. Permissions confirmées : `push: true`, `admin: true`. Voie technique : connecteur MCP GitHub local (`local_unpacked_qunfei-wu_github-mcp-server-js`). Visibilité du dépôt : `public` côté API au 2026-08-28 (le prompt de référence le décrit comme privé ; à noter, pas bloquant pour l'écriture). Branche par défaut : `main`.

## Générateur de site

Aucun générateur n'est présent dans le dépôt (aucun `astro.config.*`, `next.config.*`, `hugo.toml`, `package.json`, etc.). Le dépôt sert uniquement de dépôt de contenu (Markdown) et de suivi (`.seo/`). **Alerte haute permanente :** sans générateur ni pipeline de build/déploiement connu sur ce dépôt, aucun article produit par cet agent ne peut devenir une page live tant qu'un humain n'a pas branché un générateur de site statique sur ce dépôt (ou relié le générateur existant du site `optimasprotect.ma` à ce dépôt).

## Conventions établies par cet agent (à respecter à la lettre)

- **Dossier de contenu :** `content/blog/` (dans les branches `article/*` uniquement à ce jour ; absent de `main`, voir section alerte plus bas).
- **Nom de fichier :** `{slug}.md`, où `{slug}` est le slug court (identique au champ `slug` du frontmatter).
- **URL publique visée :** `https://optimasprotect.ma/blog/{slug}`.
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

En fin de corps d'article dans un bloc ```json-ld`. Types : `SoftwareApplication` + `Offer` pour les articles pilier 1 avec prix, `Article` avec `author.@type: Organization`, `FAQPage` pour le bloc FAQ.

## Hubs en constitution

- Hub pilier 1 (traçabilité / contrôle de ronde) : `controle-de-ronde-nfc-gardiennage-maroc`.
- Hub prix : `prix-logiciel-gardiennage-maroc`.
- Hub conformité (Loi n°27-06 / cahiers des charges) : un seul article à ce jour (`cahier-des-charges-gardiennage-maroc`) ; deuxième article planifié (obligations Loi n°27-06 employeur, voir backlog).

## Veille concurrentielle — URLs de référence

- **Cercle 1 (Maroc) :** SEKUR Africa — `sekur-africa.com/logiciel/logiciel-securite-privee-gardiennage-maroc/` (page produit Maroc, aucun prix inline), `sekur-africa.com/tarifs/` (page tarifs globale non localisée, prix en EUR uniquement : 59,99€ à 29,99€ HT/mois selon engagement). Opacité tarifaire MAD confirmée à nouveau le 2026-08-28.
- **Cercle 2 (international) :** Trackforce Valiant — `trackforce.com/fr/solutions/gestion-des-gardiens-de-securite/`. Pricing non public (sur devis).
- Ne pas confondre SEKUR Africa avec SEKUR France (`sekur.fr`) / `logiciel.sekur.fr`, hors périmètre Maroc.

## ✅ Alerte critique du 2026-08-26 (workflow `copie-repo`) — RÉSOLUE et confirmée closée le 2026-08-28

Un workflow GitHub Actions `.github/workflows/main.yml` (job `copie-repo`, cron quotidien 10:00 UTC) force-poussait chaque branche `article/*` directement sur `main`, contournant la Phase 1 (relecture par PR) imposée par le prompt de référence. Découvert et signalé le 2026-08-26. Supprimé le même jour (11:05:39 UTC, commit `bbfd0fb7`). Les 7 fichiers articles qui avaient été force-poussés avant cette suppression ont ensuite été retirés de l'arborescence `main` le 2026-08-27 (7 commits `Delete content/blog/*.md`, 17:34-17:35 UTC).

**Reéconfirmé ce run (2026-08-28)** : `list_workflows` renvoie `total_count: 0`. Listing de la racine de `main` : seul `.seo/` est présent, aucun `content/` ni `.github/`. L'arborescence courante de `main` est donc strictement limitée à `.seo/`. L'historique Git conserve la trace de l'épisode (non réécrite, normal pour l'audit). La Phase 1 est donc pleinement effective et le point est considéré clos : ne plus resurveiller sauf réapparition d'un nouveau workflow sur ce dépôt.

## Alertes non résolues (arbitrage humain attendu)

1. **Connexion au site live :** `https://optimasprotect.ma/` (dernier contrôle disponible : 2026-08-25) ne montre aucune section `/blog/` en navigation/footer, et ses assets pointent vers `storage.googleapis.com/gpt-engineer-file-uploads/...`, suggérant un site généré par un outil tiers (GPT Engineer / Lovable) non connecté à ce dépôt Git. Aucun article produit par cet agent ne peut donc devenir une page consultable sans intervention humaine.
2. **Écart de marque :** le site live affiche systématiquement « OptImasProtect » (un mot, I majuscule médian) dans le `<title>`, les meta OG/Twitter, le footer et l'alt du logo, alors que le prompt de référence impose « Optimas Protect » en deux mots. L'agent continue d'appliquer la règle du prompt (deux mots) dans les articles, en attendant arbitrage.
3. **`robots.txt` / accessibilité Googlebot :** non vérifiés depuis le 2026-08-25 (outil de fetch ayant bloqué cette URL précise). Non prioritaire tant que le point 1 n'est pas résolu.
4. **`site:optimasprotect.ma` :** toujours 0 résultat indexé sur Google (reconfirmé 2026-08-28).

## Confirmation positive

Le format de frontmatter et le dossier `content/blog/{slug}.md` établis au premier run fonctionnent sans ajustement : 9 articles produits à ce jour, tous conformes.
