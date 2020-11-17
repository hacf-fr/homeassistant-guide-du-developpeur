# Travailler GitHub

Ce service est un incontournable du développement sous HA. Il a pour vocation non seulement de gérer la vie d'un développement (source, version), mais également et surtout de pouvoir fédérer des développeurs sous un même projet, et ce sans cacophonie générale.

Pour vous aider à vous familiariser avec GitHub, vous pouvez consulter ce [petit guide](https://rogerdudler.github.io/git-guide/index.fr.html) qui présente les bases (et un peu plus).

Ne soyez pas effrayé par la manipulation en ligne de commande, vous verrez que vous pourrez vous en affranchir dans Visual Studio Code (mais les bases sont à connaître!!!).

Voyons quand même quelques concepts indispensables..

## Méthodologie

- Vous voulez soumettre un bug ou faire une demande d'évolution, dans ce cas il vous faut soumettre une `issue` sur la dépôt principal.

- Vous voulez contribuer au développement (correction de bug, ajout de fonctionnalité), il vous faut alors suivre ces étapes :

  1. Le `Fork`, qui est la duplication de la branche principale (`upstream`) du dépôt du projet sur votre dépôt personnel GitHub.

  1. Le `Clone`, qui est la copie locale (sur votre PC) de votre dépôt GitHub.

  1. La branche de développement, qui est une branche sur votre dépôt (`origin`) et propre à vos modifications.

  1. Les `Commit`, qui sont les différentes modifications que vous apportez. _Ces commits doivent être le plus spécialisé possible, c'est-à-dire traiter une seule modification et non une dizaine_.

  1. Le `Pull Request`, qui sera la demande d'intégration de vos modifications auprès de la branche principale.

  1. La `Review`, qui sera la révision de vos modifications par l'équipe de développement de la branche principale. Elle peut être amenée à vous demander des modifications, refuser certaines parties, etc

  1. Le `Merge`, qui est la dernière étape et concerne l'intégration définitive de votre `Pull Request` au projet. Cette dernière étape sera du ressort de l'équipe de la branche principale.

## Les dépôts

Les dépôts sont des espaces de stockage spécifiques à un projet. Ce terme n'est pas spécifique à GitHub, vous le retrouverez pour Docker, Maven, etc

En ce qui concerne GitHub, un dépôt est associé à un profil utilisateur ou d'organisation et son adresse sera `https://github.com/`_`profil`_`/`_`projet`_

Vous pouvez avoir plusieurs dépôts de référencés dans votre copie locale. Généralement, le 1er dépôt que vous clonerez sera nommé `origin`. Vous ajouterez la branche principale `upstream` ce qui permettra de visionner les différences, remettre à jour votre base suivant ce dépôt, etc

## Bug et amélioration (Issue)

Un `issue` est tout aussi l'identification et description d'un bug que la description d'une amélioration souhaitée. Ne pas hésiter à les alimenter, que ce soit sur les projets des autres que du votre.

C'est intimement lié aux `pull request`.

## Dupliquer un projet (Fork)

Le `fork` est une copie d'un projet (autre que le votre bien souvent) en gardant toujours la référence de l'original.

L'idée ici est surtout de copier un projet sur son propre dépôt Git, de travailler tranquillement dessus, et de pouvoir transmettre vos modifications/corrections (`commit`) au dépôt d'origine via des `pull request`.

## Créer un clone local

## Faire des modifications ou ajouts

## Soumettre un correctif (Pull Request)

Enfin un `pull request` est une proposition de correction ou modification du projet, sous forme de code source ou aytres fichiers (images, etc).

## Conclusion

Ne négligez pas GitHub, il est votre meilleur ami ... mais peut apporter pas mal de confusion (perte de source, mauvais suivi, etc).

Vous avez les bases et les concepts pour entrez dans le vif du développement HA!
