# Backlog éditorial — Optimas Protect

Dernière mise à jour : 2026-08-29.

## PR ouvertes (en attente de relecture humaine)

- PR #1 `controle-de-ronde-nfc-gardiennage-maroc` — pilier 1 — hub pilier 1.
- PR #2 `prix-logiciel-gardiennage-maroc` — pilier 1 — hub prix.
- PR #4 `main-courante-electronique-maroc` — pilier 2 — cluster 6.
- PR #5 `portail-client-securite-privee-maroc` — pilier 2.
- PR #6 `planning-agents-securite-maroc` — pilier 3.
- PR #7 `modele-rapport-de-ronde-maroc` — pilier 1 — cluster 5.
- PR #8 `cahier-des-charges-gardiennage-maroc` — pilier 1 — cluster 7, hub conformité. Article réglementaire, reste en PR en permanence (§3.3).
- PR #9 `application-pointage-ads-maroc` — pilier 1 — cluster 3.
- PR #10 `rapport-intervention-ads-maroc` — pilier 2 — cluster 5 (variante).

Les 9 PR restent ouvertes, aucune n'est encore mergée via l'interface GitHub (reconfirmé 2026-08-29). Répartition actuelle par pilier : pilier 1 = 5/9 (≈56 %), pilier 2 = 3/9 (≈33 %), pilier 3 = 1/9 (≈11 %). Proche du ratio cible 60/30/10 du §0.

## ✅ Alerte critique du 2026-08-26 (workflow copie-repo) — pleinement résolue

Voir `.seo/repo-map.md` pour le détail. Point clos, plus resurveillé sauf réapparition.

## Correction de sourçage (rappel, 2026-08-25)

Une version antérieure du backlog citait une « loi n°38-12 » comme texte régissant les marchés publics. La recherche de sourçage n'a pas confirmé ce numéro de loi. Textes confirmés : le régime des marchés publics par décret (décret n°2-12-349, puis décret n°2-22-431 de 2023) et, pour l'obligation de mention des normes dans les cahiers des charges, la loi n°12-06 du 11 février 2010 relative à la normalisation, à la certification et à l'accréditation (source IMANOR), utilisée dans PR #8. Ne pas réutiliser « loi n°38-12 » sans confirmation directe sur sgg.gov.ma.

## ⏸️ Décision du 2026-08-29 : pause de production maintenue

Semaine S35 (24–30 août) : 5 articles déjà produits du lundi au jeudi. La cadence cible du §9 (2 à 3 articles/semaine en phase de lancement) est déjà largement dépassée cette semaine. Le 2026-08-28, une première pause avait été décidée pour ce motif. Ce run (2026-08-29), la pause est maintenue et renforcée par un nouveau motif : la découverte d'une page `/articles` sur le site live, dont la structure d'URL contredit l'hypothèse `/blog/` utilisée dans les 9 PR déjà ouvertes (voir alerte critique du 2026-08-29 dans `.seo/repo-map.md`). Produire un dixième article avant l'arbitrage de ce point risquerait de compounder une éventuelle erreur de structure d'URL sur encore plus de contenu. Conformément à « qualité avant quota » (§8.4) et à la règle du §4.1 (« une journée sans article publié est normale, une journée sans veille ne l'est pas »), **aucun nouvel article n'a été produit ce run**. Veille complète réalisée à la place (étapes 1, 2, 3 et 6 du §4.1).

## Sujets scorés, prêts pour la prochaine journée de production (une fois l'alerte /articles arbitrée)

1. **Obligations de la Loi n°27-06 pour l'employeur** — pilier 1 (régime renforcé, réglementaire), cluster 8, deuxième article du hub conformité. **Score : 18/25** (intention 4, faisabilité 4, avantage local 5, volume 2, fraîcheur 3). Sourçage à démarrer : la Loi n°27-06 elle-même (dahir n°1-07-155, décret n°2-09-97, déjà confirmés et cités dans PR #8) ; ajouter une recherche ciblée CNSS si le sujet dérive vers le pilier 3 RH. Signal autocomplete revérifié ce run (2026-08-29, gl=ma hl=fr) : toujours 0 suggestion sur « obligations loi 27-06 employeur ». Priorité haute — complète un hub conformité qui n'a qu'un seul article à ce jour.
2. **Faux pointage ADS : comment le détecter sans accuser ses agents** — pilier 1/2 croisé, cluster 9. **Score : 16/25** (intention 4, faisabilité 3, avantage local 4, volume 2, fraîcheur 3). Signal autocomplete toujours à 0 suggestion ce run ; score de demande calculé via l'outil dédié : 3/5 (Trends moyen 1,9, cohérent avec un marché jeune). Angle distinct de `application-pointage-ads-maroc` (qui décrit l'outil) : celui-ci traite spécifiquement de la détection d'anomalies. Attention garde-fou §8.2 : pas de ton accusateur envers les agents.

Ces deux sujets restent valides et prêts à rédiger dès que l'alerte `/articles` du 2026-08-29 aura été arbitrée par un humain, ou dès qu'une prochaine session jugera raisonnable de reprendre la production malgré l'incertitude (à sa discrétion). Priorité au sujet 1 selon le ratio §0.

## Veille concurrentielle mise à jour ce run (2026-08-29)

**SEKUR Africa** : la page dédiée Maroc (`sekur-africa.com/logiciel/logiciel-securite-privee-gardiennage-maroc/`) ne publie toujours aucun prix inline. La page d'accueil du site annonce un prix d'appel « à partir de 99,99 € / mois pour 6 utilisateurs », un chiffre différent de celui précédemment relevé sur la page `/tarifs/` (59,99 € à 29,99 € HT/mois selon engagement pour 10 licences) — les deux pages coexistent avec des grilles différentes, à recouper si besoin dans un futur article comparatif. SEKUR Africa a également publié un article de blog comparatif type « top 5 logiciels de sécurité privée » — un format de contenu qu'Optimas Protect n'a pas encore, à garder en tête (avec prudence sur le garde-fou §8.2). Aucun prix en dirhams n'est publié nulle part sur le site pour le marché marocain — l'opacité tarifaire MAD reste un point d'appui éditorial pour Optimas Protect.

**Trackforce Valiant** : toujours aucun prix public (sur devis), reconfirmé.

**optimasprotect.ma** : toujours 0 résultat indexé sur `site:optimasprotect.ma` (reconfirmé via recherche web ce run).

## Rappel technique (non résolu, arbitrage humain toujours attendu)

Voir `.seo/repo-map.md` pour le détail complet : (1) connexion du dépôt Git au site live toujours non confirmée, complexifiée par la découverte de la page `/articles` en chargement dynamique ce run ; (2) écart de marque « OptImasProtect » (site live) vs « Optimas Protect » (charte de cet agent) toujours non arbitré ; (3) `robots.txt` non vérifié ce run (URL hors du périmètre autorisé pour l'outil de fetch de cette session).
