# Le backend

## Compétences

Pour cet environnement vous devez avoir des connaissances du langage Python.

Vous pouvez acquerir des bases sur [ce cours](https://openclassrooms.com/fr/courses/4262331-demarrez-votre-projet-avec-python) OpenClassroom.


## Context

Il y a deux façons d'ajouter des intégrations à Home Asssitant:

- En modifiant le code de [Home Assistant](https://github.com/home-assistant/core)
ainsi l'intégration est disponible immédiatement aux utilisateurs
et n'importe quel développeur peut contribuer à améliorer l'intégration.
En revanche, il y a un certain nombre de contraintes à respecter
pour voir votre contribution intégrer le code officiel de Home Assistant.
Et les mises à jour ne seront déployées qu'au rythme imposé par la l'équipe officielle.
- En développant un module tier appelé *custom component*, installable à la main
ou via [HACS](https://hacs.xyz) par les utilisateurs de Home Assistant.
Il sera hebérgé sur votre compte GitHub (ou celui de l'organisation HACF)
et vous serez responsable de la maintenance au rythme que vous imposerez.
Cette intégration sera moins visible et moins accessibles pour les utilisateurs
mais vous aurez moins de contraintes pour le mettre au point.

## Boîte à outils recommendée

- [pyenv](https://github.com/pyenv/pyenv) pour gérer les différentes versions Python à utiliser sur votre système de développement.
- [pipx](https://pipxproject.github.io/pipx/) pour installer des utilitaires Python dans des environnements isolés.
- [pre-commit](https://pre-commit.com/) pour assurer la qualité de vos modifications avant de les valider dans votre dépôt (commit).

## Préparer son environnement

Peu importe votre environnement (Linux, Mac ou Windows), vous devrez :

- Installer [Docker](https://www.docker.com/get-started). Suivant votre environnement ce sera :

  - Docker Desktop pour Windows et Mac (attention une archive d'installation par système)

  - le service Docker pour Linux, via votre gestionnaire de paquet de votre distribution (yum, apt, ...)

- Installer [Visual Studio Code (VSC)](https://code.visualstudio.com/Download)

- L'extension [Remote - Containers](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers) pour VSC.
Il permet d'utiliser les conteneurs de développement que detectera VSC
en se basant sur Docker mais de manière transparente pour vous.

### Prérequis

Avoir un compte GitHub ainsi que git installé et paramétré sur votre machine.
Nous ne vous expliquerons pas ici, cherchez sur Internet si besoin.

### Clone d'un projet existant

Pour travailler sur le code localement sur votre machine,
il faut d'abord *fork* le dépôt du custom component ou celui de HA core
pour en avoir une copie sur votre compte.
Ensuite le cloner sur votre machine.

Là aussi c'est générique, nous ne détaillerons pas comment réaliser cette partie.

### Utiliser un conteneur de développement

Le dépôt de Home Assistant core ainsi que certains custom components contiennent
tous les paramétres pour vous permettre de tester vos modifications
dans une instance locale et isolée de Home Assistant.

Pour fonctionner vous devez avoir VSC, Docker et l'extension Remote container.
Lorsque vous ouvrirez le répertoire du dépôt avec VSC, il devrait detecter la
présence du conteneur (présence du repertoire `.devcontainer/`) et vous proposez d'ouvrir
le projet dans le conteneur. Si ce n'est pas le cas vous pouvez le faire manuellement
en cliquant sur le bouton vert en bas à gauce et choisir `Remote-Containers: Reopen in Container`

La première fois VSC va créer et lancer le conteneur (cela peut prendre du temps)
et installer les extensions préconnisés pour VSC par le développeur. Vous avez alors un environnement isolé et préconfiguré.

<!-- markdown-link-check-disable -->
Pour lancer l'instance d'Home Assistant dans le conteneur, allez dans VSC,
menu `Terminal`/ `Exécuter la tâches` et choisissez `Preview`.
Le serveur Home Assistant va se lancer et sera disponible à l'adresse http://localhost:8123.
<!-- markdown-link-check-enable -->

Vous pourrez relancer la tâches après avoir modifier le code,
à l'aide de la palette de commande `Tâches - Réexécuter la dernière tâche`

Il y a d'autres tâches disponbilbes pour vous aider dans votre mise au point.

## Creation d'un custom component

A VENIR

## Linting et formatage du Code

A VENIR

## Logs et Debogguage

A VENIR
