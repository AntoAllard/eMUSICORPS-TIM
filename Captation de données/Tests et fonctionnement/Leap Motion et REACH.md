# Fonctionnement et tests du Leap Motion et REACH

## Fonctionnement

Voici les étapes pour utiliser le Leap Motion avec REACH et récupérer les données:

1. Branchez votre Leap Motion à votre ordinateur

2. Téléchargez le Leap Motion Control Panel - https://developer.leapmotion.com/sdk-leap-motion-controller/

3. Activez le Leap Motion en appuyant sur l'icône caché du Leap motion et sélectionnez "Resume Tracking"

    ![Screenshot resume tracking](../Images/resume_tracking.JPG)

4. Allez dans votre Control Panel du Leap Motion, puis dans l'onglet dépannage, cliquez sur "Visualiseur de diagnostic"

    ![Screenshot depannage](../Images/depannage.JPG)

5. Appuyez sur "V" jusqu'à ce que la vue soit configuré pour les appareils VR (head-mounted device)

    ![Screenshot visualiseur de diagnostic](../Images/visualiseur.JPG)

6. Installez REACH à partir du GitHub - https://github.com/NiccoloGranieri/Reach

7. Ouvrez REACH et vérifiez la connection en passant vos mains devant le capteur. Si vous voyez les lumières rouges passer au vert, la connection est bonne, si non il vous faudra peut-être redémarrer votre ordinateur.

8. Cochez les cases "Head Mounted" ainsi que "Normalised Values"

    ![Screenshot de REACH](../Images/reach.JPG)

9. Dans l'application de votre choix (ici Max/MSP), vous pouvez utiliser le port et/ou l'adresse IP de REACH (ici le port) pour transmettre les données

    ![Screenshot de Max/MSP](../Images/receive.JPG)

10. Voici la liste de données qui vous sera alors transmis par REACH

    ![Screenshot de liste de données](../Images/donnees.JPG)

## Éléments à tester

1. Voir si le capteur Leap Motion peut être utilisé visant vers le bas en position fixe

Dans notre utilisation du Leap Motion, nous avons besoin de capter les mains du pianiste sur le clavier. Pour se faire il suffit de tester si le Leap Motion peut être attaché sur un trépied et pointer vers le bas.

Bien qu'il est déconseillé d'utiliser le Leap Motion autre que pointant vers le haut ou sur un casque VR, nous pouvons l'utiliser sur un trépied pointant vers le bas en le mettant en vue "head-mounted device". Cela reproduit exactement un casque de réalité virtuelle qui regarde ses mains ou vers le sol.

![Photo Leap motion sur trépied](../Images/leap_motion.jpg)

2. ...

Descritpion test
Résultat

3. ...

Descritpion test
Résultat
