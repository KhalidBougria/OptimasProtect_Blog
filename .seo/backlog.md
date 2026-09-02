# Backlog éditorial — OptimasProtect

Dernière mise à jour : 2026-09-02 (troisième session de la semaine S36).

## Décision prise ce run (2026-09-02)

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

**12 PR ouvertes, aucune fusionnée à ce jour** (dépôt actif depuis le 2026-08-22, plus de deux semaines sans relecture humaine — ce point continue de croître). Répartition par pilier inchangée : pilier 1 = 7/12 (≈58 %), pilier 2 = 3/12 (≈25 %), pilier 3 = 2/12 (≈17 %). Pilier 1 proche de la cible 60 %, pilier 2 sous la cible 30 % (25 %), pilier 3 au-dessus de la cible 10 % (17 %). Prochaine session : privilégier un sujet pilier 2 réellement neuf si le seuil de 14/25 est atteint en veille.

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
