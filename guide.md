# Tuto stream TLS

## Installation (au début du tournoi)

### Physique

Pour trouver rapidement le matériel : tous les câbles sont dans la valise noire, tous les appareils / boites sont dans la valide grise.  
Les câbles vidéo/audio et les autres dans des compartiments différents dans la valise. Les câbles HDMI ont des scratchs gris, les rallonges USB des scratchs verts

Note : je pars du principe qu'on utilise la table de mixage, mais on peut aussi utiliser la carte son (scarlett 2i2), ça ne fait pas bcp de différence  

/!\ Si vous faites le rangement, lisez bien la partie dédiée plus bas svp !

La première chose à faire est le choix du PC. Pour rappel, on a 2 PC fixes, dont un petit et très facile à transporter (boite orange dans la valise grise) et une grosse tour (rangée dans son carton). Je recommande la tour car elle marche simplement mieux, mais si vous vous sentez pas de la bouger (elle pèse un peu), le petit PC marche.

- On sort le PC, et on branche son alim (elle se trouve dans la valide grise, c'est le *gros* transfo)
- On place les 5 écrans et branche leurs alims
  - Les deux écrans AOC (sac intersport) pour les joueurs
  - Pour la régie (attention quand vous branchez les écrans au gros PC via HDMI, il y a une ligne de 4 prises HDMI sur fond noir, ce ne sont PAS les sorties vidéo, il faut regarder un peu plus haut)
    - Avec le petit PC : on met le Viewsonic (TLS View 1) branché en DisplayPort au PC, et le TLS Samsung 4 branché en HDMI.
    - Avec le gros PC : on met le Viewsonic (TLS View 1) et un autre écran disponant d'un port DisplayPort (faut voir avec les TO). On les branche en displayport au PC. Dans cette disposition on n'aura pas besoin du TLS Samsung 4 donc penser à le proposer aux TO pour les setups
  - Pour les casters on sort l'écran TLS Samsung 3.
    - Si pas de projecteur, on le branche direct au PC en HDMI
    - Si on veut brancher un projecteur, déjà faut s'assurer d'avoir un câble HDMI assez long, et surtout il faut sortir le splitter HDMI **2 sorties** (dans la boite blanche et bleu foncé). On branche alors l'écran des casters à l'une des sorties du splitter, et le projecteur à l'autre sortie, puis l'entrée du splitter à la sortie HDMI du PC.
- Si on est sur le petit PC, on branche le HUB USB au PC (ce n'est PAS la boite avec marqué Hub USB), c'est le carton rectangulaire tout blanc
- On branche en USB (les * indique les périphériques à brancher directement au PC et pas au hub si y en a un)
  - * Si on est sur le petit PC, la carte de capture (elle se trouve dans une boite transparente dans la valise grise). Si on est sur le gros PC pas besoin de carte de capture !
  - * La Logi Stream Cam (dans une autre boite transparente avec les autres cams) via usb c (y a bien une prise USB-C sur le PC)
  - Une des cams USB noires, qu'on va utiliser comme cam joueurs (utiliser une rallonge USB si trop loin de la régie)
  - La souris et le clavier
- On s'occupe ensuite des HDMIs pour le jeu : 
  - On sort le splitter 4 sortie, et on branche son alim
  - On branche la sortie HDMI de la switch à l'entrée du splitter
  - On branche les écrans joueurs à 2 sorties du splitter
  - On branche une 3ème sortie du splitter à l'entrée (in) de la carte de capture. Si on est sur le gros PC pas de carte de capture, les 4 prises HDMI sur fond noir tout en bas de l'arrière du PC font office de carte de capture.
- On sort la table de mixage (valise métalique noire) ou la carte son (boite en carton focusrite). Il est recommandé d'utiliser la table de mixage (c'est pas si compliqué vraiment promis) car la carte son a du mal à tenir tout le stream.
  - Dans tous les cas, on branche en USB au PC avec le câble USB qui se trouve dans la boite/valise
  - Pour la table de mixage, il faut sortir son alim (dans la valise également)
- On sort les casque micro, qui se trouvent dans des housses noires
  - Dans chaque housse se trouve un casque et un câble séparés, une vis (dans la pochette au font de la housse), et un splitter jack (dans 1 des 2)
  - On commence par brancher la prise carrée au bout du câble au casque, puis une fois que la prise est bien insérée on tourne la vis dans le trou au niveau de la prise (pour maintenir le câble)
  - Si on est sur la carte son (le boitier rouge), on branche le splitter dans la prise jack en bas à droite de la carte son. Puis, pour chaque casque, on branche sa prise jack, et l'autre embout (XLR) à la prise correspondante sur l'avant de la carte son.
  - Si on est sur la table de mixage, les grosses prises des casques (XLR) vont dans les prises tout en haut de la table (utiliser la 2ème et la 3ème). Le splitter se branche dans la prise jack en bas à droite de la partie supérieure (marquée "Phones")
- On allume la table de mixage le cas échéant (switch juste à côté de l'alim, attention à pas allumer l'autre switch)
- On branche le cable ethernet de la box au PC.
- Pour le casque régie il est sans fil, dans sa boite il y a une petite clé USB à brancher sur un port USB du PC ; il faut l'allumer avec le bouton à gauche ; il peut être bon de le mettre à charger (cable USB-C) avant le début du tournoi
- On sort aussi l'ampli jack (le truc sur lequel les joueurs doivent brancher leurs casques, dans un carton marron) : on n'oublie pas son bloc chargeur, et on met le jack sur un des deux écrans. 

Si disponible on sort aussi la tablette pour les bans, et on lance le navigateur internet.

### Logicielle
Si tout n'est pas déjà installé, voir section "Première installation" plus bas

On commence par lancer OBS.

Dans OBS : 

- On commence par vérifier les caméras :
  - Pour Cam Joueurs et le jeu (la carte de capture compte comme une caméra), on vérifie leurs scènes de base respectives ("Cam Joueur 1" et "Jeu"), dans la liste des scènes, et dans la liste des sources on double-clique sur la source vidéo (c'est celle qui a une icône d'appareil photo), et on fait "désactiver" puis "activer". Si ça marche toujours pas, dans la liste déroulante en haut des propriétés, on choisit un autre périphérique puis on remet l'ancien.
    - Pour la Cam joueur, le périphérique sélectionné doit terminer par "c920 ou c922
    - Pour le jeu, ça doit être Game Capture HD60S pour la carte de capture, ou "Elgato Capture x" sur le gros PC (il y en 4 différent pour le Elgato Capture, un pour chaque prise à l'arrière, n'hésitez pas à tous les tester jusqu'à tomber sur la bonne prise)
- Ensuite IMPORTANT on vérifie le son
  - Si on est sur la table de mixage, il faut avant toute chose bouger les bons sliders : d'abord, tous les mettre à 0, puis remonter les deux "Main Mix" (à droite) à fond, puis le 2ème et 3ème en partant de la gauche (qui correspondent aux 2 prises sur lesquelles on a branché les casques) presque à fond. C'est ces 2 sliders que vuos allez utiliser pour contrôler le son de chaque caster individuellement.
  - Sur le panel du son en bas de l'interface d'OBS, on voit les différentes entrées. Si la barre centrale s'anime c'est que du son est capté. Pour chacune, on clique sur les 3 points en bas, propriétés, et dans le menu déroulant on choisit le bon périphérique (ATTENTION si ça a l'air d'être déjà le bon, ouvrez quand même le menu, des fois les casques aparaissent en double) : 
    - Pour le jeu, pareil que quand on a paramétré la scène Jeu plus haut
    - Pour les casters, "USB Codec" ou un truc comme ça pour la table de mixage, "Scarlett 2i2" pour la carte son
    - Pour la régie, la marque du casque utilisé (donc en général HyperX Cloud avec notre casque habituel)
  - Une fois que les périphériques sont bien on vérifie qu'OBS entend tout le monde (comme dit plus haut faut que la barre colorée s'anime ; pour le casque régie attention à bien le demute)
  - Dans les paramèrtres, partie Audio, dans "périphérique de monitoring" on choisit bien le casque de régie (HyperX Cloud)
  - Si le casque régie n'entend pas le jeu et/ou les casters : clic droit dans la partie vide du panneau de contrôle du son, "Propriétés Audio Avancées", pour les 2 sources "Casque Casters" et "Switch" on change "Monitoring et Sortie" en "Monitoring Désactivé" PUIS on remet à "Monitoring et Sortie". On remet donc comme c'était à la base au final, c'est un bug d'OBS qui nous oblige à faire ça. Fuck OBS. Ca fait 3 ans c'est pas fix
  - Si les casters n'entendent pas la régie : clic droit sur l'entrée casque régie, filtres, dans la liste à gauche "Audio monitor", dans le menu déroulant à droite on choisit le périphérique qui correspond aux casques casters (table de mixage ou carte son). C'est d'ailleurs sur ce menu qu'on contrôle le volume sonore de la régie dans les oreilles des casters.
  - Pareil si les casters n'entendent pas le jeu

On ouvre ensuite le dossier TLSStream qui se trouve sur le bureau.

On ouvre le dossier TournamentStreamHelperTLS et on lance TSH (TSH.exe) : 

Dans TSH, cliquer sur "Set tournament", et entrer l'URL de l'event (pas le tournoi, l'event spécifiquement), qui sera toujours de forme `https://start.gg/tournament/.../events/...`.


Ensuite, si on a la tablette pour le stage strike
- on va dans l'onglet "Rules"/"Règles", et dans le dropdown tout en haut on choisit TLS. 
- dans ce même onglet en bas, il doit y avoir un URL : on ouvre firefox sur la tablette et on rentre cet URL. /!\ Le tablette doit être obligatoirement connectée au même réseau local que le PC (donc par exemple au MAD c'est leur box, le mdp est dans le channel production).

En "bonus" qui permet de bien se faciliter la vie : on lance "Vicreo listener" et "Companion" (ne pas hésiter à utiliser la barre de recherche windows), puis sur un téléphone ou une tablette on peut accéder à l'URL "http://\<IP indiquée dans l'URL du stage strike\>:8000/tablet". On a alors accès à un panneau de boutons qui permettent de contrôler toutes les fonctionnalités importantes du stream (le "Panneau Companion"). Plus bas vous trouverez une section qui explique comment gérer le stream juste avec ça, lisez quand même le reste au cas où. 

## Utilisation (pendant le tournoi) 
### Explication générales
Voir section suivante pour avoir juste la liste des chose à faire step by step, là c'est la partie explications (c'est bien d'avoir lu ça au moins une fois quand même). Lisez juste au moins la partie "OBS" ici. Les parties précédées d'un 🅰️ sont les trucs un peu "avancés" : c'est bien de les connaître mais pas besoin de les maîtriser dès le début. 


**OBS** : 
- Rappel du système / concept de base : une **Scène** est basiquement un layout, un "écran" du stream avec ses éléments et leur placement (caméras, overlay, etc). La base de la régie ça va être d'afficher la bonne scène au bon moment.
- On est en mode studio, avec preview à gauche et stream à droite ; quand on sélectionne une scène elle s'affiche à gauche, le stream voit ce qui s'affiche à droite, pour passer la scène sélectionnée en preview vers le stream il faut faire une transition. Pour ça vous pouvez utiliser les boutons transitions entre la preview et le stream 
- On a différentes transitions entre les scènes ; si vous utilsez le bouton "transition" ça fait une transi par défaut mais on peut choisir la transition qu'on utilise (je recommande mais pour le début vous embêtez pas), avec les boutons en dessous du bouton transition. En gros : 
  - Les transitions "Stinger" c'est les animations stylées avec le logo TLS ; à utiliser modérément, trop de transition cool tue la transition cool. Voir section suivante pour des indications plus précises à ce niveau là.
  - "Move" c'est une transition qui déplace les éléments, en gros à utiliser à chaque fois que vous faites pas un Stinger
  - "Cut"" c'est vraiment juste un cut, pas ouf donc mais pour afficher directement une scène cam joueurs après une game pour capturer un Pop-off ça peut être bien

- **Replays/Clip** (c'est pareil) : En règle générale, vous faites Maj+! pour le premier clip du set, et Maj+: pour les suivants (en gros, on a une playlist de clips, et Maj+! la vide puis en ajoute un)

- **Stage Strike** : pour le stage strike, en gros dès que les joueurs utilisent la tablette pour faire le stage strike, si vous cliquez sur "Stage strike" dans la liste du Downstream Keyer ça va afficher le stage strike en bas (peu importe la scène où vous êtes, vu que c'est le Downstream Keyer).

**Scènes OBS** :  
Je ne vais pas lister les scènes ici, si vous ne les connaissez pas bien le mieux c'est de toutes les regarder pour voir ce qu'elles affichent (j'ai un doute sur telle scène, je clique juste dessus pour la voir dans la preview), ou de suivre le guide en section suivante pour savoir quand mettre quoi !  Quelques scène spéciales : 
- Les scènes avec "Replay" dans le nom affichent le replay/clip (ou plus précisément, si vous avez tout lu dans la partie sur les clips, la playlist des replays).
- BracketTLS 🅰️ : affiche le bracket du top 8 uniquement, bien joli et tout, voir dans la partie TSH juste en dessous pour voir comment faire pour le bracket s'affiche bien
- TLS Bracket 🅰️ : là c'est juste une page startgg avec le bracket mais en plus joli, on ouvre le bracket sur startgg et on copie l'URL pour la coller dans les propriétés de la source navigateur présente dans cette scène (elle met du temps à bien s'afficher) ; pour scroll sur le bracket on sélectionne la source navigateur, on clique sur le bouton "Interagir" juste au dessus des sources, et on scroll (avec la molette de la souris normal)

**Utilisation de TSH**
- On va charger les matchs avec la liste qui s'ouvre en cliquant sur `Load sets from xxx` en bas. Les sets qui nous intéressent sont ceux qui ont le nom de la chaine indiqué à gauche (c'est ceux qui sont streamés) ; vous pouvez faire double clic sur la colonne "Stream" pour afficher ces sets là en haut. En général vous sélectionnez juste le premier set streamé de la liste.
- Presque tout est alors mis à jour automatiquement, il faut juste remplir manuellement : 
  - Les persos 
  - Le champ "Best of" au milieu, pour indiquer si on est en BO3 ou BO5
  - Les commentateurs : pour ça il faut aller chercher dans l'onglet "Commentary"  
Le score s'update tout seul si vous le mettez à jour sur startgg (donc faut ouvrir le set sur firefox à côté, et mettre à jour game par game au fur et à mesure du set. Sur la "fenêtre" du set startgg on
- Quand on veut afficher le bracket (Scène BracketTLS), déjà on se prépare à ce que ça fasse crash TSH, ça arrive c pas grave faut juste le relancer et remettre toutes les infos, on va dans l'onglet "arbre", dans le menu déroulant en haut à gauche on sélectionne "Top 8", on attend un peu (on ne touche surtout pas à TSH tant qu'il n'affiche pas le bracket), et normalement c'est bon

### Guide concret
Là c'est la partie à relire si vous voulez vous rafraichir un peu/avez un doute sur la marche à suivre pendant le tournoi.

**Début de stream**
- On ouvre sur la scène casters en général, jusqu'à ce que les joueurs arrivent (also j'aime bien passer sur casters + scoreboard dès que les casters demandent inévitablement qui joue en premier)

**Début de match/Avant match**
- On sélectionne le match dans TSH
- Dès que les joueurs sont là on passe sur une des scènes Trio/Duo (voir partie "Entre les games") histoire d'avoir les joueurs et les casters affichés (en général on met les joueurs en grand quand ils sont installés)
- on lance le match sur startgg, on clique sur "report game data". Pas besoin de mettre les persos pour l'instant.
- on lance l'enregistrement
- En général on essaie d'afficher la scène "Head2Head", et/ou "Result History" pour les infos, et "VSScreen Cams" un peu avant qu'ils lancent. 

**Game**
- Quand vous voyez que les joueurs sont en train de faire le ban des stages sur la tablette, vous affichez le Downstream Keyer "Stage Strike" (c'est bien avec une scène qui montre la cam joueurs 2 en grand, voire carrément de mettre la scène Cam Joueurs 2 basique).
- Dans startgg on renseigne le stage choisi. Pas besoin de mettre les persos.
- dès que la game commence on passe sur "TLS In-Game"
- On pense à prendre des clips (Maj+! pour le premier clip de la game, et si jamais y d'autres clips dans la même game Maj+: pour l'ajouter par dessus le précédent au lieu de le remaplcer)
- Quand la game se termine, si on a pris des clips on passe sur une scène avec "replay" dans le nom, par contre en cas de popoff ça peut être bien de passer (en fondu carrément pour aller vite) sur une scène avec les joueurs en grand, puis ensuite de montrer le replay. 
- On update le score en choisissant le vainqueur pour cette game, sur startgg.

**Entre les games**
- on affiche une des scènes "Trio" ou "Duo", un peu comme on veut, avec les casters en grand le plus souvent, perso j'ai une petite préférences pour les Duo (qui affichent la liste des derniers sets) mais c'est bien de changer.
- dès qu'on sait qui joue on sélectionne le match dans TSH
- Si les casters ont demandé une info sur un des trucs qu'il y a dans la liste du Downstream Keyer, ou si ils ont dit de la merde (rappel : ceux qui commencent par "DSK" c'est les slides informatives, ça inclut le poids d'un perso, fonctionnement des pikmins, etc).

**Fin de match**
- Là seulement on met les persos sur startgg, et on fait "Submit Result".
- On arrête l'enregistrement

**Entre les matchs**
- C'est un peu comme pour entre les games, on met une scène Trio/Duo
- Si on est en Top 8, c'est le moment d'afficher le BracketTLS (voir section précédente)
- si changement de caster on pense à changer le nom dans TSH
- Et puis on repart à la partie "Début de match/Avant match"

Et surtout n'oubliez pas, je vous donne des indications sur les scènes à mettre, et si vous suivez mes indications normalement vous avez un stream propre, mais au final c'est à vous de juger quelle scène vous voulez mettre (hors des games en tout cas). Dans les scènes Duo/Trio mettez les casters en grand ou les joueurs en grand en fonction de ce qui vous paraît + intéressant / vivant sur le moment, et quand y a rien d'autre que les casters qui bouge on peut mettre la scène avec juste les casters, des fois le VSScreen Cams a la bonne vibe et des fois moins, bref.

## Première installation

### Résumé
- Insaller OBS
- Clone le repo
- Install plugins OBS
  - Move transition
  - Audio Monitor
  - Downstream Keyer
- Install autres : 
  - VLC
  - Elgato Capture au cas où
  - Companion
  - Vicreo
- Install fonts (dans Assets/common/Font)
- Dans OBS
  - Importer collection (TLS.json)
  - Charger le dock ALT
- DL assets TSH

### Version longue

On commencer par installer OBS.

La plupart des fichiers nécessaires sont contenus sur un dépôt github. 2 solutions pour le récupérer : 
- Solution simple qui ne permet pas de mettre à jour par la suite (je recommande donc la 2ème, néamoins plus complexe) : télécharger directement [à cette URL](https://github.com/TwilCynder/TLSStream/archive/refs/heads/main.zip), et extraire l'archive dans le dossier "C:\Stream". Il est important de le placer ici pour grandement simplifier la suite.
- Solution recommandée pour un PC qui va servir plus d'une fois, mais qui nécessite Git : 
  - installer [Git](https://www.git-scm.com/downloads) (garder les options par défaut sur l'installeur)
  - Créer un dossier "C:\Stream"
  - Clic droit sur ce dossier dans l'explorateur de fichiers (maj + clic droit sur l'horrible windows 11) -> "Open Git Bash Here"
  - Dans le terminal qui s'ouvre, taper : `git clone https://github.com/TwilCynder/TLSStream --recurse-submodules`. 
  - Le téléchargement se lance (~5Go)

Installer également : 
- Plugins OBS (Sur leur page de téléchargement choisir la version "windows-installer.zip", et lancer l'exécutable qui se trouve dans l'archive)
  - [Move Transition](https://obsproject.com/forum/resources/move.913/)
  - [Audio monitor](https://obsproject.com/forum/resources/audio-monitor.1186/)
  - [Downstream Keyer](https://obsproject.com/forum/resources/downstream-keyer.1254/)
- VLC Media Player
- Elgato capture utility

Installations optionnelles : 
- Bitfocus companion
- Vicreo listener

On installe les polices de caractère à partir des fichiers qui se trouvent dans "C:\Stream\TLSStream\Assets\common\Font\"

On lance OBS, et on importe et charge une collection de scène depuis "C:/Stream/TLSStream/Scenes/TLS.json". OBS va se plaindre qu'il manque des fichiers, mais si TLSStream a bien été placé dans "C:/Stream" ça ne devrait pas être un problème. 

Dans le menu "Docks" -> "Docks Internet personnalisés", on clique sur les 3 points, sélectionner le fichier "C:\Stream\TLSStream\tools\Animated-Lower-Thirds\lower thirds\control-panel.html"

On lance ensuite TSH ; clic sur l'icône de menu en haut à droite -> "download assets", dans la fenêtre qui s'ouvre on sélectionne SSBU dans la liste des jeux (utiliser la barre de rechercher en haut), puis on télécharge les assets "base" et "mural"