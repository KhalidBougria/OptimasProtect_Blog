# Cartographie du depot - OptimasProtect_Blog

Derniere mise a jour : 2026-09-12 (semaine S37). Ce fichier est un document de travail vivant ; pour l'historique detaille jour par jour, voir .seo/rapports/.

## Point du 2026-09-12 : decouverte majeure, un mecanisme externe alimente deja le site depuis les branches article, aucun nouvel article produit

Accès depot reconfirme : authentifie KhalidBougria, push:true / admin:true, connecteur MCP GitHub local. Bash indisponible tout le run (meme erreur de montage Windows du 8 septembre) ; contournement navigateur integre a nouveau utilise avec succes.

Decouverte majeure : en verifiant directement sitemap.xml, robots.txt et plusieurs pages /articles/slug en direct sur le site live, il apparait que 12 des 14 articles produits par cet agent sont deja en ligne, sous forme de contenu quasi identique a celui des branches article (memes titres, memes prix, meme structure), alors qu'aucune des PR correspondantes n'a ete fusionnee sur GitHub (seules les PR 3 et 11, deux corrections du prompt de reference, sont fusionnees ; les 14 PR d'articles restent toutes ouvertes). La branche main ne contient toujours que .seo (reverifie ce jour), ce qui exclut un pipeline classique ou la fusion sur main declenche un deploiement. Le mecanisme reel reste inconnu, mais la conclusion factuelle change : le contenu atteint bien le site public, tres probablement via une reprise manuelle ou un script externe qui lit directement les branches article, avec un decalage de plusieurs jours (les 2 articles les plus recents, PR 15 du 2026-09-05 et PR 16 du 2026-09-11, ne sont pas encore en ligne ; le dernier article visiblement synchronise est celui du 2026-09-01, PR 14). Point a clarifier par l'utilisateur : la publication effective ne semble pas conditionnee a la fusion de la PR sur GitHub, ce qui merite une clarification sur la maniere dont la relecture humaine prevue en Phase 1 s'articule avec ce mecanisme.

robots.txt verifie directement ce run (via navigateur, hors perimetre de l'outil de fetch habituel) : User-agent * Allow /, avec Content-Signal search=yes, ai-train=no (Cloudflare). Seuls des crawlers d'entrainement IA nommes (GPTBot, CCBot, Google-Extended, ClaudeBot, Bytespider, etc.) sont bloques ; Googlebot n'est pas restreint. Sitemap declare et actif, listant les 12 articles deja en ligne. L'alerte historique sur un eventuel filtrage anti-bot est levee cote robots.txt.

site:optimasprotect.ma reste a 0 resultat pertinent ce run via l'outil de recherche web de cette session, mais cet outil est documente comme limite aux resultats US, ce qui limite sa fiabilite pour juger de l'indexation reelle sur Google.ma. A ne plus interpreter comme preuve de non-indexation sans confirmation Search Console (toujours non connectee a cette tache planifiee).

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

Aucun fichier de generateur (astro.config, next.config, hugo.toml, package.json, etc.) n'est present dans le depot, y compris sur main qui ne contient que .seo/. Toutefois, voir le Point du 2026-09-12 ci-dessus : la verification directe du site live (sitemap.xml, pages /articles/slug) montre que 12 des 14 articles produits sont deja en ligne avec un contenu quasi identique aux branches article, sans qu'aucune PR n'ait ete fusionnee. Le mecanisme de publication reel n'est donc pas un generateur configure dans ce depot au sens classique, mais un processus externe (probablement une reprise manuelle ou un script cote utilisateur) qui lit directement le contenu des branches article, avec un decalage de quelques jours. Alerte revisee : ce n'est plus purement bloquant pour la mise en ligne (le contenu passe), mais le lien entre ce mecanisme et la relecture humaine de Phase 1 reste a clarifier par l'utilisateur.

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

- Cercle 1 (Maroc) : SEKUR Africa - sekur-africa.com/logiciel/logiciel-securite-privee-gardiennage-maroc/, sekur-africa.com/tarifs/ (EUR uniquement). sekur.fr (hors perimetre Maroc mais a garder en tete), page comparative 2026 : sekur.fr/meilleurs-logiciels-securite-privee-2026/.
- Cercle 2 (international) : Trackforce Valiant - trackforce.com/fr/solutions/gestion-des-gardiens-de-securite/. Pricing toujours non public.
- Ne pas confondre SEKUR Africa avec SEKUR France, hors perimetre Maroc.

## Alertes non resolues (arbitrage humain attendu)

1. Mecanisme de publication reel du depot vers le site live : desormais partiellement eclairci (voir Point du 2026-09-12) - le contenu atteint le site sans fusion de PR, via un canal non identifie avec precision. A clarifier par l'utilisateur : ce canal constitue-t-il deja la relecture humaine prevue, ou faut-il la renforcer.
2. robots.txt : verifie ce jour (2026-09-12) via navigateur, aucun blocage de Googlebot constate. Alerte levee.
3. site:optimasprotect.ma : 0 resultat via l'outil de recherche web, mais cet outil est documente comme limite aux resultats US - fiabilite incertaine pour Google.ma tant que la Search Console n'est pas connectee.
4. File de pull requests : 14 PR ouvertes depuis le 2026-08-22, soit 21 jours au 2026-09-12, toujours aucune fusionnee sur GitHub - a relire avec la nuance du Point du 2026-09-12 (le contenu n'est pas bloque en pratique).
5. Ecart de branding : le site live affiche OptImasProtect (I majuscule) dans son habillage, alors que le contenu editorial utilise OptimasProtect. A signaler a l'utilisateur, hors perimetre d'action de cet agent.

## Confirmation positive

Le format de frontmatter et le dossier content/blog/{slug}.md etabli au premier run fonctionnent toujours sans ajustement : 16 articles produits a ce jour au total (voir rapports quotidiens pour le detail).
