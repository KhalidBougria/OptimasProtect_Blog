# Backlog éditorial — OptimasProtect

Dernière mise à jour : 2026-09-11 (semaine S37).

## Décision prise ce run (2026-09-11)

**1 nouvel article produit : PR #16 (`controle-qualite-prestation-gardiennage-maroc`, pilier 2, score 17/25).** Priorité donnée au pilier 2 conformément à l'écart de ratio signalé sans interruption depuis le 2026-08-31 (pilier 2 sous la cible de 30 %). Rotation testée ce run, environ 25 requêtes : pilier 2 (`notation prestation sécurité privée`, `avis client société de sécurité Maroc`, `signalement incident gardiennage`, `application client société de sécurité`, `gestion réclamation client sécurité privée`, `assurance qualité gardiennage`, `bouton alerte panique agent de sécurité`, `rapport de ronde en ligne client`, `suivi qualité prestation gardiennage`, `rapport de gardiennage mensuel client`, `preuve de service société de sécurité`, `contester facture société de gardiennage`, `indicateur de performance société de sécurité`, `justificatif de ronde sécurité`, `document ronde de sécurité`, `preuve ronde de sécurité client`, `comment prouver qu'une ronde a été effectuée`, `litige client agent de sécurité preuve`, `prestation de gardiennage non effectuée que faire`), pilier 1 (`logiciel de gardiennage Casablanca`, `badge de présence agent de sécurité`, `audit rondes de sécurité`, `solution de ronde connectée`, `preuve de passage ronde sécurité`, `contrôle prestation gardiennage client`, `litige prestation gardiennage`), pilier 3 (`SIRH agent de sécurité Maroc`, `badge pointage agent de sécurité`).

Un seul signal exploitable sur l'ensemble de la rotation : `assurance qualité gardiennage` → suggestion `contrôle qualité sécurité privée`. Vérifié comme intention distincte des 13 articles déjà en PR (en particulier `portail-client-securite-privee-maroc`, qui documente ce que le portail donne à voir, et `rapport-intervention-ads-maroc`, qui documente le format d'un document d'incident) — aucun des deux ne traite la méthodologie de contrôle qualité elle-même. Score 17/25 (intention business 4, faisabilité de rank 4, avantage local 3, volume 2 faute de signal fort, fraîcheur/information gain 4 grâce au tableau comparatif méthodes traditionnelles/traçabilité et à l'exemple chiffré). Article produit et publié en PR #16, pilier 2, sans citation de chiffre réglementaire (angle opérationnel, aucun risque de sourcing au sens du §8.3).

`trends_interest` (`geo=MA`, 12 mois) sur `justificatif de ronde`, `preuve de passage`, `document ronde de sécurité` : deux pics isolés sur des semaines distinctes, aucune série exploitable, signal trop ponctuel pour être retenu comme sujet à part entière.

