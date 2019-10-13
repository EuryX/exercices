# Exercices
## Consigne
L'entrée peut se faire par saisie de l'utilisateur, ou simplement par initialisation d'une variable. Le résultat doit être affiché avec le formatage demandé.

## Exercice 03
>Ecrire un programme qui retourne la moyenne de 3 nombres, arrondie à un chiffre après la virgule.
```
Entrée : 5, 8, 12
Sortie : 12.5
```

Solution possible en PHP (proposée par [Julien21Julien](https://github.com/Julien21Julien) )  :
```PHP
$a=array (5,8,12);

$moy=array_sum($a) / count($a);


echo round($moy, 3);
```
