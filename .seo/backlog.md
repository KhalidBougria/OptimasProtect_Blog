# Backlog éditorial — OptimasProtect

Dernière mise à jour : 2026-09-01 (deuxième session de la semaine S36).

## PR ouvertes (en attente de relecture humaine)

- PR #1 `controle-de-ronde-nfc-gardiennage-maroc` — pilier 1 — hub pilier 1.
- PR #2 `prix-logiciel-gardiennage-maroc` — pilier 1 — hub prix.
- PR #4 `main-courante-electronique-maroc` — pilier 2 — cluster 6.
- PR #5 `portail-client-securite-privee-maroc` — pilier 2.
- PR #6 `planning-agents-securite-maroc` — pilier 3.
- PR #7 `modele-rapport-de-ronde-maroc` — pilier 1 — cluster 5.
- PR #8 `cahier-des-charges-gardiennage-maroc` — pilier 1 — cluster 7, hub conformité. Article réglementaire, reste en PR en permanence (§3.3). Volume utilisateur confirmé (200/mois) — reste la PR la plus prioritaire à relire du backlog.
- PR #9 `application-pointage-ads-maroc` — pilier 1 — cluster 3.
- PR #10 `rapport-intervention-ads-maroc` — pilier 2 — cluster 5 (variante).
- PR #12 `loi-32-26-agents-securite-maroc` — pilier 3 — Loi n°32.26 (journée de 8h). Score 21/25, article réglementaire, reste en PR en permanence.
- PR #13 `obligations-loi-27-06-employeur-maroc` — pilier 1 — cluster 8, hub conformité. Score 18/25, article réglementaire, reste en PR en permanence (§3.3).
- **PR #14 `faux-pointage-ads-detecter-maroc` (nouveau, 2026-09-01)** — pilier 1 — cluster 9, croisé 1/2. Score 16/25, article non réglementaire. Angle douleur → solution : signaux à vérifier avant d'accuser, comparatif registre papier / preuve NFC, posture non accusatoire envers les agents (§8.2). Premier sujet de la file d'attente établie le 2026-08-31, en attente depuis le 2026-08-26.

**12 PR ouvertes, aucune fusionnée à ce jour** (dépôt actif depuis le 2026-08-22, plus d'une semaine et demie sans relecture humaine). Répartition par pilier après PR #14 : pilier 1 = 7/12 (≈58 %), pilier 2 = 3/12 (≈25 %), pilier 3 = 2/12 (≈17 %) — pilier 1 proche de la cible 60 %, pilier 2 sous la cible 30 % (25 %), pilier 3 au-dessus de la cible 10 % (17 %). Prochaine session : privilégier un sujet pilier 2 réellement neuf si le seuil de 14/25 est atteint en veille, sinon rester sur le pilier 1 conformément à la règle de bascule (§0).

## Signaux mots-clés vérifiés ce run (2026-09-01)

Autocomplete (`gl=ma`, `hl=fr`) sur 8 requêtes ciblées pilier 2 et cluster 9 : marché toujours pauvre en autocomplete, cohérent avec les runs précédents. « faux pointage agent de sécurité », « contrôler ses agents de sécurité à distance », « transparence prestations sécurité privée », « société de sécurité litige client prestation » : 0 suggestion. « portail client sécurité » : une seule suggestion hors sujet (« espace client sécurité sociale »). « gestion des incidents sécurité » : suggestions dominées par la cybersécurité (ANSSI, ISO 27035), confirmant la mise en garde du §4.3 sur les têtes de requête génériques à ne pas attaquer. « rapport d'incident agent de sécurité » : signal intéressant (« exemple rapport d'incident agent de sécurité pdf »), mais intention proche de PR #10 déjà existante (rapport d'intervention) — pas retenu comme sujet distinct ce run pour éviter un doublon d'intention. Trends (`geo=MA`, 12 mois) sur 3 mots-clés pilier 2/cluster 9 : plat à 0 sauf deux pics isolés à 95-100 (un seul point chacun, cohérent avec le comportement déjà documenté sur ce marché, à interpréter avec prudence).

Aucun sujet pilier 2 réellement neuf n'a passé le seuil de 14/25 ce run : conformément à la règle de bascule (§0), la production est restée sur le pilier 1, avec le sujet déjà en tête de file (« Faux pointage ADS »).

## Sujets scorés en file d'attente

| Sujet | Pilier | Score /25 | Statut |
|---|---|---|---|
| Rondes électroniques obligatoires (conformité) | 1, cluster 7 | **15** | En file depuis le 2026-08-26. Volume utilisateur rapporté : 150/mois. Décision reportée : enrichir PR #8 (section dédiée) vs nouvel article court — à trancher à la prochaine session de production, après relecture complète du contenu actuel de PR #8. |
| Conformité marchés publics sécurité | 1, cluster 7 | **15** | En file depuis le 2026-08-26. Volume utilisateur rapporté : 120/mois. Recoupe le cluster 7 et la nuance du §4.3.7. Même décision en attente : enrichir PR #8 vs article dédié. |

## Décision prise ce run

**1 article produit et déposé en PR** (PR #14, `faux-pointage-ads-detecter-maroc`, score 16/25) — dernier sujet resté en tête de file depuis le 2026-08-26, prêt à produire. C'est la deuxième session de la semaine S36 (la première, le 2026-08-31, avait produit PR #13).

Les deux sujets scorés ci-dessus (rondes électroniques obligatoires, conformité marchés publics) restent en tête de file pour la suite de la semaine S36. Décision à prendre à la prochaine session : enrichir PR #8 (hub conformité déjà dense, 2 articles) plutôt que de multiplier les articles courts sur des variantes proches du même cluster 7, sauf si la relecture de PR #8 montre un angle clairement distinct.

## Veille concurrentielle (vérifiée ce run)

- **SEKUR Africa** : aucun changement structurel détecté depuis le 2026-08-31. `sekur.fr` a publié un comparatif « meilleurs logiciels sécurité privée 2026 » (`sekur.fr/meilleurs-logiciels-securite-privee-2026/`), succédant à la version 2025 déjà documentée — signal de fraîcheur éditoriale du concurrent à surveiller, sans changement de positionnement Maroc identifié. Opacité tarifaire MAD toujours confirmée côté Maroc.
- **Trackforce Valiant** : aucun changement détecté, toujours positionné à l'international, pricing sur devis.
- Aucun nouvel acteur marocain détecté.

## Rappel technique (non résolu)

Voir `.seo/repo-map.md` : absence de générateur de site connecté au dépôt — alerte haute permanente. `site:optimasprotect.ma` reconfirmé à 0 résultat indexé ce run (recherche web).
