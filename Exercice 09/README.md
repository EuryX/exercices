# Exercices
## Consigne
L'entrée peut se faire par saisie de l'utilisateur, ou simplement par initialisation d'une variable. Le résultat doit être affiché avec le formatage demandé.

## Exercice 09
>Ecrire un programme qui raccourci une chaîne caractère et retourne uiquement les trois premiers et les trois derniers caractères, séparés par trois points.
```
Entrée : neptune est une planète éloignée de la terre
Sortie : nep...rre
```

Solution possible en Ruby (proposée par [Loic](https://github.com/EuryX) )  :
```Ruby
a = 'neptune est une planète éloignée de la terre'
b = a.chars
puts b[0] + b[1] + b[2] + '...' + b[a.length-3] + b[a.length-2] + b[a.length-1]
```
