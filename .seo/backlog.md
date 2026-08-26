# Backlog éditorial — Optimas Protect

Dernière mise à jour : 2026-08-26.

## Publiés / en attente de relecture (PR ouvertes)

- `controle-de-ronde-nfc-gardiennage-maroc` — pilier 1 — PR #1 (draft) — hub pilier 1.
- `prix-logiciel-gardiennage-maroc` — pilier 1 — PR #2 (draft) — hub prix.
- `main-courante-electronique-maroc` — pilier 2 — PR #4 (draft) — cluster 6, futur hub pilier 2.
- `portail-client-securite-privee-maroc` — pilier 2 — PR #5 (draft) — premier article du futur hub pilier 2.
- `planning-agents-securite-maroc` — pilier 3 — PR #6 (draft) — premier article de ce pilier, candidat au futur hub pilier 3.
- `modele-rapport-de-ronde-maroc` — pilier 1 — PR #7 (draft) — cluster 5, jalon intermédiaire cité au §9 du prompt de référence.
- `cahier-des-charges-gardiennage-maroc` — pilier 1 — PR #8 (draft) — cluster 7, premier article du hub conformité. Article réglementaire, reste en PR même en phase 2 (§3.3). Un point `[À VÉRIFIER]` reste dans le corps (lien direct Bulletin Officiel / SGG vers le dahir n°1-07-155 et le décret n°2-09-97, non localisé avec certitude par recherche web ce run).
- `application-pointage-ads-maroc` — pilier 1 — PR #9 (draft) — cluster 3, produit ce run. Distinct du contrôle de ronde (preuve de présence en début/fin de poste, vs preuve de passage à des points fixes pendant le poste).

Les 9 PR sont toujours ouvertes côté GitHub (aucune n'a été mergée nativement via l'interface). **Voir `.seo/repo-map.md`, mise à jour du 2026-08-26 : un workflow GitHub Actions (`copie-repo`) force-pousse chaque jour à 10:00 UTC le contenu de toutes les branches `article/*` directement sur `main`, ce qui a déjà republié les 7 premiers articles sur `main` indépendamment de l'état de review des PR. Alerte haute critique, action humaine requise.**

## Correction de sourçage (2026-08-25, rappel)

Le point 3 de ce backlog (version du 2026-08-24) citait une « loi n°38-12 » comme texte régissant les marchés publics. La recherche de sourçage n'a pas confirmé ce numéro de loi. Les textes confirmés sont : le régime des marchés publics par décret (décret n°2-12-349, puis décret n°2-22-431 de 2023) et, pour l'obligation de mention des normes dans les cahiers des charges, la **loi n°12-06** du 11 février 2010 relative à la normalisation, à la certification et à l'accréditation (source IMANOR). C'est cette loi n°12-06 qui a été utilisée dans l'article `cahier-des-charges-gardiennage-maroc` (PR #8). Ne pas réutiliser « loi n°38-12 » dans un futur article sans confirmation directe sur sgg.gov.ma.

## Sujets retenus, à produire aux prochains runs

1. **Faux pointage ADS : comment le détecter sans accuser ses agents** — pilier 1/2 croisé, cluster 9. Toujours aucune confirmation autocomplete au 2026-08-26 (0 suggestion sur "faux pointage agent de sécurité"). Angle produit distinct de `application-pointage-ads-maroc` (celui-ci décrit ce que l'outil doit couvrir ; le sujet 1 traite spécifiquement de la détection d'anomalies). Attention garde-fou §8.2 : pas de ton accusateur envers les agents.
2. **Obligations Loi n°27-06 pour l'employeur** — cluster 8, hub conformité (deuxième article du hub après PR #8). Article réglementaire, même régime renforcé. Sourçage à démarrer : la Loi n°27-06 elle-même (dahir n°1-07-155, décret n°2-09-97, déjà confirmés et cités dans PR #8) couvre une partie du sujet ; ajouter au prochain run une recherche ciblée sur les obligations sociales CNSS si le sujet dérive vers le pilier 3 RH.

## Veille concurrentielle à noter

SEKUR Africa (`sekur-africa.com/logiciel/logiciel-securite-privee-gardiennage-maroc/`) ne communique toujours aucun prix public au 2026-08-26 : l'opacité tarifaire reste un point d'appui pour Optimas Protect sur le marché marocain. SEKUR met en avant une géolocalisation GPS au moment du pointage, à distinguer de la preuve de passage NFC ponctuelle d'Optimas Protect. SEKUR (France, `sekur.fr`) publie un comparatif 2026 avec prix affichés en euros (9,99 à 99,99 EUR HT/mois), mais ceci ne concerne pas le marché marocain.

## Rappel technique

Le site `https://optimasprotect.ma/` est accessible en fetch depuis le 2026-08-25, mais aucune section `/blog/` n'y est visible et le dépôt de contenu semble non connecté au site live (voir `.seo/repo-map.md`). La production continue en PR mais aucun contenu ne devient une page live consultable par ce biais. Le site live affiche « OptImasProtect » (un mot) alors que la charte de cet agent impose « Optimas Protect » (deux mots) — écart à arbitrer par un humain. Nouvelle alerte du 2026-08-26 : un workflow GitHub Actions republie déjà tout le contenu produit sur `main` en quelques heures, contournant la Phase 1 de relecture voulue par la tâche planifiée.
