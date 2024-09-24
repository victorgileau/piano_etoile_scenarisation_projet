# Projet : Le piano d'étoile

## Idée

### Concept

Installation qui utilise une kinect pour detecter la postion de l'interacteur pour effectuer une projection.

### Objectifs

Créé un lien entre l'interacteur et le visuel. Permetre de voir la grandeur des astres qui entoure la terre.

[Définition des objectifs de l'expérience : quel est le message ou l'émotion que l’on souhaite faire passer ?]: #

### Motivations

[Discussion des motivations créatives derrière le choix des médias et des technologies.]: #

* Une bonne compréension de touchDesigner

## Scénario

```mermaid
flowchart TD
    A[Interacteur entre dans la salle] --> B(Observer la salle)
    B --> C{Interacteur fait une action}
    C --> D[Va vers la zone de detection de la kinect]
    C --> E[Ne fait rien]
    E --> B
    D --> F{Fair une action}
    F -->|Bouger à droite| G[Change de son pour celui assigné à la boulle à la droite + la boulle qui était devant l'interacteur devient inactive et moins claire. L'inverse se produit à celle à droite]
    F -->|Bouger à gauche| H[Change de son pour celui assigné à la boulle à la gauche + la boulle qui était devant l'interacteur devient inactive et moins claire. L'inverse se produit à celle à gauche]
    F -->|Reculer| I[La boulle raptisie et Diminu volume trame sonore]
    F -->|Avancer| J[La boulle grossie et Augmante volume trame sonore]
    F -->|Rien faire| B
```

## Ambiance

### Planche d'ambiances visuelles (moodboard)

![mooboard](medias/images/implulsum_moodboard_projet.jpg)

![protoype](medias/images/prototype_boulle_chantante.png)

### Planche d'ambiances sonores

[Vidéo Youtube son d'étoile (les crédits des sons son dans la description de la vidéo)](https://www.youtube.com/watch?v=UoIm7IS0sgY)

[Utilisation d'échantillons, de musiques, de textures sonores pour représenter l’univers artistique.]: #

## Technologies

### Support médiatique

Utilisation de sons différents pour chaque section où il y aura une boulle dans la projection pour créer une trame sonore complète.
Visuel fait avec TouchDesigner créant des images de boulles chantantes ressemblant à des étoiles.

[Description des types de médias (vidéo, audio, lumières, capteurs, etc.) et de leur intégration pour créer une expérience immersive.]: #

### Matériel

#### Schéma

Le point est l'interacteur.

<img src="medias/images/impulsum_schema_v2.jpg" width="80%">

* Projecteur

![image](medias/svg/impulsum_icon_projecteur.svg)

* Lumières (x3)

![image](medias/svg/impulsum_icon_lumiere.svg)

* kinect (x1)

![kinect](medias/images/500px-KinectForWindows.jpg)

* Speakers (x2)

![image](medias/svg/impulsum_icon_speaker.svg)

* Mur

![image](medias/svg/impulsum_icon_mur.svg)

* Cables (extensions, cables pour la kinect)

* Portable ou ordinateur avec touchDesigner

* Écran, souris et clavier

### Logiciels

* TouchDesigner

* OSCBridge (pour le moment)

* Programme Arduino

### Réseautage

Communication faite entre un portable ou un ordinateur avec un périphérique qui a un programme Arduino qui permet la communication avec TouchDesigner.
Câble USB ou Ethernet à déterminer.

## Réferences

### Medias

* [The Immersive, Transcendental Experience of AudioVisual Installation](https://medium.com/@harrydavidhm/the-immersive-transcendental-experience-of-audiovisual-installation-b252b76d860c)
* [Générer par ai trouver sur google](https://www.freepik.com/premium-ai-image/multimedia-installation-exploring-role-design_235406780.htm)
* [‘We Harvest Wind’ Renewable energy art installation](https://www.youtube.com/watch?app=desktop&v=tzfy7VtPCCU)
* [Connection 1](https://blog.connectinstitute.ma/connexion-1-une-installation-multimedia-unique/)
* [Boulle rgb](https://www.youtube.com/watch?app=desktop&v=DKmHAMbtDlg)


**Par Victor Gileau**
