# Voting Systems Comparison
FR only - Pourquoi le mode de scrutin de votre pays n'est pas le meilleur

![](https://img.shields.io/badge/language-French-blue) ![](https://img.shields.io/badge/status-In_progress-green) ![](https://img.shields.io/badge/type-Read_only-green) ![](https://img.shields.io/github/last-commit/Relex12/Languages)

---

## Sommaire
[TOC]

## Introduction

Dans ce document, nous allons faire un état de l'art des méthodes de scrutin qui existent et qui sont pratiquées dans le monde. A partir de là, nous allons élaborer des critères qui rendent les méthodes de scrutin plus ou moins performantes, et enfin nous pourrons conclure sur le meilleur système électoral.

**Pourquoi ce sujet est-il important** : plus qu'important, la méthode de scrutin, système électoral ou régime électoral, devrait être une priorité pour toutes républiques. Il s'agit de réaliser un vote selon une méthode qui soit la plus représentative possible de l'opinion des électeurs. Chaque électeur possède une opinion très complexe de la situation politique à laquelle son pays fait face, et rendre compte de manière fidèle cette opinion n'est pas chose aisée.

**Nous allons donc nous intéresser à la meilleure façon de représenter l'opinion de l'électeur, et créer le bulletin de vote "parfait".**

Quelles sont les méthodes de scrutin qui ont existent, quels sont les défaults et les qualités de chacune de ces méthodes, qu'est-ce qui est utilisé en pratique dans le monde ? De nombreuses questions auxquelles nous allons tenter de répondre.



## Contexte

Pour commencer, voici deux définitions sur lesquelles se mettre d'accord :

* La **démocratie** est un régime politique dans lequel tous les citoyens participent aux désicions politiques, par exemple par le vote. Les citoyens exercent alors un **contrôle** sur leurs dirigeants. Pour autant, l'influence des citoyens sur la politique peut être plus ou moins présente : on distingue la démocratie **directe**, dans laquelle les citoyens votent les lois, de la démocratie **représentative**, où les citoyens éluent des représentants qui votent les lois. Attention aussi : les **citoyens** forment un ensemble plus restreint que le **peuple**, qui lui désigne l'ensemble de la population.
* La **république** est un mode de gouvernement dans lequel le pouvoir est exercé par des élus. Les **élus** ne représentent pas nécessairement l'ensemble du peuple, il est possible que seule une partie du peuple, choisit selon un critère idéologique, social, politique ou religieux.

On différencie aussi les scrutins selon le nombre de personnes qui peuvent être élues grâce à une seule élection : 

* un scrutin **uninominal** permet d'élire une seule personne parmi les candidats
* un scrutin **plurinominal** permet d'élire plusieurs personnes parmi les candidats



## Cadre de travail

Dans ce document, nous allons uniquement nous intéresser aux méthodes de scrutin uninominales. On va donc parcourir les méthodes qui permettent de choisir un unique vainqueur parmi plusieurs candidats selon diverses manières de présenter le bulletin de vote des électeurs. 



## Méthodes de scrutin

### Scrutin uninominal majoritaire

Dans un scrutin uninominal majoritaire, chaque électeur vote pour le candidat qu'il préfère voir élu. Le scrutin majoritaire peut se passer en plusieurs tours, on élimine alors à chaque tour un certain nombre de candidats, puis on refait un tour, ainsi de suite jusqu'à obtenir un seul candidat vainqueur. 

Le bulletin de vote se présente sous la forme d'un unique nom à glisser dans une urne, généralement dans une enveloppe pour garantir la confidentialité du vote. 

Le dépouillement consiste à compter pour chaque candidat le nombre de voix exprimées en sa faveur, on convertit ça le plus souvent en pourcentage de voix exprimées. Les candidats avec le moins de voix sont éliminés, et si nécessaire on procède à un nouveau scrutin avec les candidats restants. 

#### À un tour

#### À deux tours

#### À N tours (élimination au tour par tour)

### Préférences multiples ordonnées

Les préférences multiples ordonnées décrivent un ensemble de méthodes d'évaluation de l'ordre de préférence entres les candidats par les électeurs. La dénomination regroupe des méthodes de scrutin qui sont différentes et nombreuses, potentiellement infinies. 

Le bulletin de vote ressemble à une liste des candidats, l'électeur doit inscrire en face de chaque des candidats le numéro correspondant à la position du candidat dans son ordre de préférence, c'est-à-dire chaque numéro doit être unique et compris entre 1 et N inclus. 

| Candidats  | Ordre |
| :--------: | :---: |
| candidat A |       |
| candidat B |       |
| candidat C |       |

Exemple de bulletin vierge possible avec trois candidats.

Pour le dépouillement, on représente les résultats sous forme de tableau : la première colonne contient le nombre ou le pourcentage de voix qui ont adhéré à l'ordre qui est décrit dans les autres colonnes. Il y a N autres colonnes, indiquant pour chaque ligne la position d'un candidat dans l'ordre associé à la ligne.

| Pourcentage de voix exprimées | candidat A | candidat B | candidat C |
| :---------------------------: | :--------: | :--------: | :--------: |
|             30 %              |     1      |     2      |     3      |
|             30 %              |     3      |     2      |     1      |
|             20 %              |     2      |     1      |     3      |
|             20 %              |     2      |     3      |     1      |

Exemple de résultat pour le scrutin associé au bulletin ci-dessus. Ici, les ordres `A > C > B` et `C > A > B` n'ont reçu aucune voix et ne sont pas représentés.

La notation `A > B > C` se lit `A arrive avant B, et B arrive avant C`.

En pratique, le nombre de candidats peut limiter grandement l'intérêt d'une telle représentation, car le nombre d'ordres possible entre les candidats suit la fonction factorielle, c'est-à-dire que s'il y a N candidats, le tableau synthétique possède N ! lignes.

**Comment évaluer ces résultats ?**

Les préférences multiples ordonnées consistent donc en différentes manières de sélectionner un candidat vainqueur à partir du tableau des résultats tel que défini ci-dessous.

On remarque au passage que les méthodes par scrutin majoritaire sont un cas particulier de système à préférences multiples ordonnées, dans laquelle, pour un scrutin à  à N tours, on ne garderait que les N premières positions données sur le bulletin de vote. 

#### Vote alternatif

#### Méthode de Condorcet (combats 1v1)

#### Méthode de Borda (n points au premier)

#### Panachage

### Vote pondéré

### Vote par valeur

Le vote par valeur est une famille de méthodes de scrutin qui permet aux électeurs de donner une valeur à chaque candidat sur une échelle à plusieurs palier. La taille de l'échelle utilisée d'une méthode à l'autre, mais l'échelle est la même pour tous les électeurs (même taille et mêmes valeurs). Les valeurs de l'échelle peuvent être numériques ou verbales, par exemple "12/20" ou "Acceptable", on peut aussi parler de note et de mentions. 

Les systèmes de vote par valeur diffèrent des systèmes à préférences multiples ordonnées vues précédemment car ils ne consistent pas à trier les candidats mais à les juger chacun individuellement. 

Le bulletin de vote est identique à celui utilisé pour les systèmes à préférences multiples ordonnées : on présente la liste de tous les candidats, et pour chaque candidat l'électeur attribue la mention qu'il souhaite. 



| Candidats  | Note  |
| :--------: | :---: |
| candidat A | 18/20 |
| candidat B | 05/20 |
| candidat C | 12/20 |

Exemple de bulletin de vote rempli avec trois candidats, sur une échelle numérique de 0 à 20.

| Candidats  |  Ordre   |
| :--------: | :------: |
| candidat A | Supporte |
| candidat B |  Oppose  |
| candidat C |  Neutre  |

Exemple de bulletin de vote rempli avec trois candidats, sur une échelle verbale avec les mentions `Supporte`, `Neutre` et `Oppose`.



Pour le dépouillement, il n'existe pas de consensus sur la manière de représenter les résultats, mais il est possible de le faire de la manière suivante :

<!-- insérer l'explication et un exemple -->

Une fois le dépouillement réalisé, il existe deux manières de déterminer un vainqueur, sans compter les variantes :

* la méthode de la somme 
* la méthode de meilleur médiane

<!-- insérer explication et variantes --> 

#### Vote par approbation

#### Vote par note

#### Jugement majoritaire





## Problèmes

### présences d'autres "petits candidats"

### vote utile ou protestataire : stratégique

### un seul avis exprimé

### Paradoxe d'arrow (+ de voies - de chances)

### éventuelle indécidabilité

### critère de condorcet



## Tableau comparatif



## Théorème d'impossibilité

### Classement

### Jugement

<!--		par approbation, par note, par mention -> jugement majoritaire		-->

## Dans le monde

![world](https://upload.wikimedia.org/wikipedia/commons/f/f8/Electoral_systems_map.svg)

## Conclusion





## Crédits

**Section à reformuler.**

Informations :

* [Wikipédia - Système électoral](https://fr.wikipedia.org/wiki/Syst%C3%A8me_%C3%A9lectoral)
* [ScienceEtonnante - Réformons l'élection présidentielle !](https://www.youtube.com/watch?v=ZoGH7d51bvc)
* [La statistique expliquée à mon chat - Monsieur le président, avez-vous vraiment gagné cette élection ?](https://www.youtube.com/watch?v=vfTJ4vmIsO4)

Illustrations :

* [Wikipédia - Système électoral](https://fr.wikipedia.org/wiki/Système_électoral)

Voir aussi :
* https://democracychronicles.org/12-best-voting-systems/
