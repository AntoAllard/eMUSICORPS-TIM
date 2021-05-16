# Recherches et notes XSens Awinda

## Positionnement des capteurs et mensurations

Le XSens Awinda offre une captation de données pour le corps en entier. Le système de base comprend 6 capteurs pouvant être placés à plusieurs endroits sur le corps de l'utilisateur selon les besoins.

Tableau de placement des capteurs :

![Tableau de positionnement des capteurs](../Images/tableau_positionnement_xsens_awinda.JPG)

Il est important aussi de mesurer la dimension du corps de la personne qui portera les capteurs, puisque cela aura un incidence sur la calibration.

![Tableau des mensurations](../Images/tableau_mensurations_xsens_awinda.JPG)

Dans notre cas, qui est la captation de mouvement d'un joueur de piano, nous n'avons pas besoin des capteurs pour le bas du corps puisqu'il sera en position assis. Il est donc possible de mettre les capteurs en mode No-level, ce qui envoie comme message aux capteurs qu'effectivement l'utilisateur restera en position assis pour la durée de la captation. 

## Transfert de données en temps réel

Dans la théorie, il est possible de d'envoyer les données en temps réel à différentes plateformes et sous plusieurs formes selon les options du Network Streamer.

![Tableau des options streaming](../Images/tableau_options_streamer.JPG)

L'option qui nous intéresse dans notre cas est l'option Unity 3D. Cette option nous permet d'utiliser le plugin Unity pour transférer les données en temps réel vers Unity 3D.