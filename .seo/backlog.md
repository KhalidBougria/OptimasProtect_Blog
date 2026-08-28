# Backlog éditorial — Optimas Protect

Dernière mise à jour : 2026-08-28.

## PR ouvertes (en attente de relecture humaine)

- PR #1 `controle-de-ronde-nfc-gardiennage-maroc` — pilier 1 — hub pilier 1.
- PR #2 `prix-logiciel-gardiennage-maro` — pilier 1 — hub prix.
- PR #4 `main-courante-electronique-maro`)— pilier 2 — cluster 6.
- PR #5 `portail-client-securite-privee-maroc` — pilier 2.
- PR #6 `planning-agents-securite-maro` — pilier 3.
- PR #7 `modele-rapport-de-ronde-maroc` — pilier 1 — cluster 5.
- PR #8 `cahier-des-charges-gardiennage-maroc` — pilier 1 — cluster 7, hub conformité. Article réglementaire, reste en PR permanemment (§3.3).
- PR #9 `application-pointage-ads-maroc` — pilier 1 — cluster 3.
- PR #10 `rapport-intervention-ads-maroc` — pilier 2 — cluster 5 (variante).

Les 9 PR restent ouvertes, aucune ne est encore mergée via l'interface GitHub. Répartition actuelle par pilier : pilier 1 = 5/9 (≈56 %), pilier 2 = 3/9 (≈33 %), pilier 3 = 1/9 (≈11 %). Proche du ratio cible 60/30/10 du §0 du prompt de référence.

## ✅ Alerte critique du 2026-08-26 (workflow copie-repo) — pleinement résolue, reconfirmé 2026-08-28

Le workflow GitHub Actions `.github/workflows/main.yml` (job `copie-repo`, cron quotidien 10:00 UTC) qui force-poussait chaque branche `article/*` directement sur `main` sans passer par la relecture de PR a été supprimé le 2026-08-26T11:05:39Z (commit `bbfd0fb7`). Ce r{勥 reconfirme : `list_workflows` renvoie à nouveau `total_count: 0`. Le 2026-08-27 à 17:34-17:35 UTC, les 7 fichiers `content/blog/*.md` qui avaient été force-poussés sur `main` avant la suppression du workflow ont été supprimés de l'arborescence (7 commits `Delete content/blog/*.md`). Confirmé ce run par listing de la racine de `main` : seul `.seo/` est présent, aucun `content/` ni `.github/`. L'historique Git conserve la trace de l'épisode (non réécrite), ce qui est normal et utile pour l'audit, mais l'état courant du dépôt est propre. La Phase 1 (relecture par PR) est donc pleinement effective dans les faits, pas seulement dans le processus déclaré par l'agent. Point clos, ne plus resurveiller sauf réapparition d'un nouveau workflow.

## Correction de sourcage (rappel, 2026-08-25)

Une version antérieure du backlog citait une « loi n°38-12 » comme texte régissant les marchés publics. La recherche de sourcage n'a pas confirmé ce numéro de loi. Textes confirmés : le régime des marchés publics par décret (décret n°2-12-349, puis décret n°2-22-431 de 2023) et, pour l'obligation de mention des normes dans les cahiers des charges, la loi n°12-06 du 11 février 2010 relative à la normalisation, à la certification et à l'accréditation (source IMANOR), utilisée dans PR #8. Ne pas réutiliser « loi n°38-12 » sans confirmation directe sur sgg.gov.ma.

## ⏸ Décision du 2026-08-28 : pause de production, cadence hebdomadaire déjà atteinte

Semaine S35 (24-30 août) : 5 articles déjà produits du lundi au jeudi (planning-agents et modèle-rapport-de-ronde le 24, cahier-des-charges le 25, application-pointage le 26, rapport-intervention le 27). La cadence cible du §9 (2 à 3 articles par semaine en phase de lancement) est déjà dépassée cette semaine. Conformément à « qualité avant quota » (§8.4) et à la règle du §4.1 (« une journée sans article publié est normale »), aucun nouvel article n'a été produit ce run (2026-08-28). Veille complète réalisée à la place (étapes 1, 2, 3 et 6).

## Sujets scorés, prêts pour la prochaine journée de production

1. **Obligations de la Loi n°27-06 pour l'employeur** — pilier 1 (régime renforcé, réglementaire), cluster 8, deuxième article du hub conformité. **Score : 18/25** (intention 4, faisabilité 4, avantage local 5, volume 2, fraîcheur 3). Sourcage à démarrer : la Loi n°27-06 elle-même (dahir n°1-07-155, décret n°2-09-97, déjà confirmés et cités dans PR #8) ; ajouter une recherche ciblée CNSS si le sujet dérive vers le pilier 3 RH. Priorité haute — complète un hub conformité qui n'a qu'un seul article à ce jour.
2. **Faux pointage ADS : comment le détecter sans accuser ses agents** — pilier 1/2 croisé, cluster 9. **Score : 16/25** (intention 4, faisabilité 3, avantage local 4, volume 2, fraîcheur 3). Signal autocomplete toujours à 0 suggestion sur « faux pointage agent de sécurité » et « détecter faux pointage agent de sécurité » (revérifié ce run, 2026-08-28, gl=ma hl=fr) — le volume reste la variable la plus faible du score, cohérent avec un marché jeune où l'autocomplete est structurellement pauvre (attendu, pas un échec). Angle distinct de `application-pointage-ads-maroc` (qui décrit l'outil) : celui-ci traite spécifiquement de la détection d'anomalies. Attention garde-fou §8.2 : pas de ton accusateur envers les agents.

Ces deux sujets sont prêts à rédiger dès la prochaine journée de production. Priorité au sujet 1 (hub conformité) selon le ratio §0.

## Veille concurrentielle mise à jour ce run (2026-08-28)

**SEKUR Africa** : la page dédiée Maroc (`sekur-africa.com/logiciel/logiciel-securite-privee-gardiennage-maroc/`) ne publie toujours aucun prix inline — elle renvoie vers `/tarifs/`, une page globale non localisée. Cette page tarifs affiche des prix en **euros uniquement** (59,99€ HT/mois pour 10 licences et tous les modules, dégressif selon engagement : 49,99€ à 12 mois, 39,99€ à 24 mois, 29,99€ à 36 mois ; licence supplémentaire 0,99€ à 0,49€ HT/mois selon palier), sans aucune déclinaison MAD ni mention du Maroc sur cette page précise. Ceci confirme et actualise le point d'opacité déjà noté : aucun prix en dirhams n'est affiché nulle part sur le site SEKUR Africa pour le marché marocain, ce qui reste un point d'appui éditorial pour Optimas Protect (prix MAD affichés, conversion journalière). Ne pas confondre avec sekur.fr (France), hors périmètre.

**optimasprotect.ma** : toujours 0 résultat indexé sur `site:optimasprotect.ma` (revérifié ce run). CoYérent avec les constats précédents.

## Rappel technique (non résolu, arbitrage humain toujours attendu)

Le site `https://optimasprotect.ma/` reste, au dernier contrôle disponible (2026-08-25), sans section `/blog/` visible et le dépôt de contenu ne semble pas connecté au site live (assets pointant vers un outil tiers type GPT Engineer / Lovable). Le site live affiche « OptImasProtect » (un mot) alors que la charte de cet agent impose « optimas Protect » (**sic** — deux mots) — écart toujours à arbitrer par un humain. `robots.txt` non revérifié ce run (non prioritaire tant que le dépôt n'est pas connecté au site live).
