# Tuto stream TLS

## Installation (au début du tournoi)

### Physique

Pour trouver rapidement le matériel : tous les câbles sont dans la valise noire, tous les appareils / boites sont dans la valide grise.  
Les câbles vidéo/audio et les autres dans des compartiments différents dans la valise. Les câbles HDMI ont des scratchs gris, les rallonges USB des scratchs verts

Note : je pars du principe qu'on utilise la table de mixage, mais on peut aussi utiliser la carte son (scarlett 2i2), ça ne fait pas bcp de différence  

/!\ Si vous faites le rangement, lisez bien la partie dédiée plus bas svp !

La première chose à faire est le choix du PC. Pour rappel, on a 2 PC fixes, dont un petit et très facile à transporter (boite orange dans la valise grise) et une grosse tour (rangée dans son carton). Je recommande la tour car elle marche simplement mieux, mais si vous vous sentez pas de la bouger (elle pèse un peu), le petit PC marche.


- On commence par installer les tables
  - Au MAD, c'est une petite table devant le canapé des casters, une grande juste derrière pour les joueurs, une grande table sur le côté du canapé pour la régie, et une petite entre régie et joueurs (pour la table de mixage)
- On amène l'électricité au setup régie, au MAD on fait passer une rallonge avec enrouleur derrière les canapés. 
- On sort le PC, et on branche son alim (pour le petit elle se trouve dans la valide grise, c'est le *gros* transfo)
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
- On branche le cable ethernet de la box au PC. En général il vaut mieux utiliser le gros enrouleur rouge. Au MAD, on fait passer le câble derrière les canapés. 
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
  - Si on est sur la table de mixage, il faut avant toute chose bouger les bons sliders : d'abord, tous les mettre à 0, puis remonter les deux "Main Mix" (à droite) à fond, puis le 2ème et 3ème en partant de la gauche (qui correspondent aux 2 prises sur lesquelles on a branché les casques) presque à fond. C'est ces 2 sliders que vous allez utiliser pour contrôler le son de chaque caster individuellement. Ensuite on vérifie que les boutons "main" à côté des sliders en question sont enfoncés.
  - Sur le panel du son en bas de l'interface d'OBS, on voit les différentes entrées. Si la barre centrale s'anime c'est que du son est capté. Pour chacune, on clique sur les 3 points en bas, propriétés, et dans le menu déroulant on choisit le bon périphérique (ATTENTION si ça a l'air d'être déjà le bon, ouvrez quand même le menu, des fois les casques aparaissent en double) : 
    - Pour le jeu, pareil que quand on a paramétré la scène Jeu plus haut
    - Pour les casters, "USB Codec" ou un truc comme ça pour la table de mixage, "Scarlett 2i2" pour la carte son
    - Pour la régie, la marque du casque utilisé (donc en général HyperX Cloud avec notre casque habituel)
  - Une fois que les périphériques sont bien on vérifie qu'OBS entend tout le monde (comme dit plus haut faut que la barre colorée s'anime ; pour le casque régie attention à bien le demute)
  - Dans les paramèrtres, partie Audio, dans "périphérique de monitoring" on choisit bien le casque de régie (HyperX Cloud)
  - Si le casque régie n'entend pas le jeu et/ou les casters : clic droit dans la partie vide du panneau de contrôle du son, "Propriétés Audio Avancées", pour les 2 sources "Casque Casters" et "Switch" on change "Monitoring et Sortie" en "Monitoring Désactivé" PUIS on remet à "Monitoring et Sortie". On remet donc comme c'était à la base au final, c'est un bug d'OBS qui nous oblige à faire ça. Fuck OBS. Ca fait 3 ans c'est pas fix
  - Si les casters n'entendent pas la régie : clic droit sur l'entrée casque régie, filtres, dans la liste à gauche "Audio monitor", dans le menu déroulant à droite on choisit le périphérique qui correspond aux casques casters (table de mixage ou carte son). C'est d'ailleurs sur ce menu qu'on contrôle le volume sonore de la régie dans les oreilles des casters.
  - Pareil si les casters n'entendent pas le jeu
