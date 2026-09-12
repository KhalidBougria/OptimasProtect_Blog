# Backlog editorial - OptimasProtect

Derniere mise a jour : 2026-09-12 (semaine S37).

## Decision prise ce run (2026-09-12)

0 nouvel article, 0 enrichissement. Rotation testee ce run, 15 requetes sur des angles non essayes precedemment (voir liste complete dans le rapport du jour .seo/rapports/2026-09-12.md) : frequence des rondes de securite, cahier de rondes gardiennage, application mobile agent de securite, ronde de securite sans internet, carte de ronde electronique, supervision agents de securite a distance, tag NFC gardiennage, temps de reponse incident securite privee, digitalisation securite privee Maroc, logiciel de gestion de rondes, verification de presence agent site client, combien coute un pointeur NFC, assurance societe de gardiennage Maroc, sous-traitance gardiennage Maroc, superviseur de securite outils.

Un seul signal exploitable : cahier de rondes gardiennage vers cahier ronde de securite. Score de demande 3/5 (topic_demand_score), mais trends_interest ne montre qu'un pic isole sur la semaine du 2025-10-05, signal ponctuel. Anti-doublon verifie en lisant integralement le contenu de PR 7 (modele-rapport-de-ronde-maroc) : cet article couvre deja cette intention, y compris un tableau comparatif rapport papier / rapport genere automatiquement. Aucun nouvel article, aucune mise a jour necessaire.

Toutes les autres requetes : 0 suggestion, regime pauvre en autocomplete confirme une nouvelle fois sur ce marche.

Decouverte majeure ce run, documentee en detail dans .seo/repo-map.md et .seo/rapports/2026-09-12.md : en verifiant directement le site live (sitemap.xml, robots.txt, pages /articles/slug), il apparait que 12 des 14 articles produits par cet agent sont deja en ligne sur optimasprotect.ma, avec un contenu quasi identique aux branches article, alors qu'aucune des PR correspondantes n'a ete fusionnee sur GitHub. Cela nuance fortement l'alerte historique sur l'absence de generateur de site connecte, et souleve un point a clarifier par l'utilisateur sur l'articulation entre ce mecanisme de publication et la relecture humaine prevue en Phase 1.

Veille concurrentielle (recherche web ce run) : SEKUR / SEKUR Africa toujours en tarification EUR uniquement pour l'offre France, opacite MAD toujours confirmee cote Maroc, aucun changement de positionnement detecte. Trackforce Valiant toujours positionne a l'international, pricing sur devis, aucune adaptation Maroc identifiee. Aucun nouvel acteur marocain detecte au-dela de secumall.ma et kver.ma, deja documentes.

Alerte outillage ce run : le bac a sable Bash de cette session est reste indisponible toute la duree du run (meme erreur de montage Windows du 8 septembre que les runs precedents). Contournement applique avec succes via le navigateur integre.

Point signale avec insistance croissante, a relire avec la nuance de la decouverte ci-dessus : le depot compte toujours 14 pull requests ouvertes depuis le 2026-08-22, aucune fusionnee, soit 21 jours au 2026-09-12. Ce point est signale sans interruption depuis le 2026-08-31, mais sa portee doit desormais etre relativisee : le contenu ne semble pas bloque en pratique, il atteint le site par un autre canal que la fusion GitHub.

Repartition par pilier inchangee depuis le 2026-09-11 (aucun ajout) : pilier 1 = 8/14 (~57%), pilier 2 = 4/14 (~29%), pilier 3 = 2/14 (~14%), proche de la cible 60/30/10.

## Decision prise ce run (2026-09-11)

1 nouvel article produit : PR 16 (controle-qualite-prestation-gardiennage-maroc, pilier 2, score 17/25). Priorite donnee au pilier 2 conformement a l'ecart de ratio signale sans interruption depuis le 2026-08-31 (pilier 2 sous la cible de 30%). Rotation testee ce run, environ 25 requetes sur les trois piliers. Un seul signal exploitable : assurance qualite gardiennage vers controle qualite securite privee. Score 17/25. Article produit et publie en PR 16, pilier 2.

trends_interest (geo=MA, 12 mois) sur justificatif de ronde, preuve de passage, document ronde de securite : deux pics isoles sur des semaines distinctes, aucune serie exploitable.

Veille concurrentielle (recherche web ce run) : recherche controle qualite prestation gardiennage securite privee Maroc fait remonter un article de presse (Le Matin.ma) mentionnant une intensification des controles de l'inspection du travail en 2024 sur les entreprises de securite - source non autorisee au sens du paragraphe 8.3 (presse, pas une source primaire de la liste), chiffre non repris dans l'article produit. SEKUR / SEKUR Africa : aucun changement de positionnement ou de tarification detecte. Aucun nouvel acteur marocain detecte.

site:optimasprotect.ma reconfirme a 0 resultat pertinent indexe ce run (recherche web).

Alerte outillage ce run : le bac a sable Bash de cette session est reste indisponible toute la duree du run (erreur de montage liee a une mise a jour Windows du 8 septembre, deja annoncee par la plateforme). Contournement applique avec succes.

