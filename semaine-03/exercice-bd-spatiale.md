# Exercice 2: sources de données spatiales

---

* Buts de l'exercice 2:
	* Création d’une base de données spatiale
	* Calcul d’attributs
	* Jointure (par attribut et spatiale)

---


Préparez un fond de carte complet avec attributs des communes vaudoises se trouvant dans le fichier `ex2-communes.csv`. L'état des communes est celui de 2012, et le niveau de généralisation de la couche doit être le K4 de l'Office fédéral de la statistique (section ThemaKart). Vous devez y joindre les attributs suivants:

* Géocode de l'OFS et nom de la commune
* Population résidante permanente des années 2000, 2005, 2010, 2012 (noms des attributs: *pop2000, pop2005, pop2010, pop2012*)
* Nombre de personnes de nationalité française, en 2012 (nom de l'attribut: *fr2012*)
* Pourcentage de personnes de nationalité française, en 2012 (nom de l'attribut: *pfr2012*)
* Pourcentage de familles monoparentales, en 1970 et 2000 (noms des attributs: *famo1970, famo2000*)
* Evolutation de 1970 à 2000 du pourcentage de familles monoparentales (nom de l'attribut: *famo7000*)
* Nombre de logements vacants, en 2000, 2005, 2010, 2012 (noms des attributs: *lovac00, lovac05, lovac10, lovac12*)
* Total des déchets collectés en 2010, en tonnes (nom de l'attribut: *dechet10*)

Ensuite téléchargez la liste des appartements dans le fichier `appartements.csv`. Les coordonnées sont en latitude/longitude (WGS84, EPSG:4326). Importez ce fichier dans QGIS et convertissez-le en fichier Shape. Comptez ensuite le nombre d'appartements dans chaque commune se trouvant dans la liste. Ajoutez un attribut *napparts* dans votre fichier Shape des communes vaudoises contenant ce nombre.

Pour avoir une correction de votre exercice, vous devez rendre la couche Shape des communes vaudoises sélectionnées, c'est-à-dire tous les fichiers appartenant au format Shape y compris le fichier .prj (donc au minimum .shp, .shx, .dbf et .prj) et contenant les attributs mentionnés ci-dessus (vérifier que les noms des attributs ainsi que leur type soient correctes). Rendez une archive ZIP contenant l'ensemble des fichiers.
