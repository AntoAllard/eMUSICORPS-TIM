# Recherches et notes XSens DOT

Le système XSens DOT se rapproche énormément du système Awinda, à quelques différences près. Le système DOT comprend 5 capteurs individuels qui permettent de récupérer des données dans un nombre d'applications infinies, dont la santé , les sports et l'éducation. Le système de récupération de données est une application Android et iOS, mais un SDK est aussi disponible pour le développement sur Android studio ou autre.

## Positionnement des capteurs et mensurations

Les capteurs DOT offrent une liberté beaucoup plus intéressante que le système Awinda, car les capteurs peuvent être placés exactement où l'utilisateur a besoin de récupérer les données pour son champ d'expertise. Cela offre une expérience beaucoup plus personnalisée pour chaque cas d'utilisation. Un autre avantage est qu'il n'y a pas de fonction haut du corps et bas du corps, les capteurs fonctionnent avec les positions 3D X, Y et Z, dont le point de départ est établi suite à la calibration du capteur au début ou avant la captation. 

## Transfert de données en temps réel

L'application mobile DOT conçue exclusivement pour les capteurs DOT nous permet de récupérer les données suivantes : les coordonnées x, y et z, l'accélération en m/s2, la vitesse angulaire en degrée/s, le champ magnétique en a.u., et l'orientation, soit en quaternions ou en angles euler. Il n'est pas possible d'envoyer les données en temps réel d'un système Android ou iOS directement vers un ordinateur. 

![Screenshot application DOT](../Images/application_dot.JPG)

Par contre, grâce à leur SDK disponible pour iOS et Android, ainsi que le Xsens DOT Server, il est possible, avec un ordinateur possédant une connectivité Bluetooth, de recevoir directement les données sur ordinateur et ensuite les transmettre vers un autre logiciel de son choix.

