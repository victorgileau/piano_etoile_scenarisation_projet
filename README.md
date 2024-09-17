# Scénarisation

## Idée

### Concept

Installation qui utilise l'ombre de l'interacteur pour affecter une projection circulaire.

### Objectifs

Créé un lien entre l'interacteur et le visuel.

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

![mooboard](medias/images/moodboard.jpg)

### Planche d'ambiances sonores

### Références artistiques (image de reference)

## Technologies

### Support médiatique

### Matériel

#### Schéma

Le point est l'interacteur.

![schéma](medias/images/schema.jpg)

* Projecteur

![image](medias/svg/projecteur.svg)

* Lumières (x3)

![image](medias/svg/lumiere-2.svg)

* Detecteur de lumière (nombre à déterminer)

![image](medias/svg/detecteur_lumiere.svg)

* Mur

![image](medias/svg/mur.svg)

* Cables (extensions, cables pour detecteur de lumière et cables pour lumièr)

* Portable ou ordinateur avec touchDesigner

* Écran, souris et clavier

### Logiciels

* ToucheDesigner

* OSC (pour le moment)

* Programme Arduino
