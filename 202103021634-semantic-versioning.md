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

## Ressources

- [spécification](https://semver.org/)
- [sentimental versioning](http://sentimentalversioning.org/) – gentil troll de semver
