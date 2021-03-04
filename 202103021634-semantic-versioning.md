---
aliases: [SemVer]
---

# Semantic versioning

#versioning

Procédé de montée en version qui indique le niveau de changement apporté dans le code.

## Principe

Utilise le format `MAJEURE.MINEURE.PATCH` de la manière suivante :

| Numéro    | Utilisation                       |
| --------- | --------------------------------- |
| `MAJEURE` | Changement non rétrocompatible    |
| `MINEURE` | Changement rétrocompatible        |
| `PATCH`   | Correction de bug rétrocompatible |

L'incrément d'un numéro entraîne la remise à 0 des numéro suivants :

```
0.11.0 + MAJEURE = 1.0.0
2.0.6  + MINEURE = 2.1.0
1.42.2 + PATCH   = 1.42.3
```

## Première release

Au démarrage d'un projet, la majeure porte le chiffre 0. C'est la première phase de développement. Au cours de cette période, la rétrocompatibilité n'est pas garantie.

Une fois la première version stable atteinte, on incrémente la majeure, qui porte alors le chiffre 1.

## Limite

Il faut parfois se méfier des promesses faites au travers de SemVer. Même s'il est de bonne volonté, le mainteneur est toujours susceptible de commettre une erreur qui va casser le code intégrant sa librairie.

En ce sens, [Hynek Schlawack](https://hynek.me/articles/semver-will-not-save-you/) qualifie SemVer de TL;DR du changelog :

> Knowing the *intentions* of a maintainer can be valuable – especially *when* things break. Because that’s all *SemVer* is: **a TL;DR of the changelog**.

## Ressources

- [spécification](https://semver.org/)
- [sentimental versioning](http://sentimentalversioning.org/) – gentil troll de semver
