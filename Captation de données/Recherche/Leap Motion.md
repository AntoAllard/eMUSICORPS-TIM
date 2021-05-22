# Recherches et notes Leap Motion

## Fonctionnement général du Leap Motion

Le Leap Motion de Ultraleap fonctionne avec deux caméras infrarouges et plusieurs LED qui illumine les mains avec des la lumière infrarouge invisible à l'oeil nu et qui est capté par les deux caméras. Toutes les données de positionnement sont ensuite renvoyées vers l'ordinateur via USB. Le logiciel de suivi de la main d'Ultraleap modélise la structure sous-jacente de la main au niveau des articulations et des os. Cela signifie que le logiciel peut déterminer avec précision la position d'un doigt ou d'un pouce, même s'il n'est pas visible. Le SDK comporte une API appelée LeapC qui permet d'accéder aux données grâce à plusieurs langages de programmation. Les intégrations pour les moteurs Unity et Unreal sont construites sur cette API. Une liaison officielle pour C# est disponible, ainsi que des liaisons existantes pour C++, Java, JavaScript, Python et Objective-C.

## Installation et utilisation

L'Installation du Leap Motion est plug and play et le meilleur moyen de tester si tout fonctionne comme il faut est en utilisant le Leap Motion Control Panel. Le Leap Motion  peut être orienté de deux manières différentes : sur le bureau (face à une table) et sur la tête (fixé à un casque VR/AR). Un pluggin Unity permet de tester le capteur dans quelque scènes différentes pour se familiariser avec celui-ci.

## Autre information pertinente