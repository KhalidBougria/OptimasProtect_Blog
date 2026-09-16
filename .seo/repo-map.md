## Point du 2026-09-16 : aucun nouvel article, robots.txt simplifié (blocs anti-bot IA disparus), pas de nouveau concurrent majeur

Accès dépôt reconfirmé : authentifié KhalidBougria (propriétaire du compte, pas obougria), permissions push:true / admin:true inchangées, connecteur MCP GitHub local (local_unpacked_qunfei-wu_github-mcp-server-js). Bash indisponible tout le run, même erreur de montage Windows que depuis le 8 septembre ; contournement navigateur intégré à nouveau utilisé avec succès pour lire sitemap.xml, robots.txt et pour fetch/encoder les mises a jour committees (fetch + btoa via javascript_tool, en l'absence de Bash).

Prompt de référence relu intégralement depuis .seo/agent-prompt.md (version 3.2) : à jour, aucune divergence. Note pour mémoire : le texte reproduit dans le corps de la tâche planifiée elle-même diverge encore sur trois points déjà corrigés côté dépôt (Loi n°35-09 au lieu de 27-06, structure /blog/ au lieu de /articles/, "Optimas Protect" en deux mots au lieu d'un seul) ; conformément aux instructions de bootstrap, c'est la version du dépôt qui prime, appliquée intégralement ce run.

### Sitemap et robots.txt

Sitemap.xml reconfirmé : toujours les 14 articles du pipeline en ligne sous /articles/, plus le second canal /blog/main-courante-electronique-vs-papier toujours présent, inchangé.

Changement constaté sur robots.txt : le fichier est désormais réduit à deux lignes (User-agent: * / Allow: /) plus la directive Sitemap. Les blocs Cloudflare Content-Signal (search=yes / ai-train=no) et les Disallow ciblant les crawlers d'entraînement IA nommés (GPTBot, CCBot, Google-Extended, ClaudeBot, Bytespider, Applebot-Extended, CloudflareBrowserRenderingCrawler) documentés lors des vérifications précédentes ont disparu. Sans impact sur l'indexation : Googlebot reste explicitement autorisé (Allow: /) comme avant. A signaler comme changement factuel de configuration côté site, hors périmètre d'action de cet agent.

### Veille mots-clés et SERP

Marché ciblé : Maroc (gl=ma, hl=fr). Rotation de 15 requêtes sur des angles non testés lors des runs précédents (voir cumul dans les rapports du 08 au 15 septembre) : solution de contrôle de ronde pour société de sécurité, meilleur logiciel de gardiennage Maroc, logiciel de gardiennage gratuit, démo logiciel gardiennage, essai gratuit logiciel sécurité privée, modèle cahier des charges sécurité privée, attestation de service fait gardiennage, preuve de prestation gardiennage client, gestion multi-sites agents de sécurité, logiciel sécurité privée cloud Maroc, coût logiciel de pointage agents de sécurité, tableau de bord sécurité privée, audit de conformité gardiennage Maroc, pointage biométrique agent de sécurité Maroc, avis logiciel gardiennage.

Deux suggestions obtenues sur 15, toutes deux déjà couvertes : « logiciel de gardiennage gratuit » renvoie « logiciel planning agent de sécurité gratuit », intention déjà entièrement traitée par la branche planning-agents-securite-maroc (PR 6, FAQ dédiée). « Modèle cahier des charges sécurité privée » renvoie « cahier des charges sécurité privée », combinaison déjà couverte par cahier-des-charges-gardiennage-maroc (PR 8, hub conformité) ; à noter que « cahier des charges » seul en tête sèche reste une tête de requête à ne pas attaquer frontalement (règle 4.3.7). Régime pauvre en autocomplete confirmé une nouvelle fois sur ce marché, conforme au constat répété depuis plusieurs semaines.

Aucun sujet réellement neuf (pilier 1, 2 ou 3) n'a passé le seuil de production de 14/25 ce run.

### Veille concurrentielle

SEKUR / SEKUR Africa : recherche web ce run sur sekur-africa.com montre des paliers tarifaires publics en EUR (Pack Jeune Entreprise 69,99€ HT/mois, Pack Gestion 99,99€ HT/mois, Pack Terrain 9,99€ HT/mois) affichés directement sur le site Afrique, et non plus seulement sur l'offre France (sekur.fr) comme documenté précédemment. Renforce encore le différenciateur prix en MAD d'Optimas Protect : même le site à vocation africaine du concurrent direct facture en euros, aucune opacité MAD levée côté Maroc.

EasyGard / SGGI (Marrakech) : reconfirmé positionné gestion RH/paie des agents (pointage, primes, calcul de paie, facturation client), toujours aucune fonctionnalité de traçabilité NFC ou de preuve de passage identifiée, toujours aucun prix public trouvé. Aucun changement de positionnement depuis sa découverte le 2026-09-15.

Trackforce Valiant : toujours positionné à l'international, pricing sur devis, aucune adaptation Maroc identifiée. Aucun nouvel acteur marocain détecté au-delà de ceux déjà documentés (SEKUR Africa, EasyGard/SGGI, secumall.ma, kver.ma).

### Décision de production

Aucun nouvel article produit ni mis à jour ce run. Les 10 clusters prioritaires du paragraphe 4.2 restent tous couverts par au moins un article en PR, la rotation de mots-clés n'a fait remonter aucun signal de demande exploitable non déjà couvert, et le seuil de 14/25 n'a été franchi par aucun sujet neuf. Conforme à la règle qu'une journée sans article publié est normale, une journée sans veille ne l'est pas (paragraphe 4.1), et à la priorité qualité avant quota (paragraphe 8.4).

Répartition par pilier inchangée depuis le 2026-09-11 : pilier 1 = 8/14 (~57%), pilier 2 = 4/14 (~29%), pilier 3 = 2/14 (~14%), proche de la cible 60/30/10.

Le dépôt compte toujours 14 PR d'articles ouvertes depuis le 2026-08-22, soit 25 jours au 2026-09-16, aucune fusionnée sur GitHub (seules les PR 3 et 11, corrections du prompt de référence, sont fusionnées — reconfirmé ce run via list_pull_requests état closed). Voir toutefois les points des 2026-09-12 et 2026-09-15 : le contenu de la totalité des 14 articles est visible sur le site public malgré l'absence de fusion, via un mécanisme non identifié avec précision.

# Cartographie du depot - OptimasProtect_Blog

Derniere mise a jour : 2026-09-15 (semaine S38). Ce fichier est un document de travail vivant ; pour l'historique detaille jour par jour, voir .seo/rapports/.

## Point du 2026-09-15 : synchronisation du site rattrapee (14/14 articles du pipeline en ligne), nouveau concurrent marocain identifie (EasyGard/SGGI), aucun nouvel article

Acces depot reconfirme : authentifie KhalidBougria (proprietaire du compte, pas obougria), permissions push:true / admin:true inchangees, connecteur MCP GitHub local (local_unpacked_qunfei-wu_github-mcp-server-js). Bash indisponible tout le run, meme erreur de montage Windows que depuis le 8 septembre (reconfirmee explicitement ce run) ; contournement navigateur integre a nouveau utilise avec succes pour lire .seo/*, sitemap.xml, robots.txt, et pour encoder en base64 les mises a jour committees (btoa/encodeURIComponent via javascript_tool, en l'absence de Bash).

Prompt de reference relu integralement depuis .seo/agent-prompt.md (version 3.2) : a jour, aucune divergence.

Anti-doublon : repartition par pilier des 14 branches article/* reconfirmee (pas de relecture individuelle supplementaire ce run au-dela de la branche planning-agents-securite-maroc, voir plus bas), inchangee depuis le 2026-09-11 : pilier 1 = 8/14 (~57%), pilier 2 = 4/14 (~29%), pilier 3 = 2/14 (~14%), proche de la cible 60/30/10.

### Synchronisation du site live : rattrapage confirme

Le sitemap.xml live liste desormais les 14 articles produits par ce pipeline (contre 12 le 2026-09-12 et le 2026-09-14) : cahier-de-consignes-securite-maroc et controle-qualite-prestation-gardiennage-maroc, absents depuis plusieurs jours, sont maintenant en ligne sous /articles/. Le decalage de synchronisation documente depuis le 2026-09-12 s'est donc resorbe. Le mecanisme de publication reel reste non identifie avec precision (aucune PR d'article fusionnee sur GitHub, seules les PR 3 et 11 le sont), mais la conclusion factuelle est desormais que l'ensemble du contenu produit par ce pipeline est visible sur le site public.

Le second canal /blog/ independant de ce depot (voir Point du 2026-09-14) est toujours present et actif : /blog/main-courante-electronique-vs-papier reste dans le sitemap, inchange. Le risque de cannibalisation SEO sur le cluster main courante electronique reste entier et non resolu.

robots.txt reverifie ce run (navigateur) : inchange sur le fond, User-agent * Allow /, Content-Signal search=yes / ai-train=no. Deux entrees supplementaires apparaissent dans le bloc Cloudflare Managed Content depuis la derniere verification (Applebot-Extended, CloudflareBrowserRenderingCrawler, toutes deux Disallow), sans impact : Googlebot reste non restreint. Alerte anti-bot toujours levee.

### Veille mots-cles et SERP

Marche cible : Maroc (gl=ma, hl=fr ; Trends geo=MA). Rotation de 18 requetes sur des angles non testes lors des runs precedents : audit ronde de securite, preuve de service gardiennage, checklist ronde de securite, alternative Excel gardiennage, digitaliser main courante gardiennage, logiciel conformite cahier des charges securite, preuve horodatee passage agent, solution sans materiel gardiennage, logiciel main courante incident securite, portail client suivi prestation securite, rapport journalier gardiennage client, logiciel planning agents de securite, gestion absences agents de securite, evaluation performance agent de securite, registre de securite numerique gardiennage, preuve de passage ronde gardiennage, appel d'offres gardiennage cahier des charges Maroc, logiciel gestion societe de securite Maroc, EasyGard logiciel gardiennage.

Deux suggestions obtenues sur 18 : « guide ronde de securite » (derives vehicule lourd / SAAQ, contexte quebecois hors cible, bruit non exploitable) et « logiciel planning agent de securite gratuit » (score de demande 2/5 via topic_demand_score, niche). Anti-doublon verifie par lecture integrale de la branche planning-agents-securite-maroc (PR 6) : cette intention est deja entierement couverte, y compris une question FAQ dediee (« Un logiciel de planning gratuit suffit-il pour une petite societe de securite ? »). Aucune mise a jour necessaire.

trends_interest fonctionnel ce run (pas d'erreur 429, contrairement au 2026-09-14) sur logiciel gardiennage Maroc / controle de ronde / pointage agent securite (geo=MA, 12 mois) : interet a 0 sur toutes les regions marocaines disponibles dans l'outil, aucune requete associee (top ou en hausse). Confirme une nouvelle fois le regime pauvre en signal de demande mesurable sur ce marche.

Aucun sujet reellement neuf (pilier 1, 2 ou 3) n'a passe le seuil de production de 14/25 ce run.

### Veille concurrentielle

SEKUR / SEKUR Africa (cercle 1, Maroc) : toujours en opacite tarifaire MAD cote Maroc, tarification EUR uniquement pour l'offre France, aucun changement de positionnement detecte.

Trackforce Valiant (cercle 2, international) : toujours positionne a l'international, pricing sur devis, aucune adaptation Maroc identifiee.

Decouverte nouvelle ce run : EasyGard, logiciel edite par SGGI (Marrakech, sggi-maroc.com), positionne "gestion des societes de gardiennage" : pointage par agent et par site, gestion des primes/avances/sanctions, calcul de paie brut/net et bulletins de paie, facturation client. Trois modes de deploiement proposes (poste local, reseau local, cloud). Aucun prix public trouve dans les pages consultees. Ce concurrent est nettement plus oriente pilier 3 (RH et paie des agents) que pilier 1 (tracabilite NFC/preuve de passage) : aucune fonctionnalite de controle de ronde ou de preuve de passage identifiee. A ajouter au cercle 1 (Maroc) de la veille concurrentielle pour les prochains runs, a surveiller notamment si une offre tarifaire publique apparait.

Verification distincte : marocgard.com (Maroc Gard) est une societe de gardiennage potentiellement cliente, pas un editeur logiciel concurrent. Aucune action.

### Decision de production

Aucun nouvel article produit ni mis a jour ce run. Les 10 clusters prioritaires du paragraphe 4.2 restent tous couverts par au moins un article en PR, la rotation de mots-cles n'a fait remonter aucun signal de demande exploitable non deja couvert, et le seuil de 14/25 n'a ete franchi par aucun sujet neuf. Conforme a la regle qu'une journee sans article publie est normale, une journee sans veille ne l'est pas (paragraphe 4.1), et a la priorite qualite avant quota (paragraphe 8.4).

Repartition par pilier inchangee depuis le 2026-09-11 : ~57/29/14, proche de la cible 60/30/10.

Le depot compte toujours 14 PR d'articles ouvertes depuis le 2026-08-22, soit 24 jours au 2026-09-15, aucune fusionnee sur GitHub (verifie ce run sur les 5 PR les plus recemment mises a jour : toutes encore a l'etat open ; seules les PR 3 et 11, corrections du prompt de reference, sont fusionnees).

## Point du 2026-09-14 : decouverte d'un second canal de contenu (/blog/) distinct de ce pipeline, aucun nouvel article produit

Acces depot reconfirme : authentifie KhalidBougria (proprietaire du compte, pas obougria), permissions push:true / admin:true inchangees, connecteur MCP GitHub local (local_unpacked_qunfei-wu_github-mcp-server-js). Bash indisponible tout le run, meme cause que les runs precedents depuis le 8 septembre (erreur de montage Windows) ; contournement navigateur integre a nouveau utilise avec succes pour lire .seo/*, sitemap.xml, robots.txt et des pages live.

Prompt de reference relu integralement depuis .seo/agent-prompt.md (version 3.2) : a jour, aucune divergence avec le texte reproduit dans la tache planifiee au-dela des corrections deja actees (Loi n27-06, URLs /articles/slug, marque OptimasProtect en un seul mot).

Decouverte nouvelle ce run : le sitemap.xml live liste toujours exactement les 12 memes articles deja identifies le 2026-09-12 (les deux plus recents, cahier-de-consignes-securite-maroc et controle-qualite-prestation-gardiennage-maroc, n'y figurent toujours pas 2 jours plus tard, ce qui allonge le decalage de synchronisation observe au-dela de ce qui avait ete estime). Plus important : le sitemap contient aussi une URL, https://optimasprotect.ma/blog/main-courante-electronique-vs-papier, sous le prefixe /blog/ et non /articles/, avec un slug different de celui produit par cet agent (main-courante-electronique-maroc). Verification du contenu de cette page : il s'agit d'un article distinct, de ton plus commercial et tres oriente listes a puces, qui ne correspond a aucune des branches article/* de ce depot. Conclusion : il existe au moins un second canal de publication de contenu sur optimasprotect.ma, independant de ce pipeline GitHub, qui traite un sujet identique (main courante electronique) sous une URL et un slug differents. Risque de cannibalisation SEO directe sur le cluster 6 (main courante electronique / numerique gardiennage), puisque deux pages du meme site vont potentiellement concurrencer les memes requetes. Ce canal est hors perimetre d'ecriture de cet agent (aucune instruction ne couvre un dossier ou une convention /blog/), mais merite une clarification explicite de l'utilisateur : ce second canal est-il gere par une autre equipe/outil, et faut-il l'exclure du perimetre de veille anti-doublon de cet agent ou au contraire en tenir compte activement pour eviter la cannibalisation.

robots.txt reverifie ce run (navigateur) : inchange par rapport au 2026-09-12, User-agent * Allow /, Content-Signal search=yes / ai-train=no, seuls des crawlers d'entrainement IA nommes sont bloques, Googlebot non restreint. Alerte anti-bot toujours levee.

site:optimasprotect.ma toujours a 0 resultat pertinent via l'outil de recherche web de cette session (limite documentee aux resultats US, fiabilite incertaine pour Google.ma sans Search Console).

Anti-doublon : relecture complete des 14 branches article/* et de leurs frontmatters (via get_file_contents sur chaque branche). Repartition par pilier confirmee et inchangee depuis le 2026-09-11 : pilier 1 = 8/14 (application-pointage-ads-maroc, cahier-de-consignes-securite-maroc, cahier-des-charges-gardiennage-maroc, controle-de-ronde-nfc-gardiennage-maroc, faux-pointage-ads-detecter-maroc, modele-rapport-de-ronde-maroc, prix-logiciel-gardiennage-maroc, rapport-intervention-ads-maroc), pilier 2 = 4/14 (controle-qualite-prestation-gardiennage-maroc, main-courante-electronique-maroc, portail-client-securite-privee-maroc, obligations-loi-27-06-employeur-maroc), pilier 3 = 2/14 (planning-agents-securite-maroc, loi-32-26-agents-securite-maroc). Ratio ~57/29/14, proche de la cible 60/30/10.

Rotation de mots-cles testee ce run (14 requetes, angles non essayes precedemment, orientees differenciateurs pilier 1) : tracabilite prestation gardiennage, preuve de passage agent de securite, horodatage ronde de securite, remplacer pointeuse gardiennage, controle de presence agent de securite, badge NFC agent de securite, litige client societe de gardiennage, logiciel gestion incidents securite privee, reporting client societe de securite, main courante numerique gardiennage, gestion des conges agents de securite, logiciel RH societe de gardiennage, vacation 12h agent de securite Maroc, societe de securite sans materiel. 0 suggestion pour toutes, regime pauvre en autocomplete confirme une nouvelle fois. trends_interest indisponible ce run (Google renvoie 429 sur les deux lots testes, geo=MA) : alerte outillage transitoire, a reessayer au prochain run.

Verification factuelle ciblee : recherche web sur la loi n°32.26 (article deja produit, PR loi-32-26-agents-securite-maroc, pilier 3) confirme via plusieurs sources de presse marocaines (Le Matin.ma, H24info, Medias24, L'Information.ma) l'exactitude des elements deja cites dans l'article (dahir n°1.26.27 du 3 juillet 2026, Bulletin officiel n°7526 du 16 juillet 2026, delai de mise en conformite de 9 mois). Un chiffre supplementaire circule dans la presse (environ 500 000 agents concernes) mais n'est confirme par aucune source primaire autorisee au sens du paragraphe 8.3 (presse uniquement) : ce chiffre n'a donc pas ete ajoute a l'article, conformement a la regle non negociable du paragraphe 8.3. A surveiller si le SGG/Bulletin Officiel ou le Ministere de l'Interieur publie ce chiffre.

Veille concurrentielle (recherche web ce run) : SEKUR / SEKUR Africa toujours en opacite tarifaire MAD cote Maroc, tarification EUR uniquement pour l'offre France ; une page comparative datee 2025 est apparue en plus de celle de 2026 deja documentee (sekur-africa.com/meilleurs-logiciels-securite-privee-2025/), aucun changement de positionnement ou de prix. Trackforce Valiant toujours positionne a l'international, pricing sur devis, aucune adaptation Maroc identifiee. Aucun nouvel acteur marocain detecte au-dela de secumall.ma et kver.ma deja documentes.

Aucun sujet reellement neuf (pilier 1, 2 ou 3) n'a passe le seuil de 14/25 ce run : les 10 clusters prioritaires du paragraphe 4.2 sont deja tous couverts par au moins un article en PR, et la rotation de mots-cles n'a produit aucun signal de demande exploitable. Conforme a la regle qu'une journee sans article publie est normale, une journee sans veille ne l'est pas (paragraphe 4.1). Aucun nouvel article, aucune mise a jour necessaire ce run.

Le depot compte toujours 14 PR ouvertes depuis le 2026-08-22, soit 23 jours au 2026-09-14, aucune fusionnee sur GitHub (seules les PR 3 et 11, corrections du prompt de reference, sont fusionnees).

## Point du 2026-09-12 : decouverte majeure, un mecanisme externe alimente deja le site depuis les branches article, aucun nouvel article produit

Acces depot reconfirme : authentifie KhalidBougria, push:true / admin:true, connecteur MCP GitHub local. Bash indisponible tout le run (meme erreur de montage Windows du 8 septembre) ; contournement navigateur integre a nouveau utilise avec succes.

Decouverte majeure : en verifiant directement sitemap.xml, robots.txt et plusieurs pages /articles/slug en direct sur le site live, il apparait que 12 des 14 articles produits par cet agent sont deja en ligne, sous forme de contenu quasi identique a celui des branches article (memes titres, memes prix, meme structure), alors qu'aucune des PR correspondantes n'a ete fusionnee sur GitHub (seules les PR 3 et 11, deux corrections du prompt de reference, sont fusionnees ; les 14 PR d'articles restent toutes ouvertes). La branche main ne contient toujours que .seo (reverifie ce jour), ce qui exclut un pipeline classique ou la fusion sur main declenche un deploiement. Le mecanisme reel reste inconnu, mais la conclusion factuelle change : le contenu atteint bien le site public, tres probablement via une reprise manuelle ou un script externe qui lit directement les branches article, avec un decalage de plusieurs jours (les 2 articles les plus recents, PR 15 du 2026-09-05 et PR 16 du 2026-09-11, ne sont pas encore en ligne ; le dernier article visiblement synchronise est celui du 2026-09-01, PR 14). Point a clarifier par l'utilisateur : la publication effective ne semble pas conditionnee a la fusion de la PR sur GitHub, ce qui merite une clarification sur la maniere dont la relecture humaine prevue en Phase 1 s'articule avec ce mecanisme.

robots.txt verifie directement ce run (via navigateur, hors perimetre de l'outil de fetch habituel) : User-agent * Allow /, avec Content-Signal search=yes, ai-train=no (Cloudflare). Seuls des crawlers d'entrainement IA nommes (GPTBot, CCBot, Google-Extended, ClaudeBot, Bytespider, etc.) sont bloques ; Googlebot n'est pas restreint. Sitemap declare et actif, listant les 12 articles deja en ligne. L'alerte historique sur un eventuel filtrage anti-bot est levee cote robots.txt.

site:optimasprotect.ma reste a 0 resultat pertinent ce run via l'outil de recherche web de cette session, mais cet outil est documente comme limite aux resultats US, ce qui limite sa fiabilite pour juger de l'indexation reelle sur Google.ma. A ne plus interpreter comme preuve de non-indexation sans confirmation Search Console.

Observation mineure, non actionnable cote contenu : le site live affiche OptImasProtect (I majuscule median) dans la balise title et l'en-tete visuel de chaque page, alors que le corps des articles utilise bien OptimasProtect (un seul mot) conformement a la consigne du 2026-08-29. Ecart entre l'habillage du site et le contenu editorial, a signaler a l'utilisateur mais hors perimetre d'action de cet agent.

Veille concurrentielle : SEKUR / SEKUR Africa toujours en tarification EUR pour l'offre France, opacite MAD toujours confirmee cote Maroc, aucun changement de positionnement. Trackforce Valiant toujours positionne a l'international, pricing sur devis, aucune adaptation Maroc identifiee. Aucun nouvel acteur marocain detecte au-dela de secumall.ma et kver.ma deja documentes.

Rotation de mots-cles testee ce run (15 requetes, angles non essayes precedemment) : frequence des rondes de securite, cahier de rondes gardiennage, application mobile agent de securite, ronde de securite sans internet, carte de ronde electronique, supervision agents de securite a distance, tag NFC gardiennage, temps de reponse incident securite privee, digitalisation securite privee Maroc, logiciel de gestion de rondes, verification de presence agent site client, combien coute un pointeur NFC, assurance societe de gardiennage Maroc, sous-traitance gardiennage Maroc, superviseur de securite outils. Un seul signal : cahier de rondes gardiennage vers cahier ronde de securite (score de demande 3/5, un seul pic Trends isole). Anti-doublon verifie : cette intention est deja entierement couverte par PR 7 (modele-rapport-de-ronde-maroc). Aucun nouvel article, aucune mise a jour necessaire.

Aucun nouvel article produit ce run. Conforme a la regle une journee sans article publie est normale, une journee sans veille ne l'est pas (paragraphe 4.1).

Repartition par pilier inchangee depuis le 2026-09-11 (aucun ajout) : pilier 1 = 8/14 (~57%), pilier 2 = 4/14 (~29%), pilier 3 = 2/14 (~14%), proche de la cible 60/30/10.

Le depot compte toujours 14 PR ouvertes depuis le 2026-08-22, aucune fusionnee sur GitHub, mais voir la decouverte ci-dessus qui relativise fortement la portee de cette statistique comme indicateur de rien ne se passe.

## Point du 2026-09-11 : 1 article produit (PR 16), 14 PR ouvertes, toujours aucune fusion, alerte outillage Bash

PR 16 (controle-qualite-prestation-gardiennage-maroc, pilier 2, score 17/25) ajoutee ce run, priorite pilier 2 pour corriger l'ecart de ratio signale depuis le 2026-08-31. Le depot compte desormais 14 pull requests ouvertes depuis le 2026-08-22, aucune fusionnee, soit 20 jours sans relecture humaine.

Alerte outillage ce run : le bac a sable Bash de la session est reste indisponible toute la duree du run (erreur de montage liee a une mise a jour Windows du 8 septembre, deja rencontree lors du run precedent du 2026-09-10). Contournement applique avec succes via le navigateur integre.

Acces au depot reconfirme ce run : authentifie en tant que KhalidBougria (proprietaire du compte), permissions push:true / admin:true inchangees, voie technique connecteur MCP GitHub local.

Veille concurrentielle reconfirmee par recherche web ce run : SEKUR / SEKUR Africa toujours en tarification EUR uniquement pour l'offre France, opacite MAD toujours confirmee cote Maroc, aucun changement de positionnement detecte. Aucun nouvel acteur marocain detecte (au-dela de secumall.ma et kver.ma, deja documentes le 2026-09-09).

site:optimasprotect.ma reconfirme a 0 resultat pertinent indexe ce run (recherche web).

## Point du 2026-09-05 : 1 article produit (PR 15), 13 PR ouvertes, toujours aucune fusion

PR 15 (cahier-de-consignes-securite-maroc, pilier 1, score 17/25) ajoutee ce run, nouveau sujet distinct du hub main courante. Le depot compte desormais 13 pull requests ouvertes depuis le 2026-08-22, aucune fusionnee apres plus de deux semaines.

site:optimasprotect.ma reconfirme a 0 resultat pertinent indexe ce run (recherche web). robots.txt toujours hors du perimetre autorise pour l'outil de fetch de cette session lors de ce run, donc toujours non verifie directement a cette date.

Acces au depot reconfirme ce run : authentifie en tant que KhalidBougria (proprietaire du compte), permissions push:true / admin:true inchangees.

## Point du 2026-09-03 : journee de veille seule, aucun nouveau sujet retenu, 12 PR toujours ouvertes

Aucune nouvelle PR ce run. Rotation de mots-cles ciblee sur des angles non testes : 0 suggestion pour toutes, confirmant une nouvelle fois le regime pauvre en autocomplete sur ce marche.

Constat structurel : les 10 clusters prioritaires du paragraphe 4.2 ont desormais chacun au moins un article en PR. Conformement a la regle une journee sans article publie est normale, une journee sans veille ne l'est pas (4.1), aucun article n'a ete produit ce run.

## Point du 2026-09-01 : 12 PR ouvertes, toujours aucune fusion

PR 14 (faux-pointage-ads-detecter-maroc, pilier 1, cluster 9, score 16/25) ajoutee ce run.

## Point du 2026-08-31 : 11 PR ouvertes, toujours aucune fusion

PR 13 (obligations-loi-27-06-employeur-maroc, hub conformite, score 18/25) ajoutee ce run.

## Arbitrage humain du 2026-08-29 (PR 11, mergee) - alertes /articles et ecart de marque RESOLUES

Le prompt de reference .seo/agent-prompt.md (version 3.2, PR 11 mergee le 2026-08-29) tranche les deux points laisses en suspens : (1) structure d'URL /articles/slug confirmee ; (2) orthographe OptimasProtect en un seul mot confirmee.

## Acces au depot

Authentifie en tant que KhalidBougria (proprietaire du compte), pas obougria comme prevu au prompt de reference. Permissions confirmees : push: true, admin: true. Voie technique : connecteur MCP GitHub local (local_unpacked_qunfei-wu_github-mcp-server-js). Visibilite du depot : public cote API. Branche par defaut : main.

## Generateur de site

Aucun fichier de generateur (astro.config, next.config, hugo.toml, package.json, etc.) n'est present dans le depot, y compris sur main qui ne contient que .seo/. Toutefois, voir le Point du 2026-09-12 et du 2026-09-15 ci-dessus : la verification directe du site live (sitemap.xml, pages /articles/slug) montre que la totalite des 14 articles produits sont desormais en ligne avec un contenu quasi identique aux branches article, sans qu'aucune PR d'article n'ait ete fusionnee. Le mecanisme de publication reel n'est donc pas un generateur configure dans ce depot au sens classique, mais un processus externe (probablement une reprise manuelle ou un script cote utilisateur) qui lit directement le contenu des branches article, avec un decalage de quelques jours desormais resorbe. Alerte revisee le 2026-09-14 : un second canal /blog/ totalement independant de ce depot existe egalement sur le meme site (voir Point du 2026-09-14), toujours actif au 2026-09-15, ce qui confirme que la publication d'optimasprotect.ma ne repose pas sur un pipeline unique et que ce depot n'est vraisemblablement qu'une des sources de contenu du site.

## Conventions etablies par cet agent

- Dossier de contenu : content/blog/ (dans les branches article/* uniquement ; absent de main).
- Nom de fichier : {slug}.md.
- URL publique visee : https://optimasprotect.ma/articles/{slug}.
- Liens internes : relatifs, /articles/{slug}.
- Marque : OptimasProtect en un seul mot pour la production future.

### Schema de frontmatter YAML (reference)

title, description, slug, tags, date, author (Team Optimas), draft, focus_keyword, pillar, score, canonical (https://optimasprotect.ma/articles/slug-court). Aucun champ image.

### Corps de l'article

Markdown standard (H1 unique en premiere ligne, puis H2/H3). Pas de classes CSS specifiques tant qu'aucun theme n'est branche.

### JSON-LD

En fin de corps d'article dans un bloc json-ld. Types : SoftwareApplication + Offer pour les articles pilier 1 avec prix, Article avec author.@type Organization, FAQPage pour le bloc FAQ.

## Hubs en constitution

- Hub pilier 1 : controle-de-ronde-nfc-gardiennage-maroc.
- Hub prix : prix-logiciel-gardiennage-maroc.
- Hub conformite (Loi n27-06 / cahiers des charges) : deux articles (cahier-des-charges-gardiennage-maroc, obligations-loi-27-06-employeur-maroc).

## Veille concurrentielle - URLs de reference

- Cercle 1 (Maroc) : SEKUR Africa - sekur-africa.com/logiciel/logiciel-securite-privee-gardiennage-maroc/, sekur-africa.com/tarifs/ (EUR uniquement), sekur-africa.com/meilleurs-logiciels-securite-privee-2025/ (page comparative). sekur.fr (hors perimetre Maroc mais a garder en tete), page comparative 2026 : sekur.fr/meilleurs-logiciels-securite-privee-2026/. EasyGard / SGGI (Marrakech) - sggi-maroc.com/82-easygard-logiciel-de-gestion-des-societes-de-gardiennage.html, offres.sggi.ma/easygard.html (nouveau, identifie le 2026-09-15, oriente RH/paie, pas de prix public).
- Cercle 2 (international) : Trackforce Valiant - trackforce.com/fr/solutions/gestion-des-gardiens-de-securite/. Pricing toujours non public.
- Ne pas confondre SEKUR Africa avec SEKUR France, hors perimetre Maroc. Ne pas confondre EasyGard/SGGI (editeur logiciel) avec Maroc Gard / marocgard.com (societe de gardiennage cliente potentielle, pas un concurrent logiciel).

## Alertes non resolues (arbitrage humain attendu)

1. Mecanisme de publication reel du depot vers le site live : desormais eclairci pour le pipeline article/* (voir Points du 2026-09-12 et du 2026-09-15) - le contenu atteint le site sans fusion de PR, via un canal non identifie avec precision, et la totalite des 14 articles est desormais en ligne. A clarifier par l'utilisateur : ce canal constitue-t-il deja la relecture humaine prevue, ou faut-il la renforcer.
2. Un second canal /blog/ distinct de ce depot publie egalement du contenu sur optimasprotect.ma (exemple : /blog/main-courante-electronique-vs-papier), toujours present au 2026-09-15, avec un risque de cannibalisation SEO sur des clusters deja traites par ce pipeline (main courante electronique). A clarifier par l'utilisateur : qui gere ce canal, et faut-il l'integrer au perimetre de veille anti-doublon de cet agent.
3. robots.txt : verifie a nouveau le 2026-09-15 via navigateur, aucun blocage de Googlebot constate (deux crawlers supplementaires bloques dans le bloc Cloudflare, sans impact). Alerte levee.
4. site:optimasprotect.ma : outil de recherche web non retente ce run ; historiquement 0 resultat, mais cet outil est documente comme limite aux resultats US - fiabilite incertaine pour Google.ma tant que la Search Console n'est pas connectee.
5. File de pull requests : 14 PR d'articles ouvertes depuis le 2026-08-22, soit 24 jours au 2026-09-15, toujours aucune fusionnee sur GitHub - a relire avec la nuance des Points du 2026-09-12 et du 2026-09-15 (le contenu n'est pas bloque en pratique, la totalite est desormais en ligne malgre l'absence de fusion).
6. Ecart de branding : le site live affiche OptImasProtect (I majuscule) dans son habillage, alors que le contenu editorial utilise OptimasProtect. A signaler a l'utilisateur, hors perimetre d'action de cet agent.

## Confirmation positive

Le format de frontmatter et le dossier content/blog/{slug}.md etabli au premier run fonctionnent toujours sans ajustement : 16 articles produits a ce jour au total (voir rapports quotidiens pour le detail). Le site live confirme desormais la publication integrale des 14 articles du pipeline (2026-09-15).
