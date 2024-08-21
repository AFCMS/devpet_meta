---
marp: true
author: AFCMS
lang: fr-FR
theme: default
backgroundImage: url('https://marp.app/assets/hero-background.svg')
paginate: true
---

<!--
SPDX-FileCopyrightText: 2024 AFCMS <afcm.contact@gmail.com>
SPDX-License-Identifier: GPL-3.0-or-later
-->

# DevPet 🦖

## Un dinosaure de compagnie virtuel, pour les développeurs.

---

## Qui suis-je ?

Je suis **Louis Walter**, étudiant en première année à l'école **Hexagone**.

Je suis passioné par le développement de logiciel et de jeux vidéos.

---

## Introduction

Prennez soin d'un dinosaure virtuel en étant actif sur **GitHub**, en écoutant de la musique sur **Spotify** ou en jouant à un mini-jeu intégré et en le nourrissant de café régulièrement.

Plus vous êtes actif, plus votre animal de compagnie sera en bonne santé.

---

## C'est quoi exactement ?

C'est un petit boitier crée en impression 3D avec **Fusion360**, doté d'un écran et de trois boutons qui communique avec votre ordinateur via **Bluetooth**.

Depuis votre ordinateur, vous pourrez configurer et lancer le **backend** qui communique avec l'appareil et effectue la récupération de données.

Pour le développement, j'ai utilisé **C++** avec **PlatformIO** pour la partie embarquée, ainsi que **NodeJS** avec **Typescript** pour le backend.

---

## Quelles sont les fonctionalités ?

La santé de votre dinosaure est liée à trois statistiques principales :

-   **L'humeur**
-   **L'énergie**
-   **La productivité**

Si une des trois statistiques tombe à zéro, votre dinosaure virtuel meurt.

Pour vous donner une idée de sa santé, une moyenne géométrique de ces trois statistiques est calculée et affichée sur sa barre de vie.

Une zone spéciale vous permet de voir les derniers événements qui ont eu lieu, une page séparée vous permet de voir les statistiques détaillées.

---

### Humeur

Vous aimez écouter de la musique en travaillant ?

Quand vous écoutez de la musique sur **Spotify**, votre dinosaure gagne en humeur.

Vous avez une pose ? Vous pouvez aussi jouer au mini-jeu intégré pour améliorer encore plus son humeur !

---

### Energie

Vos meilleures idées vous viennent après une grande tasse de café ☕ ?

Un simple click sur le bouton central et votre dinosaure gagne en énergie.

La régularité de la prise de café est importante pour sa santé !

---

### Productivité

Vous utilisez **GitHub** pour vos projets ?

Quand vous poussez des commits Git, que vous ouvrez des issues ou que vous créez des pull requests, votre dinosaure gagne en productivité.

Ah, si seulement ça pouvait vous motiver à finir tous vos projets persos... 🤔

---

## Démonstration

---

## Architecture du projet

---

## Quelles améliorations possibles ?

---

### Mini-jeu intégré

Le mini-jeu actuel pourrait être amélioré en ajoutant des fonctionnalités supplémentaires, comme des niveaux de difficulté, des ennemis différents, des animations, etc.

---

### Driver de périphérique (sous Linux)

La connection Bluetooth se fait actuellement au travers de l'utilitaire en ligne de commande `rfcomm`.

Il serait possible de créer un driver de périphérique qui se connecte automatiquement à l'appareil lorsqu'il est à portée et qui lancerait le backend de manière entièrement automatique.

---

### Utilisation d'un service web pour la récupération de données

Au lieu de demander à l'utilisateur la mise en place d'un token d'accès **GitHub** et de sa propre application OAuth2 pour **Spotify**, ainsi que l'exécution du backend complet, il serait possible de mettre en place un service web qui effectue ces tâches au travers de tokens OAuth2 uniquement.

Le service web pourrait communiquer en WebSocket avec un driver de périphérique qui se connecterait à l'appareil de manière automatisée.

---

### Portage du backend de NodeJS à Deno

Le backend actuel est écrit en **NodeJS**. Il serait envisagable de le porter à **Deno** pour des raisons de sécurité et de performance.

La principale difficulté réside en la disponibilité des librairies, notamment pour la communication série.

Parmis les améliorations attendues :

-   Support TypeScript natif
-   Systèmes de vérification intégrés (linting, type-checking, tests unitaires, etc)
-   Création de binaires indépendants avec exécution en bac à sable

---

## Remerciements

-   [Eladji](https://github.com/eladji) pour les modèles **Fusion360** des composants de base (ESP32, écran et boutons)
-   [Émilien](https://github.com/AKArien0) pour l'[aide](https://github.com/AKArien0/arduino-input-handler) concernant le système de gestion des boutons
-   [Clément (@Klhmt)](https://github.com/Klhmt) pour le design et les sprites animés du dinosaure principal

---

## Des questions ?
