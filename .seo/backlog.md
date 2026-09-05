# Backlog éditorial — OptimasProtect

Dernière mise à jour : 2026-09-05 (semaine S36).

## Décision prise ce run (2026-09-05)

**1 article produit ce run** : `cahier-de-consignes-securite-maroc` (PR #15, pilier 1, score 17/25, `draft: true`). Sujet identifié via autocomplete (`gl=ma`, `hl=fr`) sur « cahier de consignes sécurité » (1 suggestion) puis validé par recherche web : SEKUR (sekur.fr) commercialise une fonctionnalité dédiée « Cahier de consignes » (`sekur.fr/cahier-de-consignes-logiciel-gestion-securite-privee/`), confirmant l'intention business malgré un volume mesurable faible sur ce marché — cohérent avec le régime pauvre en autocomplete déjà documenté ci-dessous.

Nouvelle rotation testée ce run sur des angles pilier 2 non essayés précédemment : « SLA prestation gardiennage », « réclamation client société de sécurité », « litige client société de sécurité preuve », « indicateurs qualité prestation gardiennage » : **0 suggestion pour toutes**, confirmant une fois de plus le régime pauvre en autocomplete sur ce marché pour les angles pilier 2. Rotation pilier 3 testée (« carte professionnelle agent de sécurité Maroc », « congés agent de sécurité Maroc ») : également 0 suggestion. Trends (`geo=MA`, 12 mois) sur trois requêtes pilier 2 : erreur 429 (Google Trends temporairement indisponible ce run, à retenter la prochaine session).

**Décision anti-doublon (§0) :** relecture complète de `main-courante-electronique-maroc` (PR #4) avant rédaction. Le cahier de consignes (instructions permanentes du site, sens donneur d'ordre → agent) est distinct de la main courante (journal d'événements, sens agent → responsable) ; les deux se complètent sans se recouper. Intention confirmée suffisamment distincte pour justifier un nouvel article plutôt qu'un enrichissement.

**Application de la règle de bascule (§0) :** aucun sujet pilier 2 réellement neuf n'a passé le seuil de 14/25 ce run (voir signaux ci-dessus). Le sujet cahier de consignes, bien que pouvant recouper les piliers 1 et 3, a été classé pilier 1 (traçabilité et preuve de transmission des consignes) conformément à la priorité du §0 en l'absence d'alternative pilier 2 qualifiée. L'écart de ratio pilier 2 (25 % contre 30 % cible) n'est donc pas résorbé ce run ; à traiter en priorité dès qu'un sujet pilier 2 franchit le seuil.

`site:optimasprotect.ma` reconfirmé à 0 résultat pertinent indexé ce run (recherche web) — mêmes homonymes sans rapport. `robots.txt` toujours hors du périmètre autorisé pour l'outil de fetch de cette session, donc toujours non vérifié directement.

**Point signalé avec insistance croissante :** le dépôt compte désormais **13 pull requests ouvertes depuis le 2026-08-22, aucune fusionnée** après plus de deux semaines. Ce point est signalé sans interruption depuis le 2026-08-31 et continue de croître en ancienneté sans qu'aucune action humaine n'ait eu lieu. L'alerte haute « aucun générateur de site connecté à ce dépôt » (voir `.seo/repo-map.md`) reste elle aussi active et non résolue.


## Décision prise ce run (2026-09-03)

Aucun article produit ni enrichi ce run. Rotation de mots-clés ciblée sur des angles pilier 1 (clusters 1/2/4) et pilier 2/3 non testés les runs précédents : « logiciel gestion société de sécurité Maroc », « meilleur logiciel gardiennage Maroc », « application ronde agent de sécurité », « traçabilité agents de sécurité Maroc », « reporting mensuel client sécurité privée », « transparence prestations sécurité privée Maroc », « logiciel congés agents de sécurité Maroc », « gestion RH société de sécurité Maroc », « société de sécurité privée Maroc logiciel » : **0 suggestion pour toutes** (autocomplete `gl=ma`, `hl=fr`). Expansion alphabet sur les graines « logiciel gardiennage » et « pointage agent » : aucun signal exploitable — soit hors sujet (logiciels grand public, résultats anglophones parasites), soit déjà couvert par PR #4 (« logiciel registre sécurité ») et PR #6 (« logiciel planning sécurité privée »). Trends (`geo=MA`, 12 mois) sur « logiciel gardiennage maroc », « prix logiciel securite privee », « portail client securite » : plat à 0 sur toute la période et sur toutes les régions.

**Constat structurel :** les 10 clusters prioritaires du §4.2 ont désormais chacun au moins un article en PR (voir table ci-dessous). Aucun angle assez distinct n'est remonté aujourd'hui pour justifier un 13e article sans risquer un doublon d'intention avec un des 12 déjà en attente. Conformément à la règle « une journée sans article publié est normale, une journée sans veille ne l'est pas » (§4.1), ce run est une journée de veille seule.

**Recommandation pour la prochaine session :** l'autocomplete et Trends sont désormais quasi systématiquement à 0 sur ce marché depuis plusieurs runs consécutifs — la boussole a atteint ses limites pratiques avec les outils actuels. Envisager de creuser plutôt via lecture directe des sites concurrents (pages FAQ, forums professionnels marocains, avis clients) ou via l'accès Search Console une fois configuré (voir alerte technique), plutôt que de répéter la même rotation autocomplete.

## Décision prise le run précédent (2026-09-02)

Aucun article distinct produit ce run. À la place : **enrichissement de la PR #8** (`cahier-des-charges-gardiennage-maroc`, hub conformité, score inchangé 20/25) avec deux nouvelles sections répondant aux deux sujets qui restaient en tête de file depuis le 2026-08-26 :

- « Rondes électroniques : une exigence de plus en plus systématique dans les CPS » (répond au sujet précédemment scoré 15/25, volume rapporté 150/mois)
- « Conformité aux marchés publics de sécurité : ce que les donneurs d'ordre vérifient réellement » (répond au sujet précédemment scoré 15/25, volume rapporté 120/mois)

Décision anti-doublon (§0) : la relecture complète du contenu existant de PR #8 a confirmé que ces deux sujets recoupaient son intention (cahier des charges / preuve de passage / hub conformité) sans angle assez distinct pour justifier un article séparé. Enrichissement retenu plutôt que création de nouveaux articles courts. Frontmatter également mis à jour : `date` → 2026-09-02, champ `canonical` ajouté (absent auparavant sur cet article, comme sur les 11 autres), tag « Marchés publics » ajouté (5 tags désormais), `dateModified` du JSON-LD Article mis à jour.

Les deux sujets scorés sont donc retirés de la file d'attente (résolus par enrichissement, pas par nouvel article).

**Aucun sujet pilier 2 réellement neuf n'a passé le seuil de 14/25 ce run** (voir signaux ci-dessous) : conformément à la règle de bascule (§0), l'effort est resté sur le pilier 1.

## PR ouvertes (en attente de relecture humaine) — inchangé, 12 PR

- PR #1 `controle-de-ronde-nfc-gardiennage-maroc` — pilier 1 — hub pilier 1.
- PR #2 `prix-logiciel-gardiennage-maroc` — pilier 1 — hub prix.
- PR #4 `main-courante-electronique-maroc` — pilier 2 — cluster 6.
- PR #5 `portail-client-securite-privee-maroc` — pilier 2.
- PR #6 `planning-agents-securite-maroc` — pilier 3.
- PR #7 `modele-rapport-de-ronde-maroc` — pilier 1 — cluster 5.
- PR #8 `cahier-des-charges-gardiennage-maroc` — pilier 1 — cluster 7, hub conformité. **Enrichie ce run (voir ci-dessus).** Article réglementaire, reste en PR en permanence (§3.3).
- PR #9 `application-pointage-ads-maroc` — pilier 1 — cluster 3.
- PR #10 `rapport-intervention-ads-maroc` — pilier 2 — cluster 5 (variante).
- PR #12 `loi-32-26-agents-securite-maroc` — pilier 3 — Loi n°32.26 (journée de 8h). Score 21/25, article réglementaire, reste en PR en permanence.
- PR #13 `obligations-loi-27-06-employeur-maroc` — pilier 1 — cluster 8, hub conformité. Score 18/25, article réglementaire, reste en PR en permanence.
- PR #14 `faux-pointage-ads-detecter-maroc` — pilier 1 — cluster 9. Score 16/25, article non réglementaire.

**13 PR ouvertes, aucune fusionnée à ce jour** (dépôt actif depuis le 2026-08-22, plus de deux semaines sans relecture humaine — ce point continue de croître). Répartition par pilier : pilier 1 = 8/13 (≈62 %), pilier 2 = 3/13 (≈23 %), pilier 3 = 2/13 (≈15 %). Pilier 1 légèrement au-dessus de la cible 60 % (effet de la règle de bascule, appliquée faute d'alternative pilier 2 qualifiée), pilier 2 sous la cible 30 % (23 %), pilier 3 au-dessus de la cible 10 % (15 %). Prochaine session : privilégier un sujet pilier 2 réellement neuf en priorité absolue si le seuil de 14/25 est atteint en veille, pour corriger l'écart qui se creuse légèrement.

- PR #15 `cahier-de-consignes-securite-maroc` — pilier 1 — nouveau, adjacent au cluster 6 (main courante), intention distincte. Score 17/25, ajouté le 2026-09-05.

## Signaux mots-clés vérifiés ce run (2026-09-02)

Autocomplete (`gl=ma`, `hl=fr`) sur des reformulations pilier 2 / cluster 9 non testées les runs précédents : « logiciel gestion incidents sécurité privée », « reporting client société de sécurité », « suivi intervention agent de sécurité », « registre incidents gardiennage », « compte rendu intervention sécurité privée », « audit prestations sécurité privée », « notification incident client sécurité », « preuve intervention agent sécurité », « digitalisation gardiennage Maroc » : 0 suggestion pour toutes. Confirme une nouvelle fois un marché pauvre en autocomplete sur ces angles.

Signal positif obtenu sur des requêtes déjà couvertes (validation, pas nouveauté) : « rapport de ronde » (expand) fait remonter « rapport de ronde de sécurité », « rapport de ronde de sécurité formulaire », « exemple rapport de ronde agent de sécurité », « rapport de ronde pdf » — confirme la pertinence de PR #7 déjà produite (cluster 5), aucune action nouvelle nécessaire. « logiciel gardiennage » (expand) fait remonter « logiciel planning sécurité privée » (déjà couvert par PR #6) et « logiciel registre sécurité » (proche de la main courante électronique, déjà couverte par PR #4) — pas de sujet distinct retenu, doublons d'intention évités.

Signal faible isolé : « pointage agent de sécurité » (expand) fait remonter « feuille de pointage agent de sécurité », qui n'a pas de suggestions propres à l'expansion — signal trop faible pour passer le seuil de scoring aujourd'hui, à garder en observation.

Trends (`geo=MA`, 12 mois) sur « logiciel gardiennage maroc », « controle de ronde », « pointage agent securite » : plat à 0 sur toute la période sauf un pic isolé à 100 pour « logiciel gardiennage maroc » le 2026-02-08 (un seul point, à interpréter avec prudence, cohérent avec le comportement déjà documenté sur ce marché à faible volume absolu).

## Veille concurrentielle (vérifiée ce run)

- **SEKUR Africa** : grille tarifaire reconfirmée par recherche web ce run, avec des paliers observés (Pack Jeune Entreprise, Pack Gestion, Pack Terrain) en euros — cohérent avec l'opacité tarifaire déjà documentée côté Maroc (aucun prix en MAD affiché). Nouvelle page de comparatif sectoriel déjà notée les runs précédents (`sekur.fr/meilleurs-logiciels-securite-privee-2026/`), aucun changement de positionnement Maroc.
- **Trackforce Valiant** : toujours positionné à l'international, pricing sur devis. Un article tiers (jobsquare.ma) confirme que Trackforce Valiant et GuardTek sont utilisés comme systèmes de supervision de rondes au Maroc — cohérent avec le cercle 2 déjà documenté, aucune action nouvelle.
- Aucun nouvel acteur marocain détecté ce run.

## Rappel technique (non résolu, alerte haute permanente)

Voir `.seo/repo-map.md` : absence de générateur de site connecté au dépôt. `site:optimasprotect.ma` reconfirmé à 0 résultat pertinent indexé ce run (recherche web) — les seuls résultats retournés concernent des entreprises homonymes sans rapport (Optimas Solutions, OptiRTC, etc.), confirmant que le domaine `optimasprotect.ma` n'est pas indexé ou n'a pas de contenu correspondant en ligne. Ce point est distinct de la structure d'URL déjà arbitrée (`/articles/{slug}`) : même si l'URL cible est connue, rien ne prouve que ce dépôt alimente réellement le site live.
