# Exercices
## Consigne
L'entrée peut se faire par saisie de l'utilisateur, ou simplement par initialisation d'une variable. Le résultat doit être affiché avec le formatage demandé.

## Exercice 10
>Ecrire un programme qui retourne l'âge à partir d'une date de naissance saisie.
```
Entrée : 10/08/1988
Sortie : 31
```

Solution possible en Ruby (proposée par [Loic](https://github.com/EuryX) )  :
```Ruby
require 'date'
a = "10/08/1988"
b = Date::strptime(a, "%d/%m/%Y")
c = Time.now.utc.to_date
  c.year - b.year - ((c.month > b.month || (c.month == b.month && c.day >= b.day)) ? 0 : 1)
```
