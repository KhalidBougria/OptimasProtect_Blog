## Point du 2026-09-18 : aucun changement detecte, etat stable depuis le 2026-09-16 (detail complet dans .seo/rapports/2026-09-18.md et .seo/backlog.md)

Acces depot reconfirme (KhalidBougria, push:true/admin:true, connecteur MCP GitHub local). Bash indisponible tout le run (meme erreur de montage Windows depuis le 8 septembre) ; contournement navigateur integre utilise avec succes. Prompt de reference .seo/agent-prompt.md (version 3.2) relu integralement, a jour, aucune divergence.

Sitemap.xml et robots.txt reverifies via navigateur : inchanges depuis le 2026-09-16 (toujours 14 articles du pipeline sous /articles/, second canal /blog/main-courante-electronique-vs-papier toujours present ; robots.txt simplifie, Googlebot non restreint). Les 14 branches article/* et le statut des PR (seules PR 3 et 11 fusionnees) ont ete reconfirmes via list_branches et list_pull_requests.

Veille mots-cles (16 requetes, marche Maroc gl=ma/hl=fr) : deux suggestions autocomplete obtenues, toutes deux deja couvertes (voir rapport du jour). trends_interest indisponible (429). Aucun sujet neuf n'a franchi le seuil de 14/25. Veille concurrentielle : SEKUR Africa confirme sa tarification publique en EUR (hors MAD) sur son site Afrique ; EasyGard/SGGI et Trackforce Valiant inchanges ; KVER/SecuMall reconfirmes comme revendeurs de materiel (cercle 3). Aucun nouvel acteur logiciel marocain.

Decision : aucun nouvel article produit ni mis a jour ce run. Repartition par pilier inchangee depuis le 2026-09-11 (pilier 1 = 8/14, pilier 2 = 4/14, pilier 3 = 2/14, ~57/29/14, proche de la cible 60/30/10). Alertes 1, 2 et 6 de ce fichier non resolues, reportees telles quelles.

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

Anti-doublon : relecture complete des 14 branches article/* et de leurs