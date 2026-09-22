## Point du 2026-09-22 : écart de run de 4 jours (dernier rapport le 2026-09-18), état du dépôt et du site inchangé, aucun nouvel article, deux nouveaux logiciels internationaux identifiés et écartés (France uniquement)

Accès dépôt reconfirmé : authentifié KhalidBougria (propriétaire du compte, pas obougria), permissions push:true / admin:true inchangées, connecteur MCP GitHub local. Alerte outillage nouvelle ce run : le bac à sable Linux (Bash) de cette session a échoué au démarrage avec un message différent de celui documenté sans interruption depuis le 8 septembre (« Workspace unavailable. The isolated Linux environment failed to start (VM service not running. Restart your computer to restore it.) » contre l'erreur de montage Windows habituelle) — cause potentiellement distincte, à surveiller. Contournement navigateur intégré + API GitHub MCP + javascript_tool (atob/btoa) appliqué avec succès pour l'ensemble des opérations de ce run ; aucun impact sur le résultat puisqu'aucune écriture d'article n'était nécessaire.

Écart de calendrier : le dernier rapport quotidien disponible est daté du 2026-09-18. Aucun rapport ni synthèse hebdomadaire pour les 2026-09-19, 20 et 21 (dont un lundi, le 09-21, qui aurait dû porter une synthèse hebdomadaire) : la tâche planifiée n'a apparemment pas été exécutée ces jours-là, hors du contrôle de cet agent. Ce run couvre donc un écart de veille de 4 jours.

Prompt de référence relu intégralement depuis .seo/agent-prompt.md (version 3.2) : à jour, aucune divergence, corrections déjà actées (Loi n°27-06, URLs /articles/slug, marque OptimasProtect en un mot) toujours appliquées.

### État du dépôt

14 branches article/* reconfirmées via list_branches (identiques à la liste du 09-18). 14 PR ouvertes reconfirmées via list_pull_requests, état open sur les mêmes numéros (1, 2, 4, 5, 6, 7, 8, 9, 10, 12, 13, 14, 15, 16) : aucune fusion, aucune nouvelle PR depuis le 08-22, soit 31 jours au 09-22. Seules les PR 3 et 11 (corrections du prompt) restent fusionnées.

### Sitemap et robots.txt

Reconfirmés inchangés via navigateur : sitemap.xml liste toujours les 14 articles du pipeline sous /articles/ plus les pages produit (pointage-agents, rondes-securite, gestion-rh-agents, gestion-incidents, portail-client, gestion-equipements) et le second canal /blog/main-courante-electronique-vs-papier, toujours présent. robots.txt toujours réduit à User-agent */Allow: / plus Sitemap, Googlebot non restreint.

Écart de branding reconfirmé : le titre de la page d'accueil affiche toujours « OptImasProtect – Gestion de gardiennage au Maroc » (I majuscule médian), alors que le corps des articles utilise bien OptimasProtect en un mot. Non résolu, hors périmètre d'action de cet agent.

### Veille mots-clés et SERP

13 requêtes testées ce run (gl=ma, hl=fr), angles non essayés précédemment : avis client société de gardiennage Maroc, comparatif logiciel gardiennage, société de sécurité amende cahier des charges, modèle main courante gardiennage, erreur de pointage agent de sécurité, loi 32.26 agents de sécurité, gestion de flotte agents de sécurité, rapport de ronde PDF, société de sécurité cahier des charges type, combien coûte une ronde de sécurité, journée de travail agent de sécurité Maroc loi, logiciel de sécurité privée avis, cahier des charges sécurité privée modèle.

Deux suggestions obtenues sur 13 : « modèle main courante gardiennage » vers « modèle main courante sécurité pdf » et « modèle main courante sécurité excel » ; « rapport de ronde PDF » vers « rapport de ronde pdf » et « rapport ronde de sécurité pdf ». Anti-doublon vérifié par lecture intégrale des deux articles concernés : la première intention est déjà couverte par main-courante-electronique-maroc (PR4, comparatif papier/électronique et contenu d'une entrée) ; la seconde est déjà couverte par modele-rapport-de-ronde-maroc (PR7, ce que doit contenir un rapport, checklist, FAQ dédiée). trends_interest (geo=MA, 12 mois) sur « modèle main courante sécurité » et « rapport de ronde pdf » : intérêt à 0 sur toutes les régions marocaines disponibles, aucune requête associée. Régime pauvre en signal de demande mesurable confirmé une nouvelle fois, conforme au constat répété sans interruption depuis plusieurs semaines. Aucun sujet réellement neuf n'a franchi le seuil de 14/25 ce run.

### Veille concurrentielle

SEKUR Africa, EasyGard/SGGI, Trackforce Valiant : non revérifiés en détail ce run (dernière vérification du 09-16/09-18 jugée suffisamment récente), aucun changement attendu.

Recherche web ciblée sur de nouveaux entrants : « TRACKTIK » mentionné dans les résultats, mais il s'agit du même éditeur que Trackforce Valiant (fusion TrackTik/Trackforce déjà ancienne), pas un nouvel acteur. Deux logiciels non documentés jusqu'ici identifiés et vérifiés directement par navigation : BanetteOne (banetteone.com) et eBrigade (ebrigade.app), tous deux positionnés « sécurité privée / gardiennage » et donc a priori dans le champ de veille. Vérification du contenu de chaque site : eBrigade cite explicitement la carte professionnelle CNAPS, les qualifications SSIAP et la convention collective Prévention Sécurité, cadre réglementaire strictement français ; BanetteOne affiche une liste de clients aux noms français (dont National France Sécurité, Opale Picarde Sécurité), sans aucune mention du Maroc. Conclusion : les deux solutions sont France uniquement, sans adaptation Maroc identifiée, traitées comme le cercle 2 (international, hors cible géographique) et non ajoutées au cercle 1 (Maroc). Documentées ici pour éviter de les revérifier inutilement lors des prochains runs.

### Décision de production

Aucun sujet réellement neuf n'a franchi le seuil de 14/25 ce run (2 signaux obtenus, tous deux déjà couverts par des articles existants, vérifié par lecture intégrale). Aucun nouvel article produit ni mis à jour. Conforme à la règle qu'une journée sans article publié est normale, une journée sans veille ne l'est pas (paragraphe 4.1), et à la priorité qualité avant quota (paragraphe 8.4).

Répartition par pilier inchangée depuis le 2026-09-11 : pilier 1 = 8/14 (~57%), pilier 2 = 4/14 (~29%), pilier 3 = 2/14 (~14%), proche de la cible 60/30/10.

Alertes 1, 2, 5 et 6 de ce fichier non résolues, reportées telles quelles. Alerte 3 (robots.txt) reste levée, alerte 4 (site:optimasprotect.ma) non retestée ce run.

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

Marché ciblé : Maroc (gl=ma, hl=fr). Rotation de 15 requêtes sur des angles non testés lors des runs précédents (voir cumul dans les rapports du 08 au 15 sep