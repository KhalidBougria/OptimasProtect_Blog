# Backlog editorial - OptimasProtect

Ce fichier est un document de travail vivant, volontairement condense a partir du 2026-09-30 (l'historique detaille jour par jour precedent restait disponible in extenso dans .seo/rapports/{AAAA-MM-JJ}.md ; les entrees plus anciennes que celle du jour ne sont plus dupliquees ici pour garder ce fichier court, conformement a la consigne de condenser un fichier qui devient long).

## Decision prise ce run (2026-10-01)

0 nouvel article, 0 enrichissement. Aucun ecart de run (dernier rapport le 2026-09-30, cadence normale). Acces au depot verifie et fonctionnel via le connecteur MCP GitHub (mcp__remote-devices__GitHub_MCP_Server__JS___*), Bash fonctionnel de bout en bout ce run.

Rotation testee ce run, 16 requetes sur des angles non essayes precedemment (gl=ma, hl=fr) : comment prouver une ronde de securite, systeme de pointage pour vigiles, bon de ronde electronique, logiciel de supervision agents de securite, comment gerer les reclamations clients securite privee, modele de registre de securite gardiennage, logiciel de gestion de securite SaaS Maroc, comment automatiser le pointage des agents, application de controle de presence vigile, digitalisation gardiennage Maroc avis, logiciel de preuve de prestation gardiennage, contester une facture de gardiennage, logiciel de securite privee pas cher Maroc, cahier de rondes obligatoire Maroc, transformation digitale societe de securite, logiciel de pointage vigile sans carte.

0 suggestion sur 16, cinquieme run consecutif a 0 suggestion exploitable (0/16 le 09-24, 0/16 le 09-25, 0/15 le 09-29, 0/16 le 09-30, 0/16 aujourd'hui). trends_interest (geo=MA, 12 mois) sur logiciel de securite SaaS Maroc / transformation digitale societe de securite / bon de ronde electronique : interet a 0 sur la quasi-totalite de la periode, deux pics isoles d'une semaine sans requete associee (bruit, pas un signal). Aucun sujet reellement neuf n'a franchi le seuil de 14/25.

Veille concurrentielle (recherche web ciblee) : aucun nouvel acteur logiciel marocain identifie, uniquement des acteurs deja documentes (SEKUR Africa, KVER, SecuMall, IBE Maroc, Securimag, tous deja classes). Recherche sur la marque elle-meme : aucun resultat pertinent hors le depot GitHub.

Verification technique du site live (WearFetch) : robots.txt et sitemap.xml inchanges, toujours 14 articles du pipeline sous /articles/, second canal /blog/main-courante-electronique-vs-papier toujours present.

### Correction de calendrier (important)

Les points des 2026-09-22 au 2026-09-30 affirmaient a tort "aucune nouvelle PR depuis le 2026-08-22, soit 33/39 jours". Verification directe des dates de creation via list_pull_requests ce run : les PR 12 a 16 ont bien ete creees entre le 2026-08-30 et le 2026-09-11. La derniere PR d'article creee (PR 16) date donc du 2026-09-11, soit 20 jours au 2026-10-01 - pas 39. Le constat qui reste exact, et qui est le vrai point d'alerte, est different : aucune des 14 PR d'articles n'a jamais ete fusionnee depuis la premiere (2026-08-22), soit 40 jours sans relecture humaine. Seules les PR 3 et 11 (corrections du prompt de reference, pas des articles) sont fusionnees, les 2026-08-22 et 2026-08-29.

### Etat du depot

14 PR toujours ouvertes (numeros 1, 2, 4, 5, 6, 7, 8, 9, 10, 12, 13, 14, 15, 16), reconfirme via list_branches et list_pull_requests. Seules PR 3 et 11 fusionnees. Aucune fusion depuis le 2026-08-29, soit 40 jours au 2026-10-01 (voir correction de calendrier ci-dessus pour la date exacte de la derniere PR creee). Point signale en alerte haute, sans reponse a ce jour, desormais plus d'un mois sans relecture humaine.

### Decision de production

Aucun sujet n'a franchi le seuil de 14/25 ce run. Aucun nouvel article produit ni mis a jour. Conforme a la regle qu'une journee sans article publie est normale, une journee sans veille ne l'est pas (paragraphe 4.1), et a la priorite qualite avant quota (paragraphe 8.4).

Repartition par pilier inchangee depuis le 2026-09-11 : pilier 1 = 8/14 (~57%), pilier 2 = 4/14 (~29%), pilier 3 = 2/14 (~14%), proche de la cible 60/30/10.

## PR ouvertes (en attente de relecture humaine), etat au 2026-10-01

- PR 1 controle-de-ronde-nfc-gardiennage-maroc - pilier 1 - hub pilier 1.
- PR 2 prix-logiciel-gardiennage-maroc - pilier 1 - hub prix.
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

Note sur les runs du 2026-09-25 et du 2026-09-29 : rapports quotidiens existants (.seo/rapports/2026-09-25.md et .seo/rapports/2026-09-29.md) mais non reportes individuellement ici avant condensation ; sans consequence sur le fond puisque l'historique complet reste disponible dans .seo/rapports/.

Pour l'historique detaille des runs anterieurs au 2026-09-30 (veille mots-cles jour par jour, decouvertes concurrentielles, alertes outillage), voir les rapports quotidiens dans .seo/rapports/ et .seo/repo-map.md, qui conservent la chronologie complete.
