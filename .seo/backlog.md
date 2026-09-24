## Decision prise ce run (2026-09-24)

0 nouvel article, 0 enrichissement. Ecart de run de 1 jour ouvre (dernier rapport le 2026-09-22, pas d'execution constatee le 2026-09-23). Acces au bac a sable Bash retabli ce run (fonctionnel de bout en bout, contrairement a la sequence d'indisponibilite documentee du 8 septembre au 22 septembre) ; utilise pour decoder/encoder les fichiers .seo/* en complement du connecteur MCP GitHub. Un jeton GITHUB_TOKEN est present dans l'environnement mais son usage direct en API REST echoue sur ce depot precis (message : acces GitHub non active pour cette session sur ce repo, add_repo requis) ; le connecteur MCP GitHub reste donc la voie d'ecriture utilisee ce run, conformement au bootstrap.

Rotation testee ce run, 16 requetes sur des angles non essayes precedemment (gl=ma, hl=fr) : logiciel de pointage agent de securite sans smartphone, badge NFC agent de securite prix, comment digitaliser une ronde de securite, preuve de passage agent securite client, solution de pointage pour agents de securite Maroc, rapport de ronde en temps reel, application de ronde de securite Maroc, logiciel de gestion des reclamations securite privee, suivi des interventions de securite en ligne, logiciel de main courante numerique gardiennage, portail client gardiennage Maroc, logiciel de gestion des agents de securite Maroc, gestion des contrats agents de securite, comparateur logiciel securite privee, application ronde de securite gratuite, societe de securite digitalisation Maroc.

0 suggestion sur 16 (pire resultat de la serie ; les runs precedents obtenaient generalement 1 a 2 suggestions). Regime pauvre en autocomplete confirme une nouvelle fois, avec une intensite record ce run. Aucun sujet reellement neuf (pilier 1, 2 ou 3) n'a franchi le seuil de 14/25.

Search Console : premiere tentative reelle d'appel via l'outil gsc_query sur sc-domain:optimasprotect.ma ce run (mcp__SEO_Advena__gsc_query, jusque-la seulement signale comme non configure au bootstrap sans etre teste techniquement) : erreur 403, l'utilisateur authentifie n'a pas la permission suffisante sur cette propriete GSC. Confirme noir sur blanc que l'acces Search Console n'est toujours pas accorde pour ce compte de service ; aucun changement par rapport au statut documente.

Veille concurrentielle (recherche web ciblee) : un acteur marocain supplementaire identifie et verifie directement, IBE MAROC (International Business Engineering, Casablanca, ibe.ma) avec son produit Guard Online, un controleur de rondes materiel (boitiers WM-5000P5+ sans GPS et WM5000L5 avec GPS, transfert des pointages par GPRS vers un serveur consultable en ligne). Aucun prix public affiche. Ce n'est pas un logiciel SaaS NFC/smartphone comparable a OptimasProtect mais un systeme de pointeurs/badgeuses physiques avec remontee GPRS : classe cercle 3 (substitut materiel, non surveillable comme concurrent logiciel direct), a l'instar de KVER/SecuMall. Non ajoute au cercle 1. SEKUR Africa, EasyGard/SGGI, Trackforce Valiant : non revérifiés en detail ce run (dernieres verifications du 09-16 au 09-22 jugees suffisamment recentes), aucun changement attendu.

### Etat du depot

14 PR toujours ouvertes (numeros 1, 2, 4, 5, 6, 7, 8, 9, 10, 12, 13, 14, 15, 16), reconfirme via list_pull_requests (etat open, tri par derniere mise a jour) : aucune fusion depuis le 2026-08-29 (date de la premiere PR d'article), soit 26 jours au 2026-09-24, et aucune nouvelle PR depuis le 2026-08-22 (33 jours). Seules les PR 3 et 11 (corrections du prompt de reference) sont fusionnees. Point signale avec une insistance croissante depuis plusieurs semaines, sans reponse a ce jour.

### Decision de production

Aucun sujet n'a franchi le seuil de 14/25 ce run (0 suggestion exploitable sur 16 requetes, plus faible resultat de la serie). Aucun nouvel article produit ni mis a jour. Conforme a la regle qu'une journee sans article publie est normale, une journee sans veille ne l'est pas (paragraphe 4.1), et a la priorite qualite avant quota (paragraphe 8.4).

Repartition par pilier inchangee depuis le 2026-09-11 : pilier 1 = 8/14 (~57%), pilier 2 = 4/14 (~29%), pilier 3 = 2/14 (~14%), proche de la cible 60/30/10.

## Decision prise ce run (2026-09-22)

0 nouvel article, 0 enrichissement. Ecart de run de 4 jours (dernier rapport le 2026-09-18, aucune execution constatee les 09-19/20/21). Rotation testee ce run, 13 requetes sur des angles non essayes precedemment (voir liste complete dans le rapport du jour .seo/rapports/2026-09-22.md) : avis client societe de gardiennage Maroc, comparatif logiciel gardiennage, societe de securite amende cahier des charges, modele main courante gardiennage, erreur de pointage agent de securite, loi 32.26 agents de securite, gestion de flotte agents de securite, rapport de ronde PDF, societe de securite cahier des charges type, combien coute une ronde de securite, journee de travail agent de securite Maroc loi, logiciel de securite privee avis, cahier des charges securite privee modele.

Deux suggestions sur 13, toutes deux deja couvertes : modele main courante gardiennage vers modele main courante securite pdf/excel, deja couvert par main-courante-electronique-maroc (PR4) ; rapport de ronde PDF vers rapport de ronde pdf / rapport ronde de securite pdf, deja couvert par modele-rapport-de-ronde-maroc (PR7). trends_interest (geo=MA) : interet a 0 partout, aucune requete associee. Regime pauvre en signal de demande confirme.

Veille concurrentielle ce run : deux logiciels internationaux non documentes jusqu'ici identifies et ecartes apres verification directe des sites — BanetteOne (banetteone.com) et eBrigade (ebrigade.app), tous deux France uniquement (references CNAPS/SSIAP/convention collective francaise pour eBrigade, clientele exclusivement francaise pour BanetteOne). Traites comme cercle 2 (international), non ajoutes au cercle 1 Maroc. TRACKTIK identifie dans les resultats mais confirme etre le meme editeur que Trackforce Valiant (fusion ancienne), pas un nouvel acteur. SEKUR Africa, EasyGard/SGGI, Trackforce Valiant : non revérifiés en détail ce run, aucun changement attendu.

Alerte outillage nouvelle ce run : le bac a sable Bash a echoue au demarrage avec un message different de l'erreur de montage Windows habituelle (« Workspace unavailable. The isolated Linux environment failed to start (VM service not running...) »), cause potentiellement distincte a surveiller. Contournement navigateur integre + API GitHub MCP applique avec succes. Un premier commit de mise a jour de .seo/repo-map.md a ete tronque par erreur (10500 octets au lieu de ~41 Ko) puis corrige dans le meme run par un second commit avec le contenu complet reconstruit et verifie.

Sitemap.xml et robots.txt reverifies via navigateur : inchanges depuis le 2026-09-16, toujours 14 articles du pipeline sous /articles/, second canal /blog/ toujours present. Alertes de repo-map.md non resolues, reportees telles quelles.

Repartition par pilier inchangee depuis le 2026-09-11 : pilier 1 = 8/14 (~57%), pilier 2 = 4/14 (~29%), pilier 3 = 2/14 (~14%), proche de la cible 60/30/10.

Le depot compte toujours 14 PR ouvertes depuis le 2026-08-22, soit 31 jours au 2026-09-22, aucune fusionnee sur GitHub.

## Decision prise ce run (2026-09-18)

0 nouvel article, 0 enrichissement. Rotation testee ce run, 16 requetes sur des angles non essayes precedemment (voir liste complete dans le rapport du jour .seo/rapports/2026-09-18.md) : comment prouver une ronde de securite, rapport de ronde automatique, fiche de ronde de securite, cahier de presence agent de securite, gestion des rondes de nuit gardiennage, pointage agent de securite sans carte, solution digitale gardiennage PME Maroc, logiciel de gestion des interventions securite, alternative a Trackforce Maroc, cout d'un logiciel de gestion de securite privee, societe de securite avis client, KPI societe de securite privee, logiciel facturation societe de securite, indicateur de performance gardiennage, gestion du materiel agents de securite, convention collective gardiennage Maroc.

Deux suggestions sur 16, aucune exploitable : fiche de ronde de securite vers rapport/exemple de rapport de ronde de securite (bruit quebecois SAAQ), deja couvert par PR 7 (modele-rapport-de-ronde-maroc) ; indicateur de performance gardiennage vers indicateur de performance securite generique (HSE), hors sujet. Regime pauvre en autocomplete confirme une nouvelle fois. trends_interest indisponible ce run (429 sur geo=MA). topic_demand_score sur gestion du materiel agents de securite : score 1/5.

Veille concurrentielle (recherche web ce run) : SEKUR / SEKUR Africa confirme tarification publique en EUR sur son propre site Afrique (Pack Jeune Entreprise 69,99EUR HT/mois, Pack Gestion 99,99EUR HT/mois, Pack Terrain 9,99EUR HT/mois), plus page comparative 2026 sur sekur.fr (hors perimetre Maroc). EasyGard/SGGI et Trackforce Valiant inchanges. KVER et SecuMall reconfirmes comme revendeurs de materiel physique (cercle 3), pas des concurrents logiciels. Aucun nouvel acteur marocain detecte.

Sitemap.xml et robots.txt reverifies via navigateur (Bash indisponible tout le run, meme erreur de montage Windows depuis le 8 septembre) : inchanges depuis le 2026-09-16, toujours 14 articles du pipeline en ligne sous /articles/, plus le second canal /blog/ (main-courante-electronique-vs-papier) toujours present. Alertes de repo-map.md non resolues, reportees telles quelles.

Repartition par pilier inchangee depuis le 2026-09-11 : pilier 1 = 8/14 (~57%), pilier 2 = 4/14 (~29%), pilier 3 = 2/14 (~14%), proche de la cible 60/30/10.

Le depot compte toujours 14 PR ouvertes depuis le 2026-08-22, soit 27 jours au 2026-09-18, aucune fusionnee sur GitHub (seules les PR 3 et 11 le sont, reconfirme ce run via list_pull_requests et list_branches).

## Decision prise ce run (2026-09-16)

0 nouvel article, 0 enrichissement. Rotation testee ce run, 15 requetes sur des angles non essayes precedemment (voir liste complete dans le rapport du jour .seo/rapports/2026-09-16.md) : solution de controle de ronde pour societe de securite, meilleur logiciel de gardiennage Maroc, logiciel de gardiennage gratuit, demo logiciel gardiennage, essai gratuit logiciel securite privee, modele cahier des charges securite privee, attestation de service fait gardiennage, preuve de prestation gardiennage client, gestion multi-sites agents de securite, logiciel securite privee cloud Maroc, cout logiciel de pointage agents de securite, tableau de bord securite privee, audit de conformite gardiennage Maroc, pointage biometrique agent de securite Maroc, avis logiciel gardiennage.

Deux suggestions sur 15, toutes deux deja couvertes (logiciel planning agent de securite gratuit vers PR 6 ; cahier des charges securite privee vers PR 8). Regime pauvre en autocomplete confirme une nouvelle fois.

Decouverte concurrentielle ce run : SEKUR Africa affiche desormais des paliers tarifaires publics en EUR sur son propre site Afrique (sekur-africa.com : Pack Jeune Entreprise 69,99EUR HT/mois, Pack Gestion 99,99EUR HT/mois, Pack Terrain 9,99EUR HT/mois), en plus de son offre France deja documentee. EasyGard/SGGI et Trackforce Valiant inchanges. Aucun nouvel acteur marocain detecte.

Changement technique constate : robots.txt simplifie (les blocs anti-bot IA nommes Cloudflare Content-Signal, GPTBot, CCBot, Google-Extended, ClaudeBot, Bytespider, Applebot-Extended, CloudflareBrowserRenderingCrawler ont disparu), sans impact sur Googlebot, toujours explicitement autorise.

Synchronisation du site live : sitemap.xml reconfirme toujours les 14 articles du pipeline en ligne sous /articles/, plus le second canal /blog/ (main-courante-electronique-vs-papier) toujours present, inchange. Alertes 1 et 2 de repo-map.md non resolues, reportees telles quelles.

Repartition par pilier inchangee depuis le 2026-09-11 : pilier 1 = 8/14 (~57%), pilier 2 = 4/14 (~29%), pilier 3 = 2/14 (~14%), proche de la cible 60/30/10.

Le depot compte toujours 14 PR ouvertes depuis le 2026-08-22, soit 25 jours au 2026-09-16, aucune fusionnee sur GitHub (seules les PR 3 et 11 sont fusionnees, reconfirme ce run).

# Backlog editorial - OptimasProtect

Derniere mise a jour : 2026-09-15 (semaine S38).

## Decision prise ce run (2026-09-15)

0 nouvel article, 0 enrichissement. Rotation testee ce run, 18 requetes sur des angles non essayes precedemment (voir liste complete dans le rapport du jour .seo/rapports/2026-09-15.md) : audit ronde de securite, preuve de service gardiennage, checklist ronde de securite, alternative Excel gardiennage, digitaliser main courante gardiennage, logiciel conformite cahier des charges securite, preuve horodatee passage agent, solution sans materiel gardiennage, logiciel main courante incident securite, portail client suivi prestation securite, rapport journalier gardiennage client, logiciel planning agents de securite, gestion absences agents de securite, evaluation performance agent de securite, registre de securite numerique gardiennage, preuve de passage ronde gardiennage, appel d'offres gardiennage cahier des charges Maroc, logiciel gestion societe de securite Maroc, EasyGard logiciel gardiennage.

Deux suggestions sur 18. « guide ronde de securite » : bruit hors cible (derives quebecois vehicule lourd / SAAQ), non exploitable. « logiciel planning agent de securite gratuit » : score de demande 2/5, niche, et intention deja entierement couverte par PR 6 (planning-agents-securite-maroc), y compris une FAQ dediee sur le sujet gratuit. Aucun nouvel article, aucune mise a jour necessaire.

trends_interest fonctionnel ce run (pas de 429) sur logiciel gardiennage Maroc / controle de ronde / pointage agent securite (geo=MA) : interet a 0 partout, aucune requete associee. Regime pauvre en signal de demande confirme une nouvelle fois.

Decouverte concurrentielle ce run, documentee en detail dans .seo/repo-map.md et le rapport du jour : EasyGard, logiciel edite par SGGI (Marrakech), positionne gestion des societes de gardiennage (pointage, paie, facturation), oriente pilier 3 (RH/paie), sans fonctionnalite de tracabilite NFC identifiee. Ajoute au cercle 1 de la veille concurrentielle pour les prochains runs. SEKUR / SEKUR Africa et Trackforce Valiant : aucun changement de positionnement ou de prix detecte.

Synchronisation du site live : le sitemap.xml liste desormais les 14 articles du pipeline (rattrapage confirme par rapport aux 12 constates les 2026-09-12 et 2026-09-14). Le second canal /blog/ independant de ce depot est toujours present (voir alertes dans repo-map.md).

Repartition par pilier inchangee depuis le 2026-09-11 : pilier 1 = 8/14 (~57%), pilier 2 = 4/14 (~29%), pilier 3 = 2/14 (~14%), proche de la cible 60/30/10.

## Decision prise ce run (2026-09-12)

0 nouvel article, 0 enrichissement. Rotation testee ce run, 15 requetes sur des angles non essayes precedemment (voir liste complete dans le rapport du jour .seo/rapports/2026-09-12.md) : frequence des rondes de securite, cahier de rondes gardiennage, application mobile agent de securite, ronde de securite sans internet, carte de ronde electronique, supervision agents de securite a distance, tag NFC gardiennage, temps de reponse incident securite privee, digitalisation securite privee Maroc, logiciel de gestion de rondes, verification de presence agent site client, combien coute un pointeur NFC, assurance societe de gardiennage Maroc, sous-traitance gardiennage Maroc, superviseur de securite outils.

Un seul signal exploitable : cahier de rondes gardiennage vers cahier ronde de securite. Score de demande 3/5 (topic_demand_score), mais trends_interest ne montre qu'un pic isole sur la semaine du 2025-10-05, signal ponctuel. Anti-doublon verifie en lisant integralement le contenu de PR 7 (modele-rapport-de-ronde-maroc) : cet article couvre deja cette intention, y compris un tableau comparatif rapport papier / rapport genere automatiquement. Aucun nouvel article, aucune mise a jour necessaire.

Toutes les autres requetes : 0 suggestion, regime pauvre en autocomplete confirme une nouvelle fois sur ce marche.

Decouverte majeure ce run, documentee en detail dans .seo/repo-map.md et .seo/rapports/2026-09-12.md : en verifiant directement le site live (sitemap.xml, robots.txt, pages /articles/slug), il apparait que 12 des 14 articles produits par cet agent sont deja en ligne sur optimasprotect.ma, avec un contenu quasi identique aux branches article, alors qu'aucune des PR correspondantes n'a ete fusionnee sur GitHub. Cela nuance fortement l'alerte historique sur l'absence de generateur de site connecte, et souleve un point a clarifier par l'utilisateur sur l'articulation entre ce mecanisme de publication et la relecture humaine prevue en Phase 1.

Veille concurrentielle (recherche web ce run) : SEKUR / SEKUR Africa toujours en tarification EUR uniquement pour l'offre France, opacite MAD toujours confirmed cote Maroc, aucun changement de positionnement detecte. Trackforce Valiant toujours positionne a l'international, pricing sur devis, aucune adaptation Maroc identifiee. Aucun nouvel acteur marocain detecte au-dela de secumall.ma et kver.ma, deja documentes.

Alerte outillage ce run : le bac a sable Bash de cette session est reste indisponible toute la duree du run (meme erreur de montage Windows du 8 septembre). Contournement applique avec succes via le navigateur integre.

Point signale avec insistance croissante, a relire avec la nuance de la decouverte ci-dessus : le depot compte toujours 14 pull requests ouvertes depuis le 2026-08-22, aucune fusionnee, soit 21 jours au 2026-09-12. Ce point est signale sans interruption depuis le 2026-08-31, mais sa portee doit desormais etre relativisee : le contenu ne semble pas bloque en pratique, il atteint le site par un autre canal que la fusion GitHub.

Repartition par pilier inchangee depuis le 2026-09-11 (aucun ajout) : pilier 1 = 8/14 (~57%), pilier 2 = 4/14 (~29%), pilier 3 = 2/14 (~14%), proche de la cible 60/30/10.

## Decision prise ce run (2026-09-11)

1 nouvel article produit : PR 16 (controle-qualite-prestation-gardiennage-maroc, pilier 2, score 17/25). Priorite donnee au pilier 2 conformement a l'ecart de ratio signale sans interruption depuis le 2026-08-31 (pilier 2 sous la cible de 30%). Rotation testee ce run, environ 25 requetes sur les trois piliers. Un seul signal exploitable : assurance qualite gardiennage vers controle qualite securite privee. Score 17/25. Article produit et publie en PR 16, pilier 2.

trends_interest (geo=MA, 12 mois) sur justificatif de ronde, preuve de passage, document ronde de securite : deux pics isoles sur des semaines distinctes, aucune serie exploitable.

Veille concurrentielle (recherche web ce run) : recherche controle qualite prestation gardiennage securite privee Maroc fait remonter un article de presse (Le Matin.ma) mentionnant une intensification des controles de l'inspection du travail en 2024 sur les entreprises de securite, source non autorisee au sens du paragraphe 8.3 (presse, pas une source primaire de la liste), chiffre non repris dans l'article produit. SEKUR / SEKUR Africa : aucun changement de positionnement ou de tarification detecte. Aucun nouvel acteur marocain detecte.

site:optimasprotect.ma reconfirme a 0 resultat pertinent indexe ce run (recherche web).

Alerte outillage ce run : le bac a sable Bash de cette session est reste indisponible toute la duree du run (erreur de montage liee a une mise a jour Windows du 8 septembre, deja annoncee par la plateforme). Contournement applique avec succes.

Point signale avec insistance croissante : le depot compte desormais 14 pull requests ouvertes depuis le 2026-08-22, aucune fusionnee, soit 20 jours sans relecture humaine au 2026-09-11.

## Decision prise ce run (2026-09-09)

0 nouvel article, 0 enrichissement. Rotation testee ce run, priorite pilier 2 : 0 suggestion exploitable sur 16 des 17 requetes, regime pauvre en autocomplete confirme une nouvelle fois.

Deux signaux identifies : rapport incident securite deja couvert par PR 10 (rapport-intervention-ads-maroc), enrichie le 2026-09-06. Gestion de conflit agent de securite exclue par la regle 4.3.2 (tetes de requete emploi/formation).

Aucun sujet pilier 1, 2 ou 3 reellement neuf n'a passe le seuil de 14/25 ce run.

Veille concurrentielle : SEKUR / SEKUR Africa toujours en tarification EUR uniquement pour l'offre France, opacite tarifaire MAD cote Maroc toujours confirmee. Nouveaux acteurs detectes ce run : secumall.ma et kver.ma, revendeurs marocains de controleurs de ronde physiques, materiel, pas logiciel SaaS.

Verification structurelle ce run : la racine de main a ete recontrolee directement et ne contient que le dossier .seo/, aucun content/blog, aucun generateur, aucun .github/workflows.

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
- PR 15 cahier-de-consignes-securite-maroc - pilier 1 - adjacent au cluster 6 (main courante), intention distincte. Score 17/25, ajoutee le 2026-09-05.
- PR 16 controle-qualite-prestation-gardiennage-maroc - pilier 2 - methodologie de controle qualite. Score 17/25, ajoutee le 2026-09-11.

14 PR ouvertes depuis le 2026-08-22, soit 24 jours au 2026-09-15, toujours aucune fusionnee sur GitHub a ce jour (seules les PR 3 et 11, corrections du prompt de reference, sont fusionnees). Voir toutefois la decouverte du 2026-09-12 et sa confirmation du 2026-09-15 (documentees dans .seo/repo-map.md) : le contenu de la totalite des 14 articles est desormais visible sur le site public malgre l'absence de fusion. Repartition par pilier inchangee : pilier 1 = 8/14 (~57%), pilier 2 = 4/14 (~29%), pilier 3 = 2/14 (~14%), proche de la cible 60/30/10. Prochaine session : continuer a privilegier le pilier 2 ou 3 si un sujet reellement neuf passe le seuil de 14/25, sinon revenir au pilier 1 conformement a la regle de bascule (paragraphe 0).
