# Travailler GitHub

Ce service est un incontournable du développement sous HA. Il a pour vocation non seulement de gérer la vie d'un développement (source, version), mais également et surtout de pouvoir fédérer des développeurs sous un même projet, et ce sans cacophonie générale.

Pour vous aider à vous familiariser avec GitHub, vous pouvez consulter ce [petit guide](https://rogerdudler.github.io/git-guide/index.fr.html) qui présente les bases (et un peu plus).

Ne soyez pas effrayé par la manipulation en ligne de commande, vous verrez que vous pourrez vous en affranchir dans un outil de bureau (mais les bases sont à connaître!!!).

Voyons quand même quelques concepts indispensables..

## Les outils

Voici quelques outils :

- [git](https://git-scm.com/) est l'outil minimal à installer pour gérer avec Github.
- [Git Desktop](https://desktop.github.com/) ou [Git Kraken](https://www.gitkraken.com/) va s'ajouter à `git` avec une application graphique vous simplifiant la vie.
- [VSCode](https://code.visualstudio.com/) avec ses différents composants de gestion Git, mais pas aussi poussé que les 2 clients précédents.

## Méthodologie

- Vous voulez soumettre un bug ou faire une demande d'évolution, dans ce cas il vous faut soumettre une `issue` sur le dépôt principal.

- Vous voulez contribuer au développement (correction de bug, ajout de fonctionnalité), il vous faut alors suivre ces étapes :

  1. Le `Fork`, qui est la copie de la branche principale du dépôt du projet sur votre dépôt personnel GitHub.

  1. Le `Clone`, qui est la copie locale (sur votre PC) de votre dépôt GitHub.

  1. Créer une branche de développement, qui est une branche sur votre dépôt et propre à vos modifications.

  1. Les `Commit`, qui sont les différentes modifications que vous apportez. _Ces commits doivent être le plus spécialisé possible, c'est-à-dire traiter une seule modification et non une dizaine_.

  1. La `Pull Request`, qui sera la demande d'intégration de vos modifications auprès de la branche principale.

  1. La `Review`, qui sera la révision de vos modifications par l'équipe de développement du projet. Elle peut être amenée à vous demander des modifications, refuser certaines parties, etc

  1. Le `Merge`, qui est la dernière étape et concerne l'intégration définitive de votre `Pull Request` au projet. Cette dernière étape sera du ressort de l'équipe du projet.

## Les dépôts

Les dépôts sont des espaces de stockage spécifiques à un projet. Ce terme n'est pas spécifique à GitHub, vous le retrouverez pour Docker, Maven, etc

En ce qui concerne GitHub, un dépôt est associé à un profil utilisateur ou d'organisation et son adresse sera `https://github.com/`_`profil`_`/`_`projet`_

Vous pouvez avoir plusieurs dépôts de référencés dans votre copie locale. Généralement, le 1er dépôt que vous clonerez sera nommé `origin` et sera lié à votre dépôt personnel. Vous ajouterez le dépôt principale du projet, le `upstream`, ce qui permettra de visionner les différences, remettre à jour votre base suivant ce dépôt, etc

## Bug et amélioration (Issue)

Un `issue` est tout aussi l'identification et description d'un bug que la description d'une amélioration souhaitée. Ne pas hésiter à alimenter, que ce soit sur les projets des autres que du votre.

C'est intimement lié aux `pull request`.

## Dupliquer un projet (Fork)

Le `fork` est une copie d'un projet (autre que le votre normalement) en gardant toujours la référence de l'original.

L'idée ici est surtout de copier un projet sur son dépôt Git personnel, de travailler tranquillement dessus, et de pouvoir transmettre vos modifications/corrections (`commit`) au dépôt d'origine via des `pull request`.

## Créer un clone local

Une fois le `fork` réalisé sur votre dépôt github personnel, vous devez créer une copie local (sur votre machine) de ce dépôt.

C'est sur cette copie locale que vous travaillerez : développer, réaliser des `commit` et les pousser régulièrement sur votre dépôt.

## Faire des modifications ou ajouts

Les modifications sont les `commit`. Le principe au sujet des `commit`est de les faire petit, lié à une correction ou un ajout minimaliste.

## Soumettre un correctif (Pull Request)

Enfin un `pull request` est une proposition de correction ou modification du projet, sous forme de code source ou autres fichiers (images, etc).

## Conclusion

Ne négligez pas GitHub, il est votre meilleur ami ... mais peut apporter pas mal de confusion (corruption de source, mauvais commentaires, etc).

Vous avez les bases et les concepts pour entrez dans le vif du développement HA!