- Dans les boutons en bas a droite, on clique sur "Démarrer le tampon de relecture". Notez juste à côté les boutons "Démarrer l'enregistrement" et "Démarrer le streaming" qu'il faudra évidemment utiliser.

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
- Pour lancer le steam, c'est le bouton en bas à droite d'OBS, pareil pour l'enregistrement. On lance l'enregistrement en même temps que le stream, et on le cut à la fin, de manière à avoir une seule grosse vidéo.
- On est en mode studio, avec preview à gauche et stream à droite ; quand on sélectionne une scène elle s'affiche à gauche, le stream voit ce qui s'affiche à droite, pour passer la scène sélectionnée en preview vers le stream il faut faire une transition. Pour ça vous pouvez utiliser les boutons transitions entre la preview et le stream 
- On a différentes transitions entre les scènes ; si vous utilsez le bouton "transition" ça fait une transi par défaut mais on peut choisir la transition qu'on utilise (je recommande mais pour le début vous embêtez pas), avec les boutons en dessous du bouton transition. En gros : 
  - Les transitions "Stinger" c'est les animations stylées avec le logo TLS ; à utiliser modérément, trop de transition cool tue la transition cool. 
  - "Move" c'est une transition smooth, à utiliser quand vous utilisez pas le stinger (surtout entre 2 scènes similaires)
  - "Cut"" c'est vraiment juste un cut, pas ouf donc mais pour afficher directement une scène cam joueurs après une game pour capturer un Pop-off ça peut être bien


- **Replays/Clip** (c'est pareil) : En règle générale, vous faites Maj+! pour le premier clip du set, et Maj+: pour les suivants (en gros, on a une playlist de clips, et Maj+! la vide puis en ajoute un)

- **Stage Strike** : pour le stage strike, en gros dès que les joueurs utilisent la tablette pour faire le stage strike, les stages vont s'afficher sur la scène "VS Screen Cam Stage Strike". 🅰️ Vous pouvez aussi utiliser le DSK Stages (voir partie DSK)

**Scènes OBS** :  
Je ne vais pas lister les scènes ici, si vous ne les connaissez pas bien le mieux c'est de toutes les regarder pour voir ce qu'elles affichent (j'ai un doute sur telle scène, je clique juste dessus pour la voir dans la preview), ou de suivre le guide en section suivante pour savoir quand mettre quoi !  
En résumé : 
- TLS In Game affiche le jeu (a toujours mettre pendant les games)
- Les scenes Trio et Duo affichent plusieurs sources (jeu, cams) en même temps
- Les scènes avec "Replay" dans le nom affichent les replay/clips sauvegardés 
- BracketTLS 🅰️ : affiche le bracket du top 8/16 uniquement, doit d'abord être configuré dans TSH
- Du reste, les noms des scènes sont plutot explicites
- La scène Timer contient un timer qu'il faut configurer manuellement, voir plus bas
- Les scènes situées apres la scène "==== SOURCES" ne sont pas a utiliser

**Utilisation de TSH**
- On va charger les matchs avec la liste qui s'ouvre en cliquant sur `Load sets from xxx` en bas. Les sets qui nous intéressent sont ceux qui ont le nom de la chaine indiqué à gauche (c'est ceux qui sont streamés) ; vous pouvez faire double clic sur la colonne "Stream" pour afficher ces sets là en haut. En général vous sélectionnez juste le premier set streamé de la liste.
- Presque tout est alors mis à jour automatiquement, il faut juste remplir manuellement : 
  - Le champ "Best of" au milieu, pour indiquer si on est en BO3 ou BO5
  - Les commentateurs : pour ça il faut aller chercher dans l'onglet "Commentary"  
Le score s'update tout seul si vous le mettez à jour sur startgg (donc faut ouvrir le set sur firefox à côté, et mettre à jour game par game au fur et à mesure du set)
- Quand on veut afficher le bracket (Scène BracketTLS), déjà on se prépare à ce que ça fasse crash TSH, ça arrive c pas grave faut juste le relancer et remettre toutes les infos, on va dans l'onglet "arbre", dans le menu déroulant en haut à gauche on sélectionne "Top 8\16", puis dans le menu deroulant juste a droite on selectionne "Poule 1" (c'est normal qu'il n'y ait que cette option dans la liste), puis on attend ; TSH va freeze un peu, puis le bracket s'affiche a droite (ne surtout pas cliquer sur tsh tant qu'il n'a pas fini d'afficher le bracket, risque de crash). A  e moment là on peut afficher la scène bracket dans OBS

