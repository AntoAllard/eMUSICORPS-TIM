# Fonctionnement et tests d'Awinda 

Au départ, l'équipement qui semblait être la meilleure idée était la station Awinda avec les capteurs de mouvements MTw. Par contre, il a été déterminé que cet outil ne convenait pas totalement aux besoins du projet. Dans la section *Éléments testés*, les problèmes survenus sont présentés.

## Éléments testés

1. Faire communiquer les données entre MT Software et Unity.
    
    **Description**: Après avoir fait des recherches, une façon de transmettre les données semblait sortir du lot : utiliser un plugin d'Unity. À partir d'un logiciel de Xsens, il est possible d'envoyer les données vers Unity, grâce à ce plugin. Par la suite, il peut être simple d'ajouter de l'OSC pour retransmettre ces données vers un autre logiciel. 

    **Résultat** : Le plugin n'est pas compatible avec le logiciel MT Software. Il faut absolument soit MVN Animate ou MVN Analyze. Ces deux derniers sont payants et requièrent un *dongle* à brancher sur l'ordinateur.
    

2. Utilisation d'une librairie Python afin de passer par-dessus les logiciels de Xsens.

    **Description**: Installer la librairie [xsens_driver](https://wiki.ros.org/xsens_driver), qui permet d'utiliser les capteurs de mouvements Xsens dans un système ROS.

    **Résultat** : Cette méthode est très pointilleuse sur les versions utilisées. Selon ce qui a été fait, il faut absolument la version 3.8.x de Python. Sinon, les commandes nécessaires à l'installation ne fonctionneront pas correctement.

3. Ouvrir la communication avec la station Awinda

    **Description**: Une fois la librairie installée, il faut ouvrir la communication avec la station Awinda en saisissant la ligne suivante dans l'invite de commandes : 

            python mtdevice.py

    **Résultat** : À chaque fois, l'erreur suivante apparaissait : 

            MTException: unable to open /dev/ttyUSB0
            
    Ceci est dû au fait que cette librairie a été créée pour Linux et macOS, alors que les tests ont été effectués avec Windows. Cette commande doit ouvrir le port où est branchée la station, mais ttyUSB0 est le nom d'un port sur un Mac. Une piste de solution a été de dire à la librairie de lire le port COM3 (où était branchée la station), mais cette commande n'a pas été comprise par l'ordinateur. 

4. Utiliser un ordinateur virtuel Linux fonctionnant sous Ubuntu

    **Description**: Puisque la librairie est fonctionnelle sous Linux, un ordinateur a été installé pour pouvoir faire les tests sous ce système d'exploitation.

    **Résultat** : Une fois la librairie installée et la connexion faite, le message suivant affichait : No suitable device found. Au final, les MTw avec Awinda n'étaient pas totalement compatibles avec cette librairie. C'est à ce moment que la décision de se tourner vers les Xsens DOT a été prise.