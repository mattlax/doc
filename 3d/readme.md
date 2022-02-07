# Mise en oeuvre de Itowns, un outil Javascript ! 

![image](/3d/media/Image1.png "Title")

---

## 1. Mais qu'est-ce que Itowns? 

Itowns c’est…
  - un framework web écrit en Javascript/WebGL
  - un outil de visualisation de données géographiques en 3D

Qui en est à l’initiative ? 
  - IGN/Oslandia

![image](/3d/media/Image2.png "Title")
![image](/3d/media/Image3.png "Title")

## 2. Comment l'installer? Deux méthodes pour le même résultat.
### Installer avec  node.js 

 - ouvrez node.js et tapez
 - npm install --save itowns
 - Node.js télécharge le dossier dans nodemodules sur votre ordinateur
 - récupérez les fichiers itowns.js, LoadingScreen.js, GuiTools.js et LoadingScreen.css, copiez les dans le répertoire voulu.
 - Faites appel à ces fichiers dans votre projet !

![image](/3d/media/Image4.png "Title")

### Installer avec Github
 - Étapes d’installations avec Github  : 
 - Aller sur le projet github, 
 - Dans iTowns/itowns/releases/tag 
 - Télécharger la dernière version qui est en .zip

![image](/3d/media/Image5.png "Title")

# Exemples de rendu Itowns
![image](/3d/media/Image6.png "Title")

* * *
# 3. Créer une vue en 2,5d avec Itowns, tuto !

### Étape 1 : Elle consiste à créer le fichier HTML, reliant entre eux les fichiers sources et les fichiers du projet. 
![image](/3d/media/Image7.png "Title")

### Étape 2 : Vient ensuite l'ajout de légende qui rappelle les commandes (optionnel !).
![image](/3d/media/Image8.png "Title")

### Étape 3 : Enfin, on fait les liens vers les fichiers principaux.
*C'est ici que les fichiers itowns.js, LoadingScreen.js, GuiTools.js et LoadingScreen.css sont chargés !* 
![image](/3d/media/Image9.png "Title")

### Étape 4 : Il est temps de créer la vue voulue ! 
![image](/3d/media/Image10.png "Title")

#### La vue obtenue est la suivante. Sympa non? 
![image](/3d/media/Image11.png "Title")

### Étape 5 : Créer une vue c'est bien, montrer quelque chose c'est mieux ! Ajoutons un fond de carte satellite, obtenu via WMS. 
*Source wms de data.grandlyon*
Il y a une logique de création de la source (en premier, sans affichage) et l'affichage/paramétrage du layer.
![image](/3d/media/Image12.png "Title")

Les données (geojson et autres) sont directement appelées dans le Javascript, ce qui en fait une logistique plus pratique que Leaflet par exemple.

#### Le rendu est déjà plus sympa non? Mais il manque quelque chose... 
![image](/3d/media/Image13.png "Title")

#### C'est tout plat !  
![image](/3d/media/Image14.png "Title")

### Étape 6 : Il faut ajouter un peu de relief à tout ça.
*Ici il s'agit d'une source WMS de Data grand Lyon.* 
![image](/3d/media/Image15.png "Title")
#### C'est beau? 
![image](/3d/media/Image16.png "Title")

![image](/3d/media/Image17.png "Title")

