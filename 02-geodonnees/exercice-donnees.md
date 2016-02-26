# Exercice 1: sources de données spatiales

L'exercice consiste en la préparation d'un fond de carte des régions riveraines du Léman. Le maillage spatial choisi est celui des communes, avec une couche supplémentaire contenant les limites des régions (cantons, département). Concrètement, il s'agit de  produire 3 couches vectorielles, sous forme de fichiers Shape:

* Une couche (une seule couche!) des communes des cantons du Valais, Vaud et Genève, ainsi que du Département de la Haute-Savoie en France. La couche doit avoir comme système de référence spatial les coordonnées suisses CH1903 (EPSG:21781).

* Une deuxième couche qui contient les limites des cantons resp. du département. Cette couche doit être générée à partir de la couche des communes.

* Une troisième couche séparée doit contenir le Léman, ainsi que d'éventuels autres lacs. Les deux premières couches ne doivent pas contenir de lac.

A ce stade, il ne faut pas faire attention aux attributs des couches. Il y aura aussi beaucoup d'imprécisions le long de la frontière entre la France et la Suisse; pas besoin de régler ce problème pour l'instant.

En plus, vous avez été informés que les communes suivantes ont fusionnées, et qu'il faut tenir compte de ces fusions:

* les communes vaudoises de Blonay et Saint-Légier-La-Chiésaz ont fusionné dans une nouvelle commune de nom *«Ognonnaz»*, du nom de la rivière qui les séparait.

* la commune française de Saint-Gingolph a fusionné avec la commune valaisanne de Saint-Gingolph, dans une nouvelle commune de nom *«New Saint-Gingolph»*. Faites attention qu'il n'y ait aucun «trou» à l'intérieur de la commune.

Les étapes nécessaires pour réaliser cet exercice sont détaillées dans les vidéos ci-dessous. L'ensemble du processus est effectué avec Quantum GIS. A vous de trouver les géodonnées de base!

Si vous voulez une correction de l'exercice, veuillez rendre par mail une archive ZIP contenant l'ensemble des couches.




## Tutoriels

* Tutoriels déjà vu au cours de Cartographie:
	* [QGIS Tutorial #1: Installation sur Windows](https://www.youtube.com/watch?v=-7tnnMc9UXU&index=1&list=PLbjixabFMUzPgm8VFyBUP7fs9DRBNEbsw)
	* [QGIS Tutorial #2: Installation sous Mac OS X](https://www.youtube.com/watch?v=5In21hlXo8k&index=2&list=PLbjixabFMUzPgm8VFyBUP7fs9DRBNEbsw)
	* [QGIS Tutorial #3: l'interface](https://www.youtube.com/watch?v=GGh63wACrTw&list=PLbjixabFMUzPgm8VFyBUP7fs9DRBNEbsw&index=3)
	* [QGIS Tutorial #4: Couches vectorielles](https://www.youtube.com/watch?v=kdaqJUGqJy0&index=4&list=PLbjixabFMUzPgm8VFyBUP7fs9DRBNEbsw)
	* [QGIS Tutorial #5: Couches raster](https://www.youtube.com/watch?v=E1X_cQQ22Vw&list=PLbjixabFMUzPgm8VFyBUP7fs9DRBNEbsw&index=5)
	* [QGIS Tutorial #6: Projections](https://www.youtube.com/watch?v=IcLHgdCyeSg&index=6&list=PLbjixabFMUzPgm8VFyBUP7fs9DRBNEbsw)

* Tutoriels par rapport à cet exercice:
	* [QGIS Tutorial #8: Projections 2](https://www.youtube.com/watch?v=ACfCxfA92kY&index=8&list=PLbjixabFMUzPgm8VFyBUP7fs9DRBNEbsw)
	* [QGIS Tutorial #9: Exporter une partie d'une couche vectorielle](https://www.youtube.com/watch?v=D5p_sZtLLuA&index=9&list=PLbjixabFMUzPgm8VFyBUP7fs9DRBNEbsw)
	* [QGIS Tutorial #10: Opération géométrique Dissolve/Regrouper](https://www.youtube.com/watch?v=s1JtQ4aZJOk&index=10&list=PLbjixabFMUzPgm8VFyBUP7fs9DRBNEbsw)
	* [QGIS Tutorial #11: Fusionner deux couches vectorielles](https://www.youtube.com/watch?v=VOJs_XJ5ocI&index=11&list=PLbjixabFMUzPgm8VFyBUP7fs9DRBNEbsw)
	* [QGIS Tutorial #12: Copier-coller des géométries d'une couche à l'autre](https://www.youtube.com/watch?v=UqvXahonVSE&index=12&list=PLbjixabFMUzPgm8VFyBUP7fs9DRBNEbsw)
	* [QGIS Tutorial #13: Fusionner des polygones en mode édition](https://www.youtube.com/watch?v=HS7yE20IPAU&index=13&list=PLbjixabFMUzPgm8VFyBUP7fs9DRBNEbsw)
	* [QGIS Tutorial #14: Editer des polygones complexes](https://www.youtube.com/watch?v=5eo5ZFy5Jek&index=14&list=PLbjixabFMUzPgm8VFyBUP7fs9DRBNEbsw)

* [Ensemble des tutoriels QGIS](https://www.youtube.com/playlist?list=PLbjixabFMUzPgm8VFyBUP7fs9DRBNEbsw)

