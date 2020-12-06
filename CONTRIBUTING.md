# Instructions pour contribuer

## Pour tester la génération du site statique

Ce dépôt utilisée pour générer un site web statique à l'aide de [Mkdocs](https://www.mkdocs.org/).

Pour tester en local la génération vous avez besoin d'installer [nox](https://nox.thea.codes/en/stable/)
au préalable.
Ensuite nox s'occupe d'installer toutes les dépendances nécessaires
dans un environnement virtuel:

`$ nox -s docs`

Cette commande a deux comportements:

- En mode interactif (typiquement quand vous lancez la commande dans votre terminal),
  elle génère le contenu du site statique
  et lance un serveur pour le consulter à l'aide de son navigateur en consultant l'URL `http://127.0.0.1:8000/`
- En mode non-interactif (dans un script de _Continuous Integration_ par exemple),
  elle génère le contenu du site statique dans le répertoire `site`.
