# Backlog éditorial — OptimasProtect

Dernière mise à jour : 2026-08-30 (mise à jour intraday suite à des signaux mots-clés fournis par l'utilisateur).

## PR ouvertes (en attente de relecture humaine)

- PR #1 `controle-de-ronde-nfc-gardiennage-maroc` — pilier 1 — hub pilier 1.
- PR #2 `prix-logiciel-gardiennage-maroc` — pilier 1 — hub prix.
- PR #4 `main-courante-electronique-maroc` — pilier 2 — cluster 6.
- PR #5 `portail-client-securite-privee-maroc` — pilier 2.
- PR #6 `planning-agents-securite-maroc` — pilier 3.
- PR #7 `modele-rapport-de-ronde-maroc` — pilier 1 — cluster 5.
- PR #8 `cahier-des-charges-gardiennage-maroc` — pilier 1 — cluster 7, hub conformité. Article réglementaire, reste en PR en permanence (§3.3). **Priorité de relecture relevée** : le volume utilisateur (200/mois sur « cahier des charges gardiennage maroc ») en fait le sujet le plus demandé du backlog.
- PR #9 `application-pointage-ads-maroc` — pilier 1 — cluster 3.
- PR #10 `rapport-intervention-ads-maroc` — pilier 2 — cluster 5 (variante).
- **PR #12 `loi-32-26-agents-securite-maroc`** — pilier 3 — nouveau. Loi n°32.26 (journée de 8h pour les agents de sécurité), sujet remonté par l'utilisateur le 2026-08-30, vérifié par recherche web (BO n°7526 du 16 juillet 2026, dahir n°1.26.27 du 3 juillet 2026). **Score 21/25**, article réglementaire, reste en PR en permanence.

10 PR ouvertes, aucune fusionnée à ce jour. Répartition par pilier après PR #12 : pilier 1 = 5/10 (50 %), pilier 2 = 3/10 (30 %), pilier 3 = 2/10 (20 %) — pilier 3 se rapproche du ratio cible (10 %), légèrement au-dessus, ce qui est cohérent avec la règle de bascule du §0 (aucun sujet neuf de pilier 2 disponible ce jour, effort reporté).

## Signaux mots-clés fournis par l'utilisateur (2026-08-30)

L'utilisateur a communiqué trois volumes de recherche mensuels (source externe non précisée, à traiter comme signal qualitatif complémentaire à l'autocomplete/Trends déjà utilisés) :

| Requête | Volume/mois | Statut |
|---|---|---|
| cahier des charges gardiennage maroc | 200 | Déjà couvert par PR #8 (hub conformité). Volume confirme la priorité de relecture de cette PR. |
| rondes électroniques obligatoires | 150 | Non couvert directement. Angle distinct de PR #1 (explicatif « comment ça marche ») : celui-ci interroge le caractère obligatoire ou non des rondes électroniques. Candidat pour enrichir PR #8 (section dédiée) ou nouvel article court, à trancher à la prochaine session de production. |
| conformité marchés publics sécurité | 120 | Non couvert directement. Recoupe le cluster 7 (§4.2) et la nuance du §4.3.7 (combinaison marchés publics + sécurité privée jouable). Candidat pour enrichir PR #8 également, ou article dédié si l'angle marchés publics justifie une intention de recherche distincte. |

**Décision :** ne pas dupliquer sur « cahier des charges gardiennage maroc » (déjà couvert). Les deux autres requêtes sont ajoutées à la file de sujets ci-dessous plutôt que traitées dans l'urgence, pour éviter une modification précipitée d'une PR déjà ouverte (#8) sans relecture complète préalable de son contenu actuel.

## Loi n°32.26 : nouveau texte majeur intégré (PR #12)

Signalée par l'utilisateur le 2026-08-30. Vérification faite par recherche web croisant plusieurs sources de presse marocaine (H24info, Le Matin, La Vie Éco, Telquel), toutes convergentes sur les mêmes références officielles : loi n°32.26 complétant l'article 193 du Code du travail (loi n°65-99), limitant à 8h la journée des agents de sécurité privée (fin des vacations de 12h), Bulletin officiel n°7526 du 16 juillet 2026, dahir n°1.26.27 du 3 juillet 2026, délai de mise en conformité de 9 mois pour les contrats en cours. Article rédigé et publié en PR le jour même (score 21/25, le plus élevé obtenu à ce jour). Distinct de la loi n°27-06 (qui encadre les activités de gardiennage dans leur ensemble) : les deux textes sont cités et distingués explicitement dans l'article pour éviter toute confusion, y compris dans une question de FAQ dédiée.

**Point de vigilance pour la relecture humaine :** le lien source de l'article pointe vers le portail général des Bulletins officiels (sgg.gov.ma/BulletinOfficiel.aspx) et non vers le PDF exact du BO n°7526, faute d'URL directe confirmée par la recherche web menée ce run. À compléter si l'URL exacte est disponible.

## Sujets en file d'attente pour la prochaine session de production

1. **Rondes électroniques obligatoires** — pilier 1, cluster 7 (conformité). Volume utilisateur : 150/mois. À scorer et trancher : enrichissement de PR #8 vs nouvel article.
2. **Conformité marchés publics sécurité** — pilier 1, cluster 7. Volume utilisateur : 120/mois. À scorer et trancher : enrichissement de PR #8 vs nouvel article.
3. **Faux pointage ADS : comment le détecter sans accuser ses agents** — pilier 1/2 croisé, cluster 9. Score : 16/25 (inchangé depuis le 2026-08-29).

## Veille concurrentielle (inchangée depuis le 2026-08-30 matin)

Voir `.seo/repo-map.md` : SEKUR Africa toujours sans prix en dirhams publié pour le Maroc ; Trackforce Valiant toujours sur devis.

## Rappel technique (non résolu)

Voir `.seo/repo-map.md` : absence de générateur de site connecté au dépôt — alerte haute permanente, distincte de l'arbitrage `/articles/` déjà résolu.
