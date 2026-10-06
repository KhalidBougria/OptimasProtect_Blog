# Backlog editorial - OptimasProtect

Ce fichier est un document de travail vivant, volontairement condense a partir du 2026-09-30 (l'historique detaille jour par jour precedent restait disponible in extenso dans .seo/rapports/{AAAA-MM-JJ}.md ; les entrees plus anciennes que celle du jour ne sont plus dupliquees ici pour garder ce fichier court, conformement a la consigne de condenser un fichier qui devient long).

## Decision prise ce run (2026-10-06)

0 nouvel article, 0 enrichissement. Acces au depot verifie et fonctionnel via le connecteur MCP GitHub (mcp__remote-devices__GitHub_MCP_Server__JS___*). GH_TOKEN/GITHUB_TOKEN presents mais explicitement non autorises par la politique de la session pour ce depot, non utilises.

Rotation testee ce run, 15 requetes sur des angles non essayes precedemment (gl=ma, hl=fr) : logiciel tracabilite gardiennage Maroc, preuve de ronde gardiennage, logiciel securite privee devis Maroc, application gardiennage sans materiel Maroc, main courante gardiennage obligatoire, logiciel vigile Maroc, logiciel conformite Loi 27-06 Maroc, suivi des agents de securite en temps reel, logiciel de rondes gardiennage essai gratuit Maroc, gestion incident securite privee application, reponse appel d'offres gardiennage tracabilite, badge NFC agent de securite Maroc, outil de pilotage agents de securite Maroc, preuve de service gardiennage client, digitalisation societe de securite Maroc 2026.

1 suggestion sur 15 (« preuve de ronde gardiennage » vers « document ronde de securite »), deja couverte par les articles existants (modele-rapport-de-ronde-maroc PR7, rapport-intervention-ads-maroc PR10). gsc_query reteste directement ce run sur sc-domain:optimasprotect.ma (06-09 au 04-10-2026, country=mar) : 403 confirme a nouveau (« User does not have sufficient permission »). Aucun sujet reellement neuf n'a franchi le seuil de 14/25 ce run.

**DECOUVERTE MAJEURE CE RUN, ALERTE HAUTE NOUVELLE : le site live (optimasprotect.ma/ et /tarifs) et la page /articles/prix-logiciel-gardiennage-maroc affichent desormais un modele "Sur devis" exclusif, sans aucun prix public en MAD.** Verifie directement par WebFetch sur les deux pages. Le brouillon Git de la PR 2 (branche article/prix-logiciel-gardiennage-maroc) contient lui toujours les anciens prix fixes (99 MAD HT, 179 MAD HT, tableau cout journalier, JSON-LD Offer price 99/179 MAD) : contradiction directe avec le site live sur cette meme URL. Le §0 et le §2.2 du prompt de reference (.seo/agent-prompt.md) reposent sur ce fait desormais perime. Element de contexte externe a ce depot (hors perimetre verifiable par cet agent) suggere qu'il s'agirait d'une decision explicite de l'utilisateur prise en octobre 2026 de retirer les tarifs publics. N'ayant recu aucune instruction directe de corriger le prompt de reference sur ce point precis ce run, cet agent n'a PAS modifie .seo/agent-prompt.md ni le contenu de la PR 2 de sa propre initiative (a la difference des corrections du 08-22 et du 08-29, faites apres confirmation directe de l'utilisateur). Voir le detail complet dans .seo/repo-map.md (point du 2026-10-06) et dans le rapport du jour. Recommandation : (1) confirmer si ce changement de modele tarifaire est definitif, (2) si oui, corriger §0/§2.2 du prompt de reference par PR dediee (meme mecanisme que les corrections precedentes) et reprendre la PR 2 (et tout autre contenu pilier 1 citant 99/179 MAD) avant toute fusion, (3) en attendant, suspendre toute nouvelle production d'article citant un prix fixe.

Veille concurrentielle non reverifiee en detail ce run (dernieres verifications jugees suffisamment recentes, voir .seo/repo-map.md). Sitemap.xml et robots.txt non reverifies ce run specifiquement (vus en detail lors de runs recents).

### Etat du depot

14 PR toujours ouvertes (numeros 1, 2, 4, 5, 6, 7, 8, 9, 10, 12, 13, 14, 15, 16), reconfirme via list_pull_requests (etat open, 14 resultats). Seules PR 3 et 11 fusionnees. Aucune fusion depuis le 2026-08-29, soit 38 jours au 2026-10-06. Aucune nouvelle PR d'article depuis le 2026-09-11 (PR 16), soit 25 jours. Alerte haute reconduite depuis plusieurs semaines sans reponse, desormais cumulee avec la decouverte tarifaire ci-dessus.

### Decision de production

Aucun sujet n'a franchi le seuil de 14/25 ce run. Aucun nouvel article produit ni mis a jour. Conforme a la regle qu'une journee sans article publie est normale, une journee sans veille ne l'est pas (paragraphe 4.1), et a la priorite qualite avant quota (paragraphe 8.4) — renforcee ce run par la prudence tarifaire ci-dessus.

Repartition par pilier inchangee depuis le 2026-09-11 : pilier 1 = 8/14 (~57%), pilier 2 = 4/14 (~29%), pilier 3 = 2/14 (~14%), proche de la cible 60/30/10.

## PR ouvertes (en attente de relecture humaine), etat au 2026-10-06

- PR 1 controle-de-ronde-nfc-gardiennage-maroc - pilier 1 - hub pilier 1.
- PR 2 prix-logiciel-gardiennage-maroc - pilier 1 - hub prix. **A reprendre avant fusion : contient des prix fixes (99/179 MAD) desormais en contradiction avec le site live "sur devis", voir alerte ci-dessus.**
- PR 4 main-courante-electronique-maroc - pilier 2 - cluster 6.
- PR 5 portail-client-securite-privee-maroc - pilier 2.
- PR 6 planning-agents-securite-maroc - pilier 3.
- PR 7 modele-rapport-de-ronde-maroc - pilier 1 - cluster 5.
- PR 8 cahier-des-charges-gardiennage-maroc - pilier 1 - cluster 7, hub conformite. Article reglementaire, reste en PR en permanence.
- PR 9 application-pointage-ads-maroc - pilier 1 - cluster 3.
- PR 10 rapport-intervention-ads-maroc - pilier 2 - cluster 5 (variante).
- PR 12 loi-32-26-agents-securite-maroc - pilier 3 - Loi n32.26 (journee de 8h). Article reglementaire, reste en PR en permanence.
- PR 13 obligations-loi-27-06-employeur-maroc - pilier 1 - cluster 8, hub conformite. Article reglementaire, reste en PR en permanence.
- PR 14 faux-pointage-ads-detecter-maroc - pilier 1 - cluster 9.
- PR 15 cahier-de-consignes-securite-maroc - pilier 1 - adjacent au cluster 6 (main courante), intention distincte.
- PR 16 controle-qualite-prestation-gardiennage-maroc - pilier 2 - methodologie de controle qualite.

Pour l'historique detaille des runs anterieurs au 2026-09-30 (veille mots-cles jour par jour, decouvertes concurrentielles, alertes outillage), voir les rapports quotidiens dans .seo/rapports/ et .seo/repo-map.md, qui conservent la chronologie complete.
