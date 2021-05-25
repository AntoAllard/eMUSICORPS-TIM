# Direction technique (Plans, schémas et équipements)

## Nature du projet

Descritpion des effets visuels recherchés

## Schéma de branchement

Fonctionnement : L'ordinateur qui génère les effets visuels envoie de 1 à 9 sorties vidéos (6 dans notre cas) vers un Pixel Map en format 4K divisé en 9 espaces symétriques de 1280x720. Une fois le Pixel Map remplit selon les désirs du créateur, la source est envoyé vers une carte de capture 4K 30fps, puis vers un deuxième ordinateur qui s'occupera de séparer le Pixel Map. 

<img src="../Images/pixelmap.png" alt="Pixel map" width="1000"/>

Sur cet ordinateur, dans OBS, il suffit de créer 6 instances du Pixel Map à partir de la source reçu de la carte 4K 30fps. 

<img src="../Images/creation_source.JPG" alt="Sources" width="1000"/>

Ensuite avec le raccourci ctrl + e, rogner dans chaque source, un vidéo du Pixel Map différent jusqu'à avoir tous les vidéos individuellement séparés.

<img src="../Images/rognage01.JPG" alt="Pixel map rogné" width="1000"/>
<img src="../Images/rognage02.JPG" alt="Pixel map rogné" width="1000"/>

Il faut savoir qu'un ordinateur peut seulement s'occupper de maximum trois projecteurs, faute de prises HDMI/DP. Ensuite, avec NDI, sur OBS, deux options s'offrent à nous. Si les vidéos n'ont pas besoin de vidéo mapping il est possible de grouper les 3 vidéos avec les offsets désirés en amont et d'envoyer le groupe complet, via un filtre NDI en effectuant un click droit sur le groupe et en ajoutant un filtre NDI dédié, vers l'ordinateur qui s'occupe des trois projecteurs désirés. 
 
<img src="../Images/groupe.JPG" alt="Grouper" width="1000"/>
<img src="../Images/NDIdedie.JPG" alt="Filtre NDI" width="1000"/>

Par contre, si les vidéos doivent passer par MadMapper, il serait mieux que les trois vidéos soient séparés, donc au lieu de grouper les vidéos, il suffit de créer trois dedicated output NDI différents, et d'envoyer les vidéos indépendemment vers l'ordinateur souhaité. 

<img src="../Images/schéma_branchement_eMUSICORPS.png" alt="Schéma de branchement" width="1000"/>

## Schéma de plantation

<img src="../Images/schema_plantation_projection.png" alt="Schéma de plantation" width="1000"/>

## Liste des équipements

Vidéo : 

Audio :

Lumières : 

Câbles et cartes :

Autre :

## Horaire d'implantation pour les tests