**Timer** : pour configurer le timer de la scène Timer, dans Outils (barre en haut d'OBS) -> Scripts, choisir "countdown.lua" et rentrer le nombre de minutes a droite de la fenêtre 
u
🅰️ **DSK (DownStream Keyer)** : un système permettant d'afficher qque chose par dessus la scène actuelle, peu importe sur quelle scène on est. Il se contrôle dans le panneau en bas à droite (c'est un petit panneau avec plusieurs onglets), qui affiche une liste d'éléments à afficher. On y trouve notament "DSK Stages", qui affiche le stage strike. Pour afficher un des éléments, vous pouvez simplemnt le sélectioner dans la liste ; pour l'enlever, cliquer sur l'icône Pause en bas du panneau. Attention, le DSK s'affiche toujours directement sur le programme. 

### Deroulement du stream

**Début de stream**
- On **lance le stream et l'enregistrement (boutons en bas à droite)** sur la scène Timer. Penser a configurer le timer avant (voir plus haut)
- A la fin du timer, on peut afficher la scène "Intro TLS" (elle affiche une vidéo, ca se voit pas dans la preview), c'est optionel
- Puis on ouvre sur la scène casters en général, jusqu'à ce que les joueurs arrivent (also j'aime bien passer sur "casters + scoreboard" dès que les casters demandent inévitablement qui joue en premier)

**Début de match/Avant match**
- On sélectionne le match dans TSH
- Dès que les joueurs sont là on passe sur une des scènes Trio/Duo (voir partie "Entre les games") histoire d'avoir les joueurs et les casters affichés (en général on met les joueurs en grand quand ils sont installés)
- on lance le match sur startgg, on clique sur "report game data". Pas besoin de mettre les persos pour l'instant.
- En général on essaie d'afficher la scène "Head2Head", "Result History" et/ou Current Run (pas pertinentau début du tournoi) pour les infos, et "VSScreen Cams" un peu avant qu'ils lancent. 

**Game**
- Quand vous voyez que les joueurs sont en train de faire le ban des stages sur la tablette, vous affichez la scène "VS Screen Cams Stage Strike" (🅰️ ou le DSK Stages)
- Dans startgg on renseigne le stage choisi. Pas besoin de mettre les persos.
- dès que la game commence on passe sur "TLS In-Game"
- On pense à prendre des clips (Maj+! pour le premier clip du match, Maj+: pour les suivants)  
- Quand la game se termine, si on sent venir un popoff on cut directement sur VS Screen Cams
- On update le score en reportant la game sur startgg (penser à faire "Save Progress" pour save, pas "Submit Result")

**Entre les games**
- on affiche une des scènes "Trio" ou "Duo", un peu comme on veut, perso j'ai une petite préférences pour les Duo (qui affichent la liste des derniers sets) mais c'est bien de changer.

**Fin de match**
- Là seulement on met les persos sur startgg, et on fait "Submit Result".

**Entre les matchs**
- C'est un peu comme pour entre les games, on met une scène Trio/Duo
- Si on est en Top 8, c'est le moment d'afficher le BracketTLS (voir section précédente)
- si changement de caster on pense à changer le nom dans TSH
- Et puis on repart à la partie "Début de match/Avant match"

