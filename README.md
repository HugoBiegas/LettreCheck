# LettreCheck

Convertisseur de montants en toutes lettres pour l'écriture de chèques, conforme à la réforme orthographique française de 1990.

## Fonctionnalités

- Conversion instantanée d'un montant numérique en son écriture littérale correcte
- Gestion des euros et centimes (`23,80 €` → `vingt-trois euros et quatre-vingts centimes`)
- Respect des règles d'accord de **vingt**, **cent**, **mille**, **million** et **milliard**
- Trait d'union entre tous les mots composés (réforme 1990), y compris autour de *et*
- Détail des règles orthographiques appliquées pour chaque résultat
- Exemples rapides cliquables
- Interface responsive, adaptée mobile

## Utilisation

Aucune installation ni build requis. Il suffit d'ouvrir `index.html` dans un navigateur.

```
open index.html
```

Saisissez un montant (virgule ou point acceptés comme séparateur décimal, espace accepté comme séparateur de milliers) et le résultat s'affiche immédiatement.

**Plage supportée :** `0` à `999 999 999 999,99`

## Exemples

| Saisie | Résultat |
|---|---|
| `100` | cent euros |
| `71` | soixante-et-onze euros |
| `80 000` | quatre-vingt-mille euros |
| `2 380,75` | deux-mille-trois-cent-quatre-vingts euros et soixante-quinze centimes |
| `200 000` | deux-cent-mille euros |

## Règles orthographiques couvertes

- **Trait d'union partout** (réforme 1990) : `vingt-et-un`, `deux-cent-trente-quatre`
- **Accord de *vingt*** : `quatre-vingts` (80) mais `quatre-vingt-un` (81)
- **Accord de *cent*** : `deux-cents` mais `deux-cent-trois`, `deux-cent-mille`
- **Invariabilité de *mille*** : jamais de *s* (`deux-mille`, `dix-mille`)
- **Accord de *million* / *milliard*** : noms communs, prennent un *s* au pluriel
- **« et »** uniquement pour 21, 31, 41, 51, 61 et 71 — pas pour 81 ni 91

## Stack

Application entièrement statique en un seul fichier (`index.html`), sans dépendance ni build.

- HTML / CSS / JavaScript vanilla
- Polices : [DM Serif Display](https://fonts.google.com/specimen/DM+Serif+Display), [IBM Plex Sans](https://fonts.google.com/specimen/IBM+Plex+Sans), [JetBrains Mono](https://fonts.google.com/specimen/JetBrains+Mono) via Google Fonts
