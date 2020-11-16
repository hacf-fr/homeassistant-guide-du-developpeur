# Home Assistant Development - Howto pour les Froggies

- [La boîte à outils](#La-Boîte-à-outils)
- [Les environnements](#Les-environnements)
  - [Le backend](#Le-backend)
  - [Le frontend](#Le-frontend)
- [Préparer son environnement](#Préparer-son-environnement)
- [Les ressources](#Les-ressources)

## La boîte à outils

**Obligatoires**:

- [git](https://git-scm.com/book/fr/v2) pour la gestion de version
- Un compte [Github](https://github.com/)

**Recommandés**:

- [Docker](https://www.docker.com/) pour tester vos contributions dans un environement local et dédié (conteneur).
- [Visual Studio Code (VSC)](https://code.visualstudio.com/). Tout autre editeur peut convenir.
  VSC offre plusieurs addons qui facilitent le développemnent avec Home Assistant.
- L'Addon [Remote - Containers](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers) pour VSC.
  Il permet d'utiliser les conteneurs de développement via Docker.

**Recommandés pour le développement de modules Python**:

- [pyenv](https://github.com/pyenv/pyenv) pour gérer les différentes versions Python à utiliser sur votre système de développement.
- [pipx](https://pipxproject.github.io/pipx/) pour installer des utilitaires Python dans des environnements isolés.
- [pre-commit](https://pre-commit.com/) pour assurer la qualité de vos modifications avant de les valider dans votre dépôt (commit)

## Participer aux projets

Avant de présenter plus en avant le développement sous Home Assistant, nous allons faire un point sur la gestion d'un projet (un développement).

Si vous êtes familier avec Gitub, vous pouvez passer ce chapitre. Pour les autres ...

- => [Travailler avec GitHub](./GITHUB.md)

## Les environnements

Il y a deux environnements distincts :

- Le backend ou le coeur de Home Assistant
- Le frontend ou l'interface utilisateur

Suivant ce que vous allez travailler, vous n'aurez pas besoin des mêmes langages, compétences et ressources.

- => [Développer en backend](./BACKEND.md)

- => [Développer en frontend](./FRONTEND.md)

## Les ressources

Ci-dessous un ensemble de ressources qui compléteront votre apprentissage.

- La [documentation développeur](https://developers.home-assistant.io/) chez Home Assistant
- La gestion des [flux](https://guides.github.com/introduction/flow/), des [Issues](https://guides.github.com/features/issues/) et des [Pull Request](https://guides.github.com/activities/forking/) (PR) de Github
- Le template prêt à lemploi [CookieCutter](https://github.com/oncleben31/cookiecutter-homeassistant-custom-component)
- Les icônes incontournables de [Material Design](https://materialdesignicons.com/)
