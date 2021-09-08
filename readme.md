#CuffelThomas_3_10082021

__Réalisation du projet 3 parcours Dev Web OpenClassRooms__

"Dynamisez une page web avec des animations CSS"

__Scénario__
-----------------

Vous venez d’être recruté chez Ohmyfood!, en tant que développeur junior. Félicitations !

Ohmyfood! est une jeune startup qui voudrait s'imposer sur le marché de la restauration. L'objectif est de développer un site 100% mobile qui répertorie les menus de restaurants gastronomiques. En plus des systèmes classiques de réservation, les clients pourront composer le menu de leur repas pour que les plats soient prêts à leur arrivée. Finis, les temps d'attente au restaurant !

__Fonctionnalités__
-----------------

* Le développement devra se faire en CSS, sans JavaScript.
* Aucun framework ne devra être utilisé, en revanche l’utilisation de SASS serait un plus.
* Aucun code CSS ne devra être appliqué via un attribut style dans une balise HTML.
* L’ensemble du site devra être responsive sur mobile, tablette et desktop.
* Les pages devront passer la validation W3C en HTML et CSS sans erreur.
* Le site doit être parfaitement compatible avec les dernières versions desktop de Chrome et Firefox.

__Livrables attendus__
-----------------

Page d’accueil (x1) 
* Affichage de la localisation des restaurants. À terme il sera possible de choisir sa 
localisation pour trouver des restaurants proches d’un certain lieu. 
*Une courte présentation de l’entreprise. 
* Une section contenant les 4 menus sous forme cartes. Au clic sur la carte, 
l’utilisateur est redirigé vers la page du menu.  
 
Pages de menu (x4) 
* 4 pages contenant chacune le menu d’un restaurant. 
 
 
Footer 
* Le footer est identique sur toutes les pages. 
* Au clic sur “Contact”, un renvoi vers une adresse mail est effectué. 
 
Header 
* Le header est présent sur toutes les pages. 
* Sur la page d’accueil, il contient le logo du site. 
* Sur les pages de menu, il contient en plus un bouton de retour vers la page d’accueil 

__Identité graphique__
-----------------

Polices Logo et titres: Shrikhand  
Texte: Roboto  
Couleurs:  
* Primaire: #9356DC
* Secondaire: #FF79DA
* Tertiaire: #99E2D0


__Effets graphiques et animations__
-----------------

* Les effets accessibles au clic ou au survol sont visibles sur la maquette. Ils devront utiliser 
les animations ou transitions CSS, pas de JavaScript ni de librairie. 
 
Boutons :
* Au survol, la couleur de fond des boutons principaux devra légèrement s’éclaircir. 
L’ombre portée devra également être plus visible.  
* À terme, les visiteurs pourront sauvegarder leurs menus préférés. Pour ça, un 
bouton "J’aime" en forme de cœur est présent sur la maquette. Au clic, il devra se 
remplir progressivement. Pour cette première version, l’effet peut être apparaître au 
survol sur desktop au lieu du clic. 
 
Page d’accueil :
* Quand l’application aura plus de menus, un “loading spinner” sera nécessaire. Sur 
cette maquette, nous souhaitons en avoir un aperçu. Il devra apparaître pendant 1 à 
3 secondes quand on arrive sur la page d'accueil, couvrir l'intégralité de l'écran, et 
utiliser les animations CSS (pas de librairie). Le design de ce loader n’est pas défini, 
toute proposition est donc la bienvenue tant qu’elle est cohérente avec la charte 
graphique du site. 
 
Pages de menu :
* À l’arrivée sur la page, les plats devront apparaître progressivement avec un léger 
décalage dans le temps. Ils pourront soit apparaître un par un, soit par groupe 
“Entrée”, “Plat” et “Dessert”. Un exemple de l’effet attendu est fourni. 
*Le visiteur peut ajouter les plats qu'il souhaite à sa commande en cliquant dessus. 
Cela fait apparaître une petite coche à droite du plat. Cette coche devra coulisser de 
la droite vers la gauche. Pour cette première version, l’effet peut apparaître au survol 
sur desktop au lieu du clic. Si l’intitulé du plat est trop long, il devra être rogné avec 
des points de suspension. Un exemple de l’effet attendu est fourni. 

__Installation SASS__
-----------------

Pour installer Sass, vous allez avoir besoin d’installer NodeJS. 

### 1. Installez NodeJS sur votre ordinateur

Rendez-vous sur la page d’installation de NodeJS et téléchargez la LTS

Une fois l’installation terminée, je vous invite à lancer l’invite de commandes windows :
  
  Entrez la commande: `node -v` puis la commande `npm -v`

> Ces deux commandes vous permettront de vérifier si :
> Node et Npm est bien installé et de connaitre sa version.

### 2. Vous pouvez maintenant installer Sass 

Avec la commande  `npm -g install sass` 

Pour vérifier que vous avez bien installé Sass dans votre système, tapez " `sass --version` " dans le terminal.

### 3. Vous avez installé Sass, maintenant comment est-ce qu’on le fait fonctionner ?

Grâce au ficher package.json crée au préalable pour ce projet, vous pouvez voir dans le fichier un script :
  > "sass": "sass --watch sass/main.scss:public/css/style.css -w --style expanded"

Dans le terminal, tapez  `npm run sass` 

Ça y est, vous êtes fin prêt !
Tant que vous n’interrompez pas le processus, soit en tapant Ctrl+C dans le terminal, soit en cliquant sur la corbeille,
le script attendra et sera à l'affût de tout changement à compiler.