Veille concurrentielle (recherche web ce run) : recherche `contrôle qualité prestation gardiennage sécurité privée Maroc` fait remonter un article de presse (Le Matin.ma) mentionnant une intensification des contrôles de l'inspection du travail en 2024 sur les entreprises de sécurité (1 022 visites, 9 160 observations) — **source non autorisée au sens du §8.3 (presse, pas une source primaire de la liste), chiffre non repris dans l'article produit.** SEKUR / SEKUR Africa : aucun changement de positionnement ou de tarification détecté par rapport aux runs précédents (EUR uniquement pour l'offre France, opacité MAD toujours confirmée côté Maroc). Aucun nouvel acteur marocain détecté.

`site:optimasprotect.ma` reconfirmé à 0 résultat pertinent indexé ce run (recherche web) — seuls des homonymes sans rapport remontent.

**Alerte outillage ce run :** le bac à sable Bash de cette session est resté indisponible toute la durée du run (erreur de montage liée à une mise à jour Windows du 8 septembre, déjà annoncée par la plateforme). Contournement appliqué avec succès : lecture des fichiers `.seo/*.md` du dépôt via navigation du navigateur intégré vers les URLs `raw.githubusercontent.com` (texte brut, pas de décodage base64 nécessaire), et encodage base64 du nouvel article via `TextEncoder`/`btoa` exécuté dans la page du navigateur avant l'appel `create_or_update_file`. Aucun impact sur la qualité de la veille ou de la production ce run, mais le contournement ajoute plusieurs appels par rapport à une session Bash fonctionnelle — à noter si le problème persiste sur plusieurs runs.

**Point signalé avec insistance croissante :** le dépôt compte désormais **14 pull requests ouvertes depuis le 2026-08-22, aucune fusionnée**, soit **20 jours** sans relecture humaine au 2026-09-11. Ce point est signalé sans interruption depuis le 2026-08-31 et continue de croître en ancienneté sans qu'aucune action humaine n'ait eu lieu. L'alerte haute « aucun générateur de site connecté à ce dépôt » (voir `.seo/repo-map.md`) reste elle aussi active et non résolue.

## Décision prise ce run (2026-09-09)

**0 nouvel article, 0 enrichissement.** Rotation testée ce run, priorité pilier 2 (écart de ratio non résorbé depuis plusieurs runs) : `portail client rapport incident sécurité`, `main courante incident sécurité privée`, `délai de réponse incident sécurité privée`, `preuve intervention agent de sécurité`, `historique interventions société de sécurité`, `tableau de bord client sécurité privée`, `alerte sécurité temps réel site client`, `suivi ronde en temps réel client`, `export rapport mensuel sécurité gardiennage`, `logiciel gestion incident sécurité` ; pilier 1 : `digitaliser main courante gardiennage`, `remplacer registre papier gardiennage`, `badge NFC ronde de sécurité`, `erreur de pointage agent de sécurité`, `logiciel de sécurité gardiennage devis`, `logiciel de ronde de sécurité sans matériel` ; pilier 3 : `turnover agent de sécurité Maroc solution` : **0 suggestion exploitable sur 16 des 17 requêtes**, régime pauvre en autocomplete confirmé une nouvelle fois.

Deux signaux identifiés :

- `rapport incident sécurité` (+ `rapport d'incident de sécurité`) → intention déjà couverte par la PR #10 (`rapport-intervention-ads-maroc`), enrichie le 2026-09-06 avec précisément ce synonyme. Anti-doublon, pas de nouvel article.
- `gestion de conflit agent de sécurité` / `gestion des conflits agent de sécurité` / `formation gestion de crise agent de sécurité` → intention formation/conduite du personnel, exclue par la règle §4.3.2 (têtes de requête emploi/formation). Non retenu.

`trends_interest` (`geo=MA`, 12 mois) sur `rapport incident sécurité`, `logiciel gardiennage Maroc`, `controle de ronde` : plat à 0 sur toutes les régions testées.

**Aucun sujet pilier 1, 2 ou 3 réellement neuf n'a passé le seuil de 14/25 ce run.** Aucune création ni aucun enrichissement n'a été retenu — conformément à la logique anti-doublon et à la règle « une journée sans article publié est normale, une journée sans veille ne l'est pas » (§4.1). L'écart de ratio pilier 2 (toujours sous la cible de 30 %) reste donc non résorbé ce run, faute de signal exploitable dans ce pilier.

Veille concurrentielle : SEKUR / SEKUR Africa toujours en tarification EUR uniquement pour l'offre France (à partir de 99,99 €/mois/6 utilisateurs), opacité tarifaire MAD côté Maroc toujours confirmée, aucun changement de positionnement détecté. Trackforce Valiant : positionnement international inchangé, pricing sur devis, aucune adaptation Maroc identifiée. **Nouveaux acteurs détectés ce run : `secumall.ma` et `kver.ma`**, revendeurs marocains de contrôleurs de ronde physiques (boîtiers Rondier/RFID) — matériel, pas logiciel SaaS ; renforce le différenciateur « sans matériel dédié » d'Optimas, à garder en tête pour un futur contenu comparatif sans dénigrement nominal (§8.2). GRS Maroc : société de gardiennage cliente potentielle utilisant elle-même la technologie NFC en interne, pas un éditeur concurrent.

`site:optimasprotect.ma` reconfirmé à 0 résultat pertinent indexé (recherche web).

**Vérification structurelle ce run :** la racine de `main` a été recontrôlée directement (listing API) et ne contient que le dossier `.seo/` — aucun `content/blog`, aucun générateur, aucun `.github/workflows`. Ceci infirme dans l'état actuel l'alerte historique de la PR #9 (2026-08-26) sur un workflow de force-push vers `main` : ce mécanisme n'est pas actif sur `main` tel que constaté ce jour. À resurveiller si un pipeline est branché.

**Point signalé avec insistance croissante :** le dépôt compte toujours **13 pull requests ouvertes depuis le 2026-08-22, aucune fusionnée**, soit désormais **18 jours** sans relecture humaine. Ce point est signalé sans interruption depuis le 2026-08-31 et continue de croître en ancienneté sans qu'aucune action humaine n'ait eu lieu. L'alerte haute « aucun générateur de site connecté à ce dépôt » (voir `.seo/repo-map.md`) reste elle aussi active et non résolue.

## Décision prise ce run (2026-09-08)

**0 nouvel article, 0 enrichissement.** Rotation testée ce run sur des angles non essayés précédemment, tous piliers confondus : pilier 2 (`logiciel gestion incidents sécurité privée`, `alerte panique agent de sécurité`, `communication client société de sécurité`, `consultation rapport ronde client en ligne`), pilier 3 (`planning agents de sécurité logiciel`, `remplacement agent de sécurité absence`, `gestion heures agent de sécurité Maroc`, `contrat de travail agent de sécurité Maroc`, `évaluation performance agent de sécurité`), pilier 1 (`digitaliser rondes de sécurité Maroc`, `alternative pointeuse biométrique gardiennage`, `logiciel conforme cahier des charges gardiennage`, `effectif agent de sécurité minimum site`, `consigne de sécurité gardiennage modèle`, `gestion multi-sites société de sécurité`, `logiciel de ronde sans matériel dédié`, `essai gratuit logiciel gardiennage`, `comparatif logiciel gardiennage Maroc`) et angles sectoriels (`gardiennage site industriel Maroc`, `sécurité centre commercial Maroc`, `gardiennage chantier Maroc`, `gardiennage résidence Maroc logiciel`, `cahier des charges type gardiennage Maroc`) : **0 suggestion exploitable sur 20 des 21 requêtes**, régime pauvre en autocomplete une nouvelle fois confirmé sur ce marché.

Deux signaux identifiés, tous deux déjà couverts par des PR existantes (anti-doublon, §0) :

- `planning agents de sécurité logiciel` → suggestion `logiciel planning agent de sécurité gratuit`. Vérification du contenu de PR #6 (`planning-agents-securite-maroc`) : la FAQ de cet article répond déjà directement à « Un logiciel de planning gratuit suffit-il pour une petite société de sécurité ? ». Intention déjà couverte, aucune mise à jour nécessaire.
- `appel d'offre gardiennage Maroc` → 5 suggestions (« appel d'offre gardiennage maroc 2025/2026 », « appel d offre sécurité gardiennage maroc »). Signal réel, mais recoupe directement l'intention de PR #8 (`cahier-des-charges-gardiennage-maroc`, hub conformité, cluster 7), qui contient déjà une section et une checklist dédiées à « répondre à un appel d'offres de gardiennage ». Intention déjà couverte en profondeur, aucune mise à jour nécessaire.

`trends_interest` (`geo=MA`, 12 mois) sur `logiciel de ronde`, `digitalisation gardiennage`, `pointage agent sécurité` : aucune série temporelle exploitable (`interest_over_time` vide), un seul pic isolé sur une région (Tadla-Azilal, valeur 100, toutes les autres régions à 0) — signal trop ponctuel pour être retenu.

**Aucun sujet pilier 1, 2 ou 3 réellement neuf n'a passé le seuil de 14/25 ce run.** Les 10 clusters prioritaires du §4.2 ayant déjà chacun au moins un article en PR, et aucun angle testé ce run n'apportant un signal ou une intention suffisamment distincte, aucune création ni aucun enrichissement n'a été retenu — conformément à la logique anti-doublon et à la règle « une journée sans article publié est normale, une journée sans veille ne l'est pas » (§4.1). L'écart de ratio pilier 2 (toujours sous la cible de 30 %, voir répartition ci-dessous) reste donc non résorbé ce run, faute de signal exploitable dans ce pilier.

Veille concurrentielle : SEKUR a publié une nouvelle page comparative datée 2026, `sekur.fr/meilleurs-logiciels-securite-privee-2026/` (« Les 5 meilleurs logiciels pour agences de sécurité privée & de gardiennage en 2026 »), qui semble succéder à la version « 2025 » déjà documentée (`sekur-africa.com/meilleurs-logiciels-securite-privee-2025/`). Format à garder en tête comme idée de contenu futur pour le hub prix ou pilier 2, avec la prudence habituelle sur la comparaison nominale (§8.2) — aucune action ce run. SEKUR Africa se présente par ailleurs comme née en 2024 (repositionnement) ; une mise à jour produit mineure (SEKUR Africa 4.31) a également été repérée sans impact sur le positionnement ou les prix déjà documentés. Trackforce Valiant : positionnement international inchangé, pricing toujours sur devis, aucune adaptation Maroc identifiée. Aucun nouvel acteur marocain détecté.

`site:optimasprotect.ma` reconfirmé à 0 résultat pertinent indexé (recherche web) — seuls des homonymes sans rapport (Optimas Solutions, OptiRTC, etc.) remontent.

**Point signalé avec insistance croissante :** le dépôt compte toujours **13 pull requests ouvertes depuis le 2026-08-22, aucune fusionnée**, après plus de deux semaines. Ce point est signalé sans interruption depuis le 2026-08-31 et continue de croître en ancienneté sans qu'aucune action humaine n'ait eu lieu. L'alerte haute « aucun générateur de site connecté à ce dépôt » (voir `.seo/repo-map.md`) reste elle aussi active et non résolue.

## PR ouvertes (en attente de relecture humaine)

- PR #1 `controle-de-ronde-nfc-gardiennage-maroc` — pilier 1 — hub pilier 1.
- PR #2 `prix-logiciel-gardiennage-maroc` — pilier 1 — hub prix.
- PR #4 `main-courante-electronique-maroc` — pilier 2 — cluster 6.
- PR #5 `portail-client-securite-privee-maroc` — pilier 2.
- PR #6 `planning-agents-securite-maroc` — pilier 3.
- PR #7 `modele-rapport-de-ronde-maroc` — pilier 1 — cluster 5.
- PR #8 `cahier-des-charges-gardiennage-maroc` — pilier 1 — cluster 7, hub conformité. Article réglementaire, reste en PR en permanence (§3.3).
- PR #9 `application-pointage-ads-maroc` — pilier 1 — cluster 3.
- PR #10 `rapport-intervention-ads-maroc` — pilier 2 — cluster 5 (variante). Enrichie le 2026-09-06 (synonyme « rapport d'incident » + modèle prêt à remplir).
- PR #12 `loi-32-26-agents-securite-maroc` — pilier 3 — Loi n°32.26 (journée de 8h). Score 21/25, article réglementaire, reste en PR en permanence.
- PR #13 `obligations-loi-27-06-employeur-maroc` — pilier 1 — cluster 8, hub conformité. Score 18/25, article réglementaire, reste en PR en permanence.
- PR #14 `faux-pointage-ads-detecter-maroc` — pilier 1 — cluster 9. Score 16/25, article non réglementaire.
- PR #15 `cahier-de-consignes-securite-maroc` — pilier 1 — adjacent au cluster 6 (main courante), intention distincte. Score 17/25, ajouté le 2026-09-05.
- PR #16 `controle-qualite-prestation-gardiennage-maroc` — pilier 2 — méthodologie de contrôle qualité. Score 17/25, ajouté le 2026-09-11.

**14 PR ouvertes, aucune fusionnée à ce jour** (dépôt actif depuis le 2026-08-22, soit **20 jours** sans relecture humaine au 2026-09-11 — ce point continue de croître). Répartition par pilier après ajout de PR #16 : pilier 1 = 8/14 (~57 %), pilier 2 = 4/14 (~29 %), pilier 3 = 2/14 (~14 %). Le pilier 2 se rapproche enfin de sa cible de 30 % grâce à l'ajout de ce run ; pilier 1 revient sous sa cible haute historique, pilier 3 reste légèrement au-dessus de sa cible de 10 %. Prochaine session : continuer à privilégier le pilier 2 si un sujet réellement neuf passe le seuil de 14/25, sinon revenir au pilier 1 conformément à la règle de bascule (§0).