**Fin du stream** 
- Une fois la GF finie, on peut passer sur la scène Casters pour les laisser clore le stream (après une éventuelle interview), puis on passe sur la scène fin, on coupe le record, puis on attend un peu avant de couper le stream. 
- On branche le SSD TLS au PC (demander aux TO qui l'a), et on y copie la la vidéo enregistrée, qui se trouve dans le dossier Vidéos. 

Et surtout n'oubliez pas, je vous donne des indications sur les scènes à mettre, et si vous suivez mes indications normalement vous avez un stream propre, mais au final c'est à vous de juger quelle scène vous voulez mettre (hors des games en tout cas). Dans les scènes Duo/Trio mettez les casters en grand ou les joueurs en grand en fonction de ce qui vous paraît + intéressant / vivant sur le moment, et quand y a rien d'autre que les casters qui bouge on peut mettre la scène avec juste les casters, des fois le VSScreen Cams a la bonne vibe et des fois moins, bref.

### Utiliser Companion
Companion est un logiciel optionnel qui permet d'afficher un tableau de boutons permettant de contrôler la plupart des éléments de la régie.

Après l'avoir lancé, une petite fenêtre rouge apparaît. Dans le menu dropdown marqué "Change network interfaces", sélectionner "0.0.0.0 / All Interfaces".

![alt text](./assets-guide/companion%20window.png)

On va ensuite récupérer l'IP du PC, pour ça le plus simple est d'aller voir l'URL en bas de l'onglet "Règles / Rules" dans TSH et repérer l'IP entre le "http://" et le ":5000" (4 nombres séparés par des points).  
On va aller à l'URL suivante : `http://IpDuPC:8000/button`.  

Une fois la page ouvert on devrait avoir une grande grille de boutons, qui permettent de contrôler un peu tout le stream :
- Les boutons "score" changent le score. Attention, si on utilise ça au lieu de changer le score via startgg directement, il faut préciser aux joueurs d'aller report eux mêmes à la fin. 
- Les boutons avec des noms de scène OBS (vert/noir/orange) affichent cette scène directement.
- Les boutons gris permettent de contrôler les replays (rappel : on les affiche en mettant une scène qui a "Replay" dans le nom)
- 🅰️ Les boutons Jaunes contrôlent le DSK


### Rangement
En soi il n'y a rien à savoir de plus si vous connaissez déjà la procédure pour l'installation, on va juste tout remettre comme avant. 
- De manière générale les alims des apareils restent avec les appareils en question. Toutes les boites peuvent se ranger sans forcer.
  - La table de mixage se range avec son câble USB (en plus de l'alim). Pareil pour la carte son
  - Le casque régie hyper X se range avec sa clé USB, penser à détacher le micro avant de mettre dans la boite
  - L'ampli des joueurs se range avec son câble jack en plus de l'alim
  - Le petit PC se range SANS son alim (le gros transfo) qui va dans la valise des câbles
- Pour le gros PC, faites y vraiment gaffe svp, les cadres en mousse vont en haut et en bas, le PC se met avec l'avant en bas dans le carton
- Pour les casques : on dévisse la vis près du câble, on retire le câble, puis on range dans les housses. La vis va dans la poche au fond de la housse, le câble s'enroule au centre. On range le splitter jack avec un des 2 casques.
- Pour tous les câbles qui ne sont pas avec un appareil en particulier (câbles HDMI/DP, rallonges USB, etc) c'est direction la valise noire : le compartiment très rempli c'est pour les câbles audio/vidéo, l'autre c'est pour le reste (USB, etc). Pensez bien à ENROULER TOUS LES CABLES, ils ont des scratchs qui vous permettent de les maintenir enroulés. Avant de fermer la valise, veiller à ce que les câbles ne soient pas trop en tas, que la valise puisse bien fermer.
- Dans le sac régie (le sac carrefour avec marqué "Régie"), on met les housses des casques, puis les claviers, puis les souris
- Les cams vont dans une des boites transparentes
- Toutes les boites vont dans la valise grise. Pour pouvoir la fermer sans forcer (ne faites pas ça!!!!) il faut un peu d'organisation : y a un exemple dans les épinglés du channel production


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