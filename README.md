# Projet : Sellae Lucidae

## Concept

Installation qui utilise une Kinect pour détecter la position de l'interacteur pour effectuer une projection. La projection consiste de plusieurs étoiles alignées les unes à côté des autres, ayant chacune une section assignée où les interacteurs peuvent interagir avec l'étoile dans leurs sections.

### Objectifs

Émerveiller l'interacteur en créant un lien entre l'interacteur et le visuel. Permettre de voir la grandeur des astres qui entourent la terre.

[Définition des objectifs de l'expérience : quel est le message ou l'émotion que l’on souhaite faire passer ?]: #

### Motivations

[Discussion des motivations créatives derrière le choix des médias et des technologies.]: #

* Les étoiles (objets peu connus est donc un sujet intéressant à explorer)
* Une bonne compréhension de TouchDesigner

### Références et inspirations

#### Planche d'ambiances visuelles (moodboard)

![mooboard](medias/images/piano-etoile_moodboard_v2.jpg)

Prototype que j'ai fait.

![protoype](medias/images/prototype_boulle_chantante.png)

### Planche d'ambiances sonores

[Vidéo Youtube son d'étoile (les crédits des sons son dans la description de la vidéo)](https://www.youtube.com/watch?v=UoIm7IS0sgY)

[Utilisation d'échantillons, de musiques, de textures sonores pour représenter l’univers artistique.]: #

## Scénario interactif

### Déroulement interactif

L'utilisateur interagie en bougant devant l'ecran qui a une Kinect en dessous qui perment de detecter l'utiisateur est dans quelle sections. L'utilisateur peut interagire en  bougant ce qui affect des grosses étoiles leur lumière, leur grosseur et leur noise. L'uttilisateur affect aussie les petites étoile dans le background. Le son d'ambiance est constant.

[ - Décrire comment l’utilisateur interagit avec l’installation. - Expliquer les actions possibles, les réponses de l’installation (visuelles, sonores, lumineuses) et les chemins narratifs ou évolutions possibles.]: #

### Logigramme des interactions

[ - Présenter un schéma illustrant les points d’interaction clé, les déclenchements multimédias, et les éventuels embranchements narratifs.]: #

```mermaid
%%{init: {'theme': 'base', 'themeVariables': { 'fontSize': '2em', 'primaryColor': '#cfccff'}}}%%
flowchart TD
    A[Interacteur entre dans la salle] --> B(Observer la salle)
    B --> C{Interacteur fait une action}
    C --> D[Va vers la zone de detection de la kinect]
    C --> E[Ne fait rien]
    E --> B
    D --> F{Fair une action}
    F -->|Bouger à droite| G[Change de son pour celui assigné à la boulle à la droite + ]
    F -->|Bouger à gauche| H[Change de son pour celui assigné à la boulle à la gauche + ]
    F -->|Reculer| I[L'étoile raptisie et affect aussi les petites étoile en arrière]
    F -->|Avancer| J[L'étoile grossie et affect aussi les petites étoile en arrière]
    F -->|Rien faire| B
    G --> K[L'étoile qui était devant l'interacteur devient inactive et moins claire. L'inverse se produit à celle à droite]
    H --> L[L'étoile qui était devant l'interacteur devient inactive et moins claire. L'inverse se produit à celle à gauche]

linkStyle default stroke:#3e30ff
```

## Scénarimage / Simulation

### Visualisation des séquences

![arrière](medias/images/test_back-v2.jpg)

![côté](medias/images/test_side-v2.jpg)

![coin](medias/images/test_coin-v2.jpg)

[![video](https://img.youtube.com/vi/aPS43QriIpo/0.jpg)](https://www.youtube.com/watch?v=aPS43QriIpo)


[ - Présenter un scénarimage ou une simulation en 3D qui montre les principales étapes de l’expérience multimédia, du point de vue de l’utilisateur.]: #

### Illustrations des interactions

[ - Intégrer des visuels ou des captures d’écrans montrant comment l’installation réagit aux actions des utilisateurs.]: #

### Évolution visuelle et narrative

[ - Visualiser la progression de l'expérience en fonction des interactions utilisateurs.]: #

## Synoptique

![protoype](medias/images/plan_synoptique.png)

### Schéma technique

[ - Créer un synoptique représentant les connexions entre les dispositifs (câblages, réseaux, signaux audio/vidéo, etc.). - Préciser les types de signal, les protocoles utilisés et la communication entre les dispositifs (OSC, MIDI, DMX, etc.).]: #

### Flux de données

[ - Décrire le cheminement des flux de données entre les différentes composantes de l’installation.]: #

## Plantation

![côté](medias/images/test_side-v2.jpg)

### Emplacement des dispositifs

#### Schéma

Le point est l'interacteur.

<img alt="schema" src="medias/images/schema_v3.jpg" width="80%">

[ - Planifier la disposition des dispositifs multimédias dans l’espace (projecteurs, capteurs, caméras, haut-parleurs, etc.). - Justifier chaque emplacement en fonction des besoins techniques et des interactions utilisateurs..]: #

### Circulation des visiteurs

[ - Anticiper le mouvement des visiteurs et leur interaction avec les points d’interaction dans l’espace.]: #

### Gestion des câblages

[ - Préciser comment les câblages et connexions seront organisés pour assurer la sécurité et l’esthétique de l’installation.]: #

Next ------------------------------------------- tech

## Anticiper les besoins matériels et logiciels

### Liste des équipements

![côté](medias/images/projecteur.png)
![côté](medias/images/cable_kinect.png)
![côté](medias/images/lumiere.png)
![côté](medias/images/speaker.png)
![côté](medias/images/500px-KinectForWindows.jpg)

[ - Identifier les équipements nécessaires (projecteurs, serveurs, capteurs, dispositifs interactifs, etc.) et justifier leur choix en fonction des besoins du projet.]: #

### Logiciels et réseaux

[ - Préciser les logiciels et systèmes nécessaires au bon fonctionnement de l’installation (logiciels de projection, de traitement vidéo, gestion d’éclairage, etc.). - Décrire la gestion des réseaux et des systèmes de communication entre les différentes composantes.]: #

## Technologies

### Support médiatique

Utilisation de sons différents pour chaque section où il y aura une boulle dans la projection pour créer une trame sonore complète.
Visuel fait avec TouchDesigner créant des images de boulles chantantes ressemblant à des étoiles.

[Description des types de médias (vidéo, audio, lumières, capteurs, etc.) et de leur intégration pour créer une expérience immersive.]: #

### Matériel



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
