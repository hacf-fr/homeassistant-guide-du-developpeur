# Home Assistant - Guide du développeur

- [La boîte à outils](#La-Boîte-à-outils)
- [Participer aux projets](#Participer-aux-projets)
- [Les environnements](#Les-environnements)
  - Le backend
  - Le frontend
- [Préparer son environnement](#Préparer-son-environnement)
- [Les ressources](#Les-ressources)

## Présentation

Ce guide a pour vocation de présenter le développement de composants de Home Assistant.

Pour ce faire nous présenterons indépendamment chacun des environnements de développement :

- le backend qui concerne les intégrations (entités/sensors)

- le frontend qui concerne l'interface utilisateur (Lovelace et ses composants)

## La boîte à outils

Chaque environnement a ses outils spécifiques et seront précisés dans chaque section.

Néanmoins voici quelques éléments commun aux deux :

**Obligatoires**:

- [git](https://git-scm.com/book/fr/v2) pour la gestion de version.
- Un compte [Github](https://github.com/)

**Recommandés**:

- [Docker](https://www.docker.com/) pour tester vos contributions dans un environement local et dédié (conteneur).
- [Visual Studio Code (VSC)](https://code.visualstudio.com/). Tout autre editeur peut convenir.
  VSC offre plusieurs addons qui facilitent le développemnent avec Home Assistant.
- L'Addon [Remote - Containers](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers) pour VSC.
  Il permet d'utiliser les conteneurs de développement via Docker.

## Participer aux projets

Avant de présenter plus en avant le développement sous Home Assistant, nous allons faire un point sur la gestion d'un projet (un développement).

Si vous êtes familier avec GitHub, vous pouvez passer ce chapitre. Pour les autres ...

- [Travailler avec GitHub](./GitHub.md)

## Les environnements

Il y a deux environnements distincts :

- Le backend ou le coeur de Home Assistant
- Le frontend ou l'interface utilisateur

Suivant ce que vous allez travailler, vous n'aurez pas besoin des mêmes langages, compétences et ressources.

- [Développer en backend](./Backend.md)

- [Développer en frontend](./Frontend.md)

## Les ressources

Ci-dessous un ensemble de ressources qui compléteront votre apprentissage.

- La [documentation développeur](https://developers.home-assistant.io/) chez Home Assistant
- La gestion des [flux](https://guides.github.com/introduction/flow/), des [Issues](https://guides.github.com/features/issues/) et des [Pull Request](https://guides.github.com/activities/forking/) (PR) de Github
- Le template prêt à lemploi [CookieCutter](https://github.com/oncleben31/cookiecutter-homeassistant-custom-component)
- Les icônes incontournables de [Material Design](https://materialdesignicons.com/)
