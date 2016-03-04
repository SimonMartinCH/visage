# Exercice 2: sources de données spatiales

---

* Buts de l'exercice 2:
	* Création d’une base de données spatiale
	* Calcul d’attributs
	* Jointure (par attribut et spatiale)

---


Préparez un fond de carte complet avec plusieurs attributs pour la liste des communes vaudoises se trouvant dans le fichier `communes_vd.csv` (tuto #15). L'état des communes est celui de 2012. Comme fond de carte, utilisez la couche simplifiée du K4 de l'Office fédéral de la statistique (section ThemaKart).

Vous devez y joindre les attributs suivants (tuto #16 et 17):
* Géocode de l'OFS et nom de la commune
* Population résidante permanente des années 2000, 2005, 2010, 2012 (noms des attributs: *pop2000, pop2005, pop2010, pop2012*)
* Nombre de personnes de nationalité française, en 2012 (nom de l'attribut: *fr2012*)
* Pourcentage de personnes de nationalité française, en 2012 (nom de l'attribut: *pfr2012*)
* Pourcentage de familles monoparentales, en 1970 et 2000 (noms des attributs: *famo1970, famo2000*)
* Evolution de 1970 à 2000 du pourcentage de familles monoparentales (nom de l'attribut: *famo7000*)
* Nombre de logements vacants, en 2000, 2005, 2010, 2012 (noms des attributs: *lovac00, lovac05, lovac10, lovac12*)
* Total des déchets collectés en 2010, en tonnes (nom de l'attribut: *dechet10*)

Ensuite téléchargez la liste des appartements dans le fichier `appartements.csv` (tuto #18). Les coordonnées sont en latitude/longitude (WGS84, EPSG:4326). Importez ce fichier dans QGIS et convertissez-le en fichier Shape (attention à la projection! tuto #8) Comptez ensuite le nombre d'appartements dans chaque commune se trouvant dans la liste (tuto #19). Ajoutez un attribut *napparts* dans votre fichier Shape des communes vaudoises contenant ce nombre.

Pour avoir une correction de votre exercice, vous devez rendre la couche Shape des communes vaudoises sélectionnées, c'est-à-dire tous les fichiers appartenant au format Shape y compris le fichier .prj (donc au minimum .shp, .shx, .dbf et .prj) et contenant les attributs mentionnés ci-dessus (vérifier que les noms des attributs ainsi que leur type soient correctes). Rendez une archive ZIP contenant l'ensemble des fichiers.

* Tutoriels par rapport à cet exercice:
	* Pour remplacer l'attribut "Communes" de STAT-TAB (de style "......5401 Aigle") par le géocode seul dans LibreOffice Calc: ouvrir "Rechercher & remplacer"; Rechercher ...... et Remplacer par [rien]; cocher "Expressions régulières" dans "Autres Options"; Rechercher ([:digit:]{4}).+$ et Remplacer par $1. Fini!
	* [QGIS Tutorial #8: Projections](https://www.youtube.com/watch?v=ACfCxfA92kY&index=8&list=PLbjixabFMUzPgm8VFyBUP7fs9DRBNEbsw)
	* [QGIS Tutorial #15: Sélectionner des entités avec une liste de valeurs ](https://youtu.be/W51UaWcTExw?list=PLbjixabFMUzPgm8VFyBUP7fs9DRBNEbsw)
	* [QGIS Tutorial #16: Joindre des attributs sur la base d'un champ commun ](https://youtu.be/EhliMhtdxUI?list=PLbjixabFMUzPgm8VFyBUP7fs9DRBNEbsw)
	* [QGIS Tutorial #17: Conversion du type d'attribut avec la calculatrice d'attributs ](https://youtu.be/iiMUN6hYhbc?list=PLbjixabFMUzPgm8VFyBUP7fs9DRBNEbsw)
	* [QGIS Tutorial #18: Convertir un fichier CSV en Shape à l'aide de colonnes lat/long ](https://youtu.be/8JO7rZRWj9o?list=PLbjixabFMUzPgm8VFyBUP7fs9DRBNEbsw)
	* [QGIS Tutorial #19: Jointure spatiale](https://www.youtube.com/watch?v=HS7yE20IPAU&index=13&list=PLbjixabFMUzPgm8VFyBUP7fs9DRBNEbsw)

* [Ensemble des tutoriels QGIS](https://www.youtube.com/playlist?list=PLbjixabFMUzPgm8VFyBUP7fs9DRBNEbsw)
