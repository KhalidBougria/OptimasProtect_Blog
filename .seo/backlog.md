# Backlog éditorial — OptimasProtect

Dernière mise à jour : 2026-08-30.

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

Les 9 PR restent ouvertes, aucune n'est encore mergée (reconfirmé 2026-08-30). Répartition par pilier : pilier 1 = 5/9 (≈56 %), pilier 2 = 3/9 (≈33 %), pilier 3 = 1/9 (≈11 %). Proche du ratio cible 60/30/10.

## ✅ Arbitrage humain du 2026-08-29 (PR #11) : alerte `/articles` RÉSOLUE

La structure d'URL cible est confirmée à `/articles/{slug}` (et non `/blog/{slug}`). La marque s'écrit désormais `OptimasProtect` (un mot) pour la production future. Voir `.seo/repo-map.md` pour le détail et le spot-check effectué ce run sur PR #1. La raison de pause du 2026-08-29 liée à cette incertitude est donc levée.

## ⏸️ Pause de production maintenue ce run (2026-08-30) — nouveau motif : cadence hebdomadaire

La raison d'incertitude sur l'URL est levée, mais la semaine S35 (24–30 août) a déjà produit 5 articles (lundi à jeudi), contre une cadence cible de 2 à 3 articles/semaine en phase de lancement (§9). De surˆcroît, les 9 PR de la semaine restent toutes non relues par un humain à ce jour. Conformément à « qualité avant quota » (§8.4), aucun dixième article n'est produit aujourd'hui (dernier jour de la semaine S35). Production à reprendre normalement en semaine S36 (31 août–6 septembre), en commençant par le sujet 1 ci-dessous. Veille complète réalisée à la place (étapes 1, 2, 3 et 6 du §4.1).

## Sujets scorés, prêts pour la prochaine journée de production (semaine S36)

1. **Obligations de la Loi n°27-06 pour l'employeur** — pilier 1 (régime renforcé, réglementaire), cluster 8, deuxième article du hub conformité. **Score : 18/25** (intention 4, faisabilité 4, avantage local 5, volume 2, fraîcheur 3). Sourçage : Loi n°27-06 (dahir n°1-07-155, décret n°2-09-97, déjà cités dans PR #8) ; ajouter CNSS si dérive vers pilier 3 RH. Signal autocomplete revérifié ce run (2026-08-30, gl=ma hl=fr) : toujours 0 suggestion sur « obligations loi 27-06 employeur ». Trends (geo=MA, 12 mois) : signal quasi-nul sur les trois requêtes du cluster pilier 1 testées ce run (1 seul pic isolé à 100 sur « contrôle de ronde » la semaine du 2025-11-02, bruit probable sur un marché très jeune). Priorité haute — complète un hub conformité qui n'a qu'un seul article à ce jour.
2. **Faux pointage ADS : comment le détecter sans accuser ses agents** — pilier 1/2 croisé, cluster 9. **Score : 16/25** (intention 4, faisabilité 3, avantage local 4, volume 2, fraîcheur 3). Signal autocomplete toujours à 0 suggestion ce run. Angle distinct de `application-pointage-ads-maroc` (qui décrit l'outil) : celui-ci traite spécifiquement de la détection d'anomalies. Attention garde-fou §8.2 : pas de ton accusateur envers les agents.

## Veille concurrentielle (signal inchangé ce run)

**SEKUR Africa** : toujours aucun prix inline sur la page dédiée Maroc ni en dirhams nulle part sur le site — opacité tarifaire MAD toujours un point d'appui éditorial pour OptimasProtect. **Trackforce Valiant** : toujours sur devis. Non re-vérifié en détail ce run (signal de la veille du 2026-08-29 encore récent); à rafraîchir au prochain jour de production.

## Rappel technique (non résolu)

Voir `.seo/repo-map.md` : (1) connexion du dépôt Git au site live toujours non confirmée - alerte haute permanente (aucun générateur de site branché) ; (2) `robots.txt` non vérifié.
