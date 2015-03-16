# Exercice: carte choroplèthe avec QGIS


# Objectif

Créer une carte choroplèthe dans QGIS et la terminer dans Illustrator.

Concrètement, l'exercice consiste en:

- Faire une carte choroplèthe d'un des indicateurs pour votre dossier pratique. Pour des fins d'illustration, nous avons choisi de faire une carte de l'évolution des familles monoparentales dans quelques communes du canton de Vaud, mais vous êtes libres de choisir ce que vous voulez.

- Pour la cartographie d'une évolution, il faut faire une légende bi-colore, avec une classification de Jenks en 2 temps (valeurs positives et négatives séparément)

- Palette de couleurs appropriée (consultez [Colorbrewer](http://colorbrewer2.org/), les couleurs proposées par QGIS ne sont pas toujours optimales)

- Dans le cas de la région lausannoise, évidemment inclure le lac dans la carte

- Ajouter également échelle, titre, source de données, labels si nécessaires, ...

- Soyez esthétiques


Attention aux données manquantes. QGIS a tendance de simplement ignorer ces communes, mais il faut les afficher typiquement avec une couleur de gris clair sur la carte ainsi que dans la légende.


Les [tutoriels vidéo de création de cartes choroplèthes avec QGIS](https://www.youtube.com/playlist?list=PLbjixabFMUzNNbpkTFE_c_Q9b4o2qAepS) vous guide à travers les étapes nécessaires pour créer votre carte.



## Données

Pour ceux qui veulent faire l'exercice avec l'évolution des familles monoparentales entre 1970 et 2000 autour de Lausanne, le fichier contenant les données est fourni (`exercice-choroplethe-qgis-data-famo.txt`). Les données peuvent facilement être téléchargées directement depuis [l'atlas statistique du canton de Vaud](http://www.scris.vd.ch/Default.aspx?DomId=2091), établi par Statistique Vaud. La source des données est le Recensement fédéral de la population de 1970 et 2000, de [l'Office fédéral de la statistique (OFS)](http://www.bfs.admin.ch/bfs/portal/fr/index.html/).

Les limites des communes peuvent être obtenues à différents endroits:

- [ThemaKart de l'OFS](http://www.bfs.admin.ch/bfs/portal/fr/index/regionen/thematische_karten/01/02.html) est un jeu de géométries de base pour la cartographie thématique. Probablement le meilleur jeu de données disponible en vue de l'exercice, car assez généralisé, mais malheureusement payant.
- [Limites communales généralisées Geostat de l'OFS](http://www.bfs.admin.ch/bfs/portal/fr/index/dienstleistungen/geostat/datenbeschreibung/generalisierte_gemeindegrenzen.html). Meilleur jeu de données gratuit en vue de l'exercice.
- [Swisstopo, données swissBOUNDARIES3D](http://www.swisstopo.admin.ch/internet/swisstopo/fr/home/products/landscape/swissBOUNDARIES3D.html)
- [Swiss Maps sur GitHub](https://github.com/interactivethings/swiss-maps) (ce sont des données Swisstopo à l'origine)


