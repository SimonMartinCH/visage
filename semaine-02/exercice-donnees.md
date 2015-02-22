# Exercice 1: sources de données spatiales

L'exercice consiste en la préparation d'un fond de carte des régions riveraines du Léman. Le maillage spatial choisi est celui des communes, avec une couche supplémentaire contenant les limites des régions (cantons, département). Concrètement, il s'agit de  produire 3 couches vectorielles, sous forme de fichiers Shape:

* Une couche (une seule couche!) des communes des cantons du Valais, Vaud et Genève, ainsi que du Département de la Haute-Savoie en France. La couche doit avoir comme système de référence spatial les coordonnées suisses CH1903 (EPSG:21781).

* Une deuxième couche qui contient les limites des cantons resp. du département. Cette couche doit être générée à partir de la couche des communes.

* Une troisième couche séparée doit contient le Léman, ainsi que d'éventuels autres lacs. Les deux premières couches ne doivent pas contenir de lac.

A ce stade, il ne faut pas faire attention aux attributs des couches. Il y aura aussi beaucoup d'imprécisions le long de la frontière entre la France et la Suisse; pas besoin de régler ce problème pour l'instant.

En plus, vous avez été informés que les communes suivantes ont fusionnées, et qu'il faut tenir compte de ces fusions:

* les communes vaudoises de Blonay et Saint-Légier-La-Chiésaz ont fusionné dans une nouvelle commune de nom *«Beau-coin-au-dessus-de-Vevey»*

* la commune française de Saint-Gingolph a fusionné avec la commune valaisanne de Saint-Gingolph, dans une nouvelle commune de nom *«New Saint-Gingolph»*. Faites attention qu'il n'y a pas de «trou» à l'intérieur de la commune.

Si vous voulez une correction de l'exercice, veuillez rendre par mail une archive ZIP contenant l'ensemble des couches.