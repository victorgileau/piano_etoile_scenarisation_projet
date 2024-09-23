# Projet : Instrumentum

## Idée

### Concept

Installation qui utilise des instruments de musique utiliser par l'interacteur pour affecter une projection circulaire.

### Objectifs

Créé un lien entre l'interacteur, la musique et le visuel.

Voir l'impact de la musique visuellement.

### Motivations

* Une bonne compréension de touchDesigner
* Permet un element d'intercativiter simple

## Scénario

```mermaid
flowchart TD
    A[Interacteur entre dans la salle] --> B(Observer la salle)
    B --> C{Interacteur fait une action}
    C --> D[Va vers les detecteur de lumière]
    C --> E[Ne fait rien]
    E --> B
    D --> F{Fair une action}
    F -->|Bouger à droite| G[Fait bouger les boulles sur la projections vers la droites]
    F -->|Bouger à gauche| H[Fait bouger les boulles sur la projections vers la gauche]
    F -->|Reculer| I[La boulle raptisie]
    F -->|Avancer| J[La boulle grossie]
    F -->|Rien faire| B
```

## Ambiance

### Planche d'ambiances visuelles (moodboard)

![mooboard](medias/images/moodboard_projet.jpg)

### Planche d'ambiances sonores

### Références artistiques (image de reference)

## Technologies

### Support médiatique

### Matériel

#### Schéma

Le point est l'interacteur.

![schéma](medias/images/schema.jpg)

* Projecteur

![image](medias/svg/icon_projecteur.svg)

* Lumières (x3)

![image](medias/svg/icon_lumiere.svg)

* Instruments de musiques

![image](medias/svg/icon_detecteur_lumiere.svg)

* Mur

![image](medias/svg/icon_mur.svg)

* Cables (extensions, cables pour detecteur de lumière et cables pour lumièr)

* Portable ou ordinateur avec touchDesigner

* Écran, souris et clavier

* Instrument de musique (x5) 

* Micro sur chaque instrument pour capter les instruments

### Logiciels

* ToucheDesigner

* OSC (pour le moment)

* Programme Arduino
