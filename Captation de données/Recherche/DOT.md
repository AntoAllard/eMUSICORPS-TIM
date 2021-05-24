# Recherches et notes XSens DOT

Le système XSens DOT se rapproche énormément du système Awinda, à quelques différences près. Le système DOT comprend 5 capteurs individuels qui permettent de récupérer des données dans un nombre d'applications infinies, dont la santé , les sports et l'éducation. Le système de récupération de données est une application Android et iOS, mais un SDK est aussi disponible pour le développement sur Android studio ou autre.

## Positionnement des capteurs et mensurations

Les capteurs DOT offrent une liberté beaucoup plus intéressante que le système Awinda, car les capteurs peuvent être placés exactement où l'utilisateur a besoin de récupérer les données pour son champ d'expertise. Cela offre une expérience beaucoup plus personnalisée pour chaque cas d'utilisation. Un autre avantage est qu'il n'y a pas de fonction haut du corps et bas du corps, les capteurs fonctionnent avec les positions 3D X, Y et Z, dont le point de départ est établi suite à la calibration du capteur au début ou avant la captation. 

## Transfert de données en temps réel

L'application mobile DOT conçue exclusivement pour les capteurs DOT nous permet de récupérer les données suivantes : les coordonnées x, y et z, l'accélération en m/s2, la vitesse angulaire en degrée/s, le champ magnétique en a.u., et l'orientation, soit en quaternions ou en angles euler. Il n'est pas possible d'envoyer les données en temps réel d'un système Android ou iOS directement vers un ordinateur. 

![Screenshot application DOT](../Images/application_dot.JPG)

Par contre, grâce à leur SDK disponible pour iOS et Android, ainsi que le Xsens DOT Server, il est possible, avec un ordinateur possédant une connectivité Bluetooth, de recevoir directement les données sur ordinateur et ensuite les transmettre vers un autre logiciel de son choix.

## Autre information pertinente

Lien vers les capteurs DOT:
https://www.xsens.com/xsens-dot?utm_term=xsensdot&utm_medium=ppc&utm_campaign=CAN+%7C+Search+%7C+Brand&utm_source=adwords&hsa_cam=11537670902&hsa_src=g&hsa_mt=e&hsa_ver=3&hsa_net=adwords&hsa_tgt=kwd-1155776015707&hsa_acc=1306794700&hsa_grp=111847232785&hsa_kw=xsensdot&hsa_ad=476804384851&gclid=CjwKCAjw-qeFBhAsEiwA2G7Nl1zq45NmTaHv38y1Ivt9yWipseE91V9k6sVdG5uCw3kyYGGbgseIqxoCwYMQAvD_BwE

Lien vers le manuel d'utilisation:
https://www.xsens.com/hubfs/Downloads/Manuals/Xsens%20DOT%20User%20Manual.pdf?hsCtaTracking=ba3917b0-c02b-4b83-9dd0-fcc0d06d0d13%7Ca200d741-4f23-4e67-9041-048d7a27de39