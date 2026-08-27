# Backlog éditorial — Optimas Protect

Dernière mise à jour : 2026-08-27.

## Publiés / en attente de relecture (PR ouvertes)

- `controle-de-ronde-nfc-gardiennage-maroc` — pilier 1 — PR #1 (draft) — hub pilier 1.
- `prix-logiciel-gardiennage-maroc` — pilier 1 — PR #2 (draft) — hub prix.
- `main-courante-electronique-maroc` — pilier 2 — PR #4 (draft) — cluster 6, futur hub pilier 2.
- `portail-client-securite-privee-maroc` — pilier 2 — PR #5 (draft) — premier article du futur hub pilier 2.
- `planning-agents-securite-maroc` — pilier 3 — PR #6 (draft) — premier article de ce pilier, candidat au futur hub pilier 3.
- `modele-rapport-de-ronde-maroc` — pilier 1 — PR #7 (draft) — cluster 5, jalon intermédiaire cité au §9 du prompt de référence.
- `cahier-des-charges-gardiennage-maroc` — pilier 1 — PR #8 (draft) — cluster 7, premier article du hub conformité. Article réglementaire, reste en PR même en phase 2 (§3.3). Un point `[À VÉRIFIER]` reste dans le corps (lien direct Bulletin Officiel / SGG vers le dahir n°1-07-155 et le décret n°2-09-97, non localisé avec certitude par recherche web).
- `application-pointage-ads-maroc` — pilier 1 — PR #9 (draft) — cluster 3, produit le 2026-08-26. Distinct du contrôle de ronde (preuve de présence en début/fin de poste, vs preuve de passage à des points fixes pendant le poste). **Pas encore présent sur `main`** au 2026-08-27 (le workflow qui le republiait a été supprimé avant son prochain déclenchement, voir plus bas).
- `rapport-intervention-ads-maroc` — pilier 2 — PR #10 (draft) — cluster 5 (variante « rapport d'intervention »), produit ce run. Distinct de `modele-rapport-de-ronde-maroc` (passages aux points de contrôle pendant une ronde programmée) et du paragraphe incident de `portail-client-securite-privee-maroc` : traite en profondeur le contenu d'un rapport sur un événement ponctuel hors routine. Score 15/25.

Les 10 PR sont ouvertes côté GitHub, aucune n'a été mergée nativement via l'interface.

## ✅ Alerte critique du 2026-08-26 résolue — workflow `copie-repo` supprimé

Le workflow GitHub Actions `.github/workflows/main.yml` (job `copie-repo`, cron quotidien 10:00 UTC) qui force-poussait chaque branche `article/*` directement sur `main` sans passer par la relecture de PR a été **supprimé** : le dernier commit sur `main` avant ce run est `Delete .github/workflows/main.yml`, signé, par `KhalidBougria`, daté du 2026-08-26T11:05:39Z — soit peu après le signalement de l'alerte dans le rapport du 2026-08-26. `list_workflows` confirme `total_count: 0` sur le dépôt ce run. La Phase 1 (relecture par PR) est de nouveau pleinement effective pour toute nouvelle branche `article/*` : c'est pour cela qu'`application-pointage-ads-maroc` (PR #9, créée le 2026-08-26) n'a pas été republiée sur `main` avant la suppression du workflow.

**Point non résolu :** les 7 articles déjà force-poussés sur `main` avant la suppression (controle-de-ronde-nfc, prix-logiciel, main-courante-electronique, modele-rapport-de-ronde, planning-agents-securite, portail-client-securite-privee, cahier-des-charges-gardiennage) restent publiés dans l'historique Git de `main`, y compris l'article réglementaire `cahier-des-charges-gardiennage-maroc` qui aurait dû rester en PR en permanence (§3.3). Cela ne peut pas être défait par l'agent (règle §7.4 : jamais de suppression de fichier existant sans demande explicite) ; c'est un fait acquis à signaler, pas une alerte active.

## Correction de sourçage (2026-08-25, rappel)

Le point 3 de ce backlog (version du 2026-08-24) citait une « loi n°38-12 » comme texte régissant les marchés publics. La recherche de sourçage n'a pas confirmé ce numéro de loi. Les textes confirmés sont : le régime des marchés publics par décret (décret n°2-12-349, puis décret n°2-22-431 de 2023) et, pour l'obligation de mention des normes dans les cahiers des charges, la **loi n°12-06** du 11 février 2010 relative à la normalisation, à la certification et à l'accréditation (source IMANOR). C'est cette loi n°12-06 qui a été utilisée dans l'article `cahier-des-charges-gardiennage-maroc` (PR #8). Ne pas réutiliser « loi n°38-12 » dans un futur article sans confirmation directe sur sgg.gov.ma.

## Sujets retenus, à produire aux prochains runs

1. **Faux pointage ADS : comment le détecter sans accuser ses agents** — pilier 1/2 croisé, cluster 9. Toujours aucune confirmation autocomplete au 2026-08-27 (0 suggestion sur "détecter faux pointage agent de sécurité"). Angle produit distinct de `application-pointage-ads-maroc` (celui-ci décrit ce que l'outil doit couvrir ; ce sujet traite spécifiquement de la détection d'anomalies). Attention garde-fou §8.2 : pas de ton accusateur envers les agents.
2. **Obligations Loi n°27-06 pour l'employeur** — cluster 8, hub conformité (deuxième article du hub après PR #8). Article réglementaire, même régime renforcé. Sourçage à démarrer : la Loi n°27-06 elle-même (dahir n°1-07-155, décret n°2-09-97, déjà confirmés et cités dans PR #8) couvre une partie du sujet ; ajouter au prochain run une recherche ciblée sur les obligations sociales CNSS si le sujet dérive vers le pilier 3 RH.

## Veille concurrentielle à noter

SEKUR Africa (`sekur-africa.com/logiciel/logiciel-securite-privee-gardiennage-maroc/`) ne communiquait toujours aucun prix public au dernier contrôle (2026-08-26) : l'opacité tarifaire reste un point d'appui pour Optimas Protect sur le marché marocain. Pas de nouvelle vérification web ce run (URL hors provenance de session, fetch bloqué techniquement) ; à revérifier au prochain run. SEKUR met en avant une géolocalisation GPS au moment du pointage, à distinguer de la preuve de passage NFC ponctuelle d'Optimas Protect. SEKUR (France, `sekur.fr`) publie un comparatif 2026 avec prix affichés en euros (9,99 à 99,99 EUR HT/mois), mais ceci ne concerne pas le marché marocain.

## Rappel technique

Le site `https://optimasprotect.ma/` reste, au dernier contrôle disponible, sans section `/blog/` visible et le dépôt de contenu ne semble pas connecté au site live (voir `.seo/repo-map.md`, non revérifié ce run). Le site live affiche « OptImasProtect » (un mot) alors que la charte de cet agent impose « Optimas Protect » (deux mots) — écart toujours à arbitrer par un humain.