Point signale avec insistance croissante : le depot compte desormais 14 pull requests ouvertes depuis le 2026-08-22, aucune fusionnee, soit 20 jours sans relecture humaine au 2026-09-11.

## Decision prise ce run (2026-09-09)

0 nouvel article, 0 enrichissement. Rotation testee ce run, priorite pilier 2 : 0 suggestion exploitable sur 16 des 17 requetes, regime pauvre en autocomplete confirme une nouvelle fois.

Deux signaux identifies : rapport incident securite deja couvert par PR 10 (rapport-intervention-ads-maroc), enrichie le 2026-09-06. Gestion de conflit agent de securite exclue par la regle 4.3.2 (tetes de requete emploi/formation).

Aucun sujet pilier 1, 2 ou 3 reellement neuf n'a passe le seuil de 14/25 ce run.

Veille concurrentielle : SEKUR / SEKUR Africa toujours en tarification EUR uniquement pour l'offre France, opacite tarifaire MAD cote Maroc toujours confirmee. Nouveaux acteurs detectes ce run : secumall.ma et kver.ma, revendeurs marocains de controleurs de ronde physiques - materiel, pas logiciel SaaS.

Verification structurelle ce run : la racine de main a ete recontrolee directement et ne contient que le dossier .seo/ - aucun content/blog, aucun generateur, aucun .github/workflows.

Point signale avec insistance croissante : le depot compte toujours 13 pull requests ouvertes depuis le 2026-08-22, aucune fusionnee, soit desormais 18 jours sans relecture humaine.

## Decision prise ce run (2026-09-08)

0 nouvel article, 0 enrichissement. Rotation testee ce run sur des angles non essayes precedemment : 0 suggestion exploitable sur 20 des 21 requetes.

Deux signaux identifies, tous deux deja couverts par des PR existantes : planning agents de securite logiciel (PR 6) et appel d'offre gardiennage Maroc (recoupe PR 8).

Aucun sujet pilier 1, 2 ou 3 reellement neuf n'a passe le seuil de 14/25 ce run.

Veille concurrentielle : SEKUR a publie une nouvelle page comparative datee 2026, sekur.fr/meilleurs-logiciels-securite-privee-2026/. Trackforce Valiant : positionnement international inchange. Aucun nouvel acteur marocain detecte.

Point signale avec insistance croissante : le depot compte toujours 13 pull requests ouvertes depuis le 2026-08-22, aucune fusionnee, apres plus de deux semaines.

## PR ouvertes (en attente de relecture humaine)

- PR 1 controle-de-ronde-nfc-gardiennage-maroc - pilier 1 - hub pilier 1.
- PR 2 prix-logiciel-gardiennage-maroc - pilier 1 - hub prix.
- PR 4 main-courante-electronique-maroc - pilier 2 - cluster 6.
- PR 5 portail-client-securite-privee-maroc - pilier 2.
- PR 6 planning-agents-securite-maroc - pilier 3.
- PR 7 modele-rapport-de-ronde-maroc - pilier 1 - cluster 5.
- PR 8 cahier-des-charges-gardiennage-maroc - pilier 1 - cluster 7, hub conformite. Article reglementaire, reste en PR en permanence.
- PR 9 application-pointage-ads-maroc - pilier 1 - cluster 3.
- PR 10 rapport-intervention-ads-maroc - pilier 2 - cluster 5 (variante). Enrichie le 2026-09-06.
- PR 12 loi-32-26-agents-securite-maroc - pilier 3 - Loi n32.26 (journee de 8h). Score 21/25, article reglementaire, reste en PR en permanence.
- PR 13 obligations-loi-27-06-employeur-maroc - pilier 1 - cluster 8, hub conformite. Score 18/25, article reglementaire, reste en PR en permanence.
- PR 14 faux-pointage-ads-detecter-maroc - pilier 1 - cluster 9. Score 16/25, article non reglementaire.
- PR 15 cahier-de-consignes-securite-maroc - pilier 1 - adjacent au cluster 6 (main courante), intention distincte. Score 17/25, ajoute le 2026-09-05.
- PR 16 controle-qualite-prestation-gardiennage-maroc - pilier 2 - methodologie de controle qualite. Score 17/25, ajoute le 2026-09-11.

14 PR ouvertes depuis le 2026-08-22, soit 21 jours au 2026-09-12, toujours aucune fusionnee sur GitHub a ce jour. Voir toutefois la decouverte du 2026-09-12 (documentee dans .seo/repo-map.md et le rapport du jour) : le contenu de 12 de ces articles est deja en ligne sur le site public malgre l'absence de fusion, via un mecanisme externe non identifie avec precision. Repartition par pilier inchangee : pilier 1 = 8/14 (~57%), pilier 2 = 4/14 (~29%), pilier 3 = 2/14 (~14%), proche de la cible 60/30/10. Prochaine session : continuer a privilegier le pilier 2 si un sujet reellement neuf passe le seuil de 14/25, sinon revenir au pilier 1 conformement a la regle de bascule (paragraphe 0).
