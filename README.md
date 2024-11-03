# Projet : Le piano d'étoile

## Idée

### Concept

Installation qui utilise une Kinect pour détecter la position de l'interacteur pour effectuer une projection. La projection consiste de plusieurs étoiles alignées les unes à côté des autres, ayant chacune une section assignée où les interacteurs peuvent interagir avec l'étoile dans leurs sections.

### Objectifs

Émerveiller l'interacteur en créant un lien entre l'interacteur et le visuel. Permettre de voir la grandeur des astres qui entourent la terre.

[Définition des objectifs de l'expérience : quel est le message ou l'émotion que l’on souhaite faire passer ?]: #

### Motivations

[Discussion des motivations créatives derrière le choix des médias et des technologies.]: #

* Les étoiles (objets peu connus est donc un sujet intéressant à explorer)
* Une bonne compréhension de TouchDesigner


## Scénario

```mermaid
flowchart TD
    A[Interacteur entre dans la salle] --> B(Observer la salle)
    B --> C{Interacteur fait une action}
    C --> D[Va vers la zone de detection de la kinect]
    C --> E[Ne fait rien]
    E --> B
    D --> F{Fair une action}
    F -->|Bouger à droite| G[Change de son pour celui assigné à la boulle à la droite + ]
    F -->|Bouger à gauche| H[Change de son pour celui assigné à la boulle à la gauche + ]
    F -->|Reculer| I[L'étoile raptisie et Diminu volume trame sonore]
    F -->|Avancer| J[L'étoile grossie et Augmante volume trame sonore]
    F -->|Rien faire| B
    G --> K[L'étoile qui était devant l'interacteur devient inactive et moins claire. L'inverse se produit à celle à droite]
    H --> L[L'étoile qui était devant l'interacteur devient inactive et moins claire. L'inverse se produit à celle à gauche]
```

## Ambiance

### Planche d'ambiances visuelles (moodboard)

![mooboard](medias/images/piano-etoile_moodboard_v2.jpg)

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

<img alt="schema" src="medias/images/schema-v4.jpg" width="80%">

| Projecteur | Lumières (x3) | Kinect | Speakers (x2) | Mur |
| :--------------- |:---------------| :-----| :--------------- |:---------------|
| ![svg de projecteur](medias/svg/icon_projecteur.svg) | ![svg de lumière](medias/svg/icon_lumiere.svg) | ![svg de kinect](medias/svg/icon_detecteur_lumiere.svg) ![image de kinect](medias/images/500px-KinectForWindows.jpg) | ![svg de speaker](medias/svg/icon_speaker.svg) | ![svg de mur](medias/svg/icon_mur.svg) |

* Cables (extensions, cables pour la kinect, cables pour les lumières)

* Portable ou ordinateur avec touchDesigner

* Écran, souris et clavier

### Logiciels

* TouchDesigner

* QLC+ (pour les lumières)

* Programme pour utiliser la kinect

### Réseautage

Un portable ou un ordinateur avec TouchDesigner communique avec un logiciel qui peut comprendre les données de la Kinect et qui les renvoie à TouchDesigner.
Câble USB ou Ethernet à déterminer.

## Réferences

### Medias

* [Étoile (soleil)](https://www.numerama.com/sciences/642330-cette-etoile-se-deplace-a-8-de-la-vitesse-de-la-lumiere-pourquoi-est-elle-si-rapide.html)
* [Générer par ai trouver sur google](https://www.freepik.com/premium-ai-image/multimedia-installation-exploring-role-design_235406780.htm)
* [Première Étoile](https://www.cieletespace.fr/actualites/les-astronomes-ont-ils-enfin-observe-une-etoile-primordiale)
* [Connection 1](https://blog.connectinstitute.ma/connexion-1-une-installation-multimedia-unique/)
* [Boulle rgb](https://www.youtube.com/watch?app=desktop&v=DKmHAMbtDlg)


**Par Victor Gileau**
