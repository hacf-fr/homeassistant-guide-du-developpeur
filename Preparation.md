# Préparation de votre environnement

Pour développer sous Home Assistant, il vous faut un environnement de développement spécifique.

Nous vous présentons 2 environnements possibles pour vos développements :

- Un environnement avec Docker
- Un environnement virtuel avec Python

Dans les 2 cas [Visual Studio Code](https://code.visualstudio.com/) (VSCode) sera l'outil de développement.

## Environnement Docker

Cet environnement utilise docker et l'extension [Remote - container](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers) de VSCode.

## Environnement Python

L'avantage de cet environnement est que vous pouvez le faire sans module d'accès à un environnement distant.

Vous devrez par contre avoir un environnement type Linux comme un de ceux-ci :

- Une station Linux native
- Un Windows avec WSL2 (avec Ubuntu ou autre distribution, vous adapterez les commandes)
- un Mac (avec Homebrew)

### Préparation github

Les sources des composants de Home Assistant sont disponibles sur github mais vous n'allez pas travailler directement avec le dépôt officiel. La bonne pratique est de faire un copie (fork) sur votre compte github et ensuite travailler dessus.

### Structure fichiers

Si vous voulez travailler une intégration ou un composant natifs alors la clone du Core en local sera suffisant.

Par contre si vous voulez travailler
Pour travailler vous devrez avoir une base pour Home Assistant et autant de base pour vos développements (ce que j'appelle base est tout simplement un dossier :) ).

Le principe est de faire des liens de vos développements dans l'arborescence de Home Assistant, vos développements étant sous Git cela simplifiera les choses de les avoir en dehors du dossier HA.

Exemple de structure où j'ai 2 développements en cours et une base de home assistant

    /home/myuser/homeassistant
        |- /dev1
        |- /dev2
        |- /core
            |- /config/custom_components/dev1
            |- /config/custom_components/dev2

### Installer sous Linux

L'exécution de Home Assistant nécessite d'installer les dépendences :

    sudo apt-get install python3-pip python3-dev python3-venv autoconf libssl-dev libxml2-dev libxslt1-dev libjpeg-dev libffi-dev libudev-dev zlib1g-dev pkg-config libavformat-dev libavcodec-dev libavdevice-dev libavutil-dev libswscale-dev libavresample-dev libavfilter-dev ffmpeg

Cloner le dépôt officiel Core de Home Assistant sur votre Github, puis récupérer en local avec Git :

    cd ~/homeassistant
    git clone https://github.com/YOUR_GIT_USERNAME/core.git
    cd core
    git remote add upstream https://github.com/home-assistant/core.git

Démarrer Home Assistant :

    hass -c config

**ATTENTION, ne fermez pas votre session sinon vous tuez le process en cours !**

Vous pouvez maintenant vous y connecter pour la 1ère configuration sur <http://localhost:8123/>

### Installer sous Windows

Vous devez activer WSL2, installer une distribution Linux comme Ubuntu ... et suivre la procédure d'installation sous Linux ;)

### Installer sous Mac OS

TODO
