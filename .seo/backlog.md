# Backlog éditorial — OptimasProtect

Dernière mise à jour : 2026-08-31 (première session de la semaine S36).

## PR ouvertes (en attente de relecture humaine)

- PR #1 `controle-de-ronde-nfc-gardiennage-maroc` — pilier 1 — hub pilier 1.
- PR #2 `prix-logiciel-gardiennage-maroc` — pilier 1 — hub prix.
- PR #4 `main-courante-electronique-maroc` — pilier 2 — cluster 6.
- PR #5 `portail-client-securite-privee-maroc` — pilier 2.
- PR #6 `planning-agents-securite-maroc` — pilier 3.
- PR #7 `modele-rapport-de-ronde-maroc` — pilier 1 — cluster 5.
- PR #8 `cahier-des-charges-gardiennage-maroc` — pilier 1 — cluster 7, hub conformité. Article réglementaire, reste en PR en permanence (§3.3). Volume utilisateur confirmé (200/mois sur « cahier des charges gardiennage maroc ») — reste la PR la plus prioritaire à relire du backlog.
- PR #9 `application-pointage-ads-maroc` — pilier 1 — cluster 3.
- PR #10 `rapport-intervention-ads-maroc` — pilier 2 — cluster 5 (variante).
- PR #12 `loi-32-26-agents-securite-maroc` — pilier 3 — Loi n°32.26 (journée de 8h pour les agents de sécurité). Score 21/25, article réglementaire, reste en PR en permanence.
- **PR #13 `obligations-loi-27-06-employeur-maroc` (nouveau, 2026-08-31)** — pilier 1 — cluster 8, hub conformité. Score 18/25, article réglementaire, reste en PR en permanence (§3.3). Complète le hub conformité qui n'avait qu'un seul article (PR #8). Distinct de PR #8 (exigences d'un marché/CPS) et de PR #12 (durée du travail) : traite des obligations propres à l'employeur au titre de la loi elle-même (autorisation, registre du personnel, embauche, CNSS).

**11 PR ouvertes, aucune fusionnée à ce jour** (dépôt actif depuis le 2026-08-22, plus d'une semaine sans relecture humaine). Répartition par pilier après PR #13 : pilier 1 = 6/11 (≈55 %), pilier 2 = 3/11 (≈27 %), pilier 3 = 2/11 (≈18 %) — proche de la cible 60/30/10, légèrement sous-représenté sur le pilier 2. Prochaine session : privilégier un sujet pilier 2 réellement neuf si le seuil de 14/25 est atteint, sinon rester sur le pilier 1 conformément à la règle de bascule.

## Signaux mots-clés vérifiés ce run (2026-08-31)

Autocomplete (`gl=ma`, `hl=fr`) sur 15 requêtes en rotation : marché structurellement pauvre en autocomplete, cohérent avec les runs précédents. Signaux positifs : « loi 27 06 relative à la sécurité privée au maroc pdf » (sous « loi 27-06 sécurité privée »), « main courante électronique gratuite » / « télécharger main courante électronique gratuite », « contrôleur de ronde prix maroc » (variante orthographique, à noter : cette formulation évoque potentiellement un équipement physique plutôt qu'un logiciel — à surveiller si elle prend du volume), « planning agent de sécurité gratuit excel ». Trends (`geo=MA`, 12 mois) sur 3 mots-clés : plat à 0 sauf un pic isolé à 100 pour « rondes électroniques obligatoires » le 2026-01-18 (un seul point, à interpréter avec prudence sur un volume quasi nul, cohérent avec le comportement déjà documenté sur ce marché).

## Sujets scorés en file d'attente

| Sujet | Pilier | Score /25 | Statut |
|---|---|---|---|
| Rondes électroniques obligatoires (conformité) | 1, cluster 7 | **15** | En file. Volume utilisateur rapporté : 150/mois. Autocomplete/Trends faibles ce run. Angle distinct de PR #1 (« comment ça marche ») : interroge le caractère obligatoire ou non des rondes électroniques. Décision reportée : enrichir PR #8 (section dédiée) vs nouvel article court — à trancher à la prochaine session de production, après relecture complète du contenu actuel de PR #8. |
| Conformité marchés publics sécurité | 1, cluster 7 | **15** | En file. Volume utilisateur rapporté : 120/mois. Recoupe le cluster 7 et la nuance du §4.3.7 (combinaison marchés publics + sécurité privée jouable). Même décision en attente : enrichir PR #8 vs article dédié. |
| Faux pointage ADS : comment le détecter sans accuser ses agents | 1/2 croisé, cluster 9 | **16** | En file depuis le 2026-08-26, inchangé. Prêt à produire à la prochaine session. |

## Décision prise ce run

**1 article produit et déposé en PR** (PR #13, `obligations-loi-27-06-employeur-maroc`, score 18/25) — premier sujet du backlog, en tête de file depuis le 2026-08-28 et reporté à trois reprises pour des raisons de cadence et d'incertitude technique (désormais résolues). C'est le premier jour de la semaine S36 : la cadence hebdomadaire repart à zéro, ce qui justifie de reprendre la production après la pause de la semaine S35.

Les trois sujets scorés ci-dessus restent en tête de file pour la suite de la semaine S36, en commençant par « Faux pointage ADS » (prêt depuis le plus longtemps) sauf si un sujet pilier 2 neuf apparaît en veille, ce qui serait cohérent avec le léger sous-poids actuel du pilier 2.

## Veille concurrentielle (vérifiée ce run)

- **SEKUR Africa** : la page produit dédiée Maroc ne publie toujours aucun prix inline. Le site français (`sekur.fr`) affiche désormais un prix d'appel à partir de 69,99 € HT/mois (offre différente de la grille `/tarifs/` de SEKUR Africa documentée les runs précédents, 59,99 à 29,99 € HT/mois selon engagement). Aucune déclinaison en dirhams détectée. L'opacité tarifaire sur le marché marocain reste confirmée et reste un point d'appui éditorial pour OptimasProtect (prix MAD affichés publiquement).
- **Trackforce Valiant** : toujours positionné à l'international (300 000+ professionnels, 30 000+ sites, 45 pays), aucune mention spécifique au Maroc trouvée ce run, pricing toujours sur devis.
- Aucun nouvel acteur marocain détecté.

## Rappel technique (non résolu)

Voir `.seo/repo-map.md` : absence de générateur de site connecté au dépôt — alerte haute permanente, distincte de la question de structure d'URL (déjà arbitrée). `site:optimasprotect.ma` reconfirmé à 0 résultat indexé ce run (recherche web).
