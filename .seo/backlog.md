# Backlog éditorial — Optimas Protect

Dernière mise à jour : 2026-08-25.

## Publiés / en attente de relecture (PR ouvertes)

- `controle-de-ronde-nfc-gardiennage-maroc` — pilier 1 — PR #1 (draft) — hub pilier 1.
- `prix-logiciel-gardiennage-maroc` — pilier 1 — PR #2 (draft) — hub prix.
- `main-courante-electronique-maroc` — pilier 2 — PR #4 (draft) — cluster 6, futur hub pilier 2.
- `portail-client-securite-privee-maroc` — pilier 2 — PR #5 (draft) — premier article du futur hub pilier 2.
- `planning-agents-securite-maroc` — pilier 3 — PR #6 (draft) — premier article de ce pilier, candidat au futur hub pilier 3.
- `modele-rapport-de-ronde-maroc` — pilier 1 — PR #7 (draft) — cluster 5, jalon intermédiaire cité au §9 du prompt de référence.
- `cahier-des-charges-gardiennage-maroc` — pilier 1 — PR #8 (draft) — cluster 7, **premier article du hub conformité**. Article réglementaire, reste en PR même en phase 2 (§3.3). Un point `[À VÉRIFIER]` reste dans le corps (lien direct Bulletin Officiel / SGG vers le dahir n°1-07-155 et le décret n°2-09-97, non localisé avec certitude par recherche web ce run).

Les 7 PR sont toujours ouvertes, aucune n'a encore été relue ni mergée par un humain. **Aucun article ne peut devenir une page live pour l'instant : voir alerte haute n°1 mise à jour dans `.seo/repo-map.md` (site live accessible mais probablement non connecté à ce dépôt, pas de section /blog/ visible).**

## Correction de sourçage (2026-08-25)

Le point 3 de ce backlog (version du 2026-08-24) citait une « loi n°38-12 » comme texte régissant les marchés publics et l'obligation de mention des normes dans les cahiers des charges. La recherche de sourçage effectuée ce run ne confirme pas ce numéro de loi. Les textes confirmés sont : le régime des marchés publics par décret (décret n°2-12-349, puis décret n°2-22-431 de 2023) et, pour l'obligation de mention des normes applicables, la **loi n°12-06** du 11 février 2010 relative à la normalisation, à la certification et à l'accréditation (source IMANOR). C'est cette loi n°12-06 qui a été utilisée dans l'article `cahier-des-charges-gardiennage-maroc` (PR #8). Ne pas réutiliser « loi n°38-12 » dans un futur article sans confirmation directe sur sgg.gov.ma.

## Sujets retenus, à produire aux prochains runs

1. **Application de pointage ADS au Maroc : ce qu'un responsable d'exploitation doit vérifier** — pilier 1, cluster 3. Toujours aucune confirmation autocomplete au 2026-08-25 (0 suggestion). Angle produit distinct du contrôle de ronde et du planning déjà publiés ; anti-cannibalisation à revérifier avant rédaction.
2. **Faux pointage ADS : comment le détecter sans accuser ses agents** — pilier 1/2 croisé, cluster 9. Aucune confirmation autocomplete ce run. Attention garde-fou §8.2 : pas de ton accusateur envers les agents.
3. **Obligations Loi n°27-06 pour l'employeur** — cluster 8, hub conformité (deuxième article du hub après PR #8). Article réglementaire, même régime renforcé. Sourçage à démarrer : la Loi n°27-06 elle-même (dahir n°1-07-155, décret n°2-09-97, déjà confirmés et cités dans PR #8) couvre une partie du sujet ; ajouter au prochain run une recherche ciblée sur les obligations sociales CNSS si le sujet dérive vers le pilier 3 RH.

## Rappel technique

**Mise à jour 2026-08-25 :** le site `https://optimasprotect.ma/` est maintenant accessible en fetch (ne l'était pas aux runs précédents), mais aucune section `/blog/` n'y est visible et le dépôt de contenu semble non connecté au site live (voir `.seo/repo-map.md`). La production continue en PR mais aucun contenu ne devient une page live consultable. Nouvelle alerte à signaler à l'utilisateur : le site live affiche « OptImasProtect » (un mot) alors que la charte de cet agent impose « Optimas Protect » (deux mots) — écart à arbitrer par un humain.

## Veille concurrentielle à noter

SEKUR Africa (`sekur-africa.com/logiciel/logiciel-securite-privee-gardiennage-maroc/`) ne communique toujours aucun prix public au 2026-08-25 : l'opacité tarifaire reste un point d'appui pour Optimas Protect sur le marché marocain. SEKUR met en avant une géolocalisation GPS au moment du pointage, à distinguer de la preuve de passage NFC ponctuelle d'Optimas Protect. SEKUR (France, `sekur.fr`) publie un comparatif 2026 avec prix affichés en euros (9,99 à 99,99 EUR HT/mois), mais ceci ne concerne pas le marché marocain.
