# Exercices
## Consigne
L'entrée peut se faire par saisie de l'utilisateur, ou simplement par initialisation d'une variable. Le résultat doit être affiché avec le formatage demandé.

## Exercice 04
>Ecrire un programme qui affiche les nombres pairs de 0 (inclus) à N (inclus), en respectant le format.
```
Entrée : N
Sortie : 0-2-4-6-8-10-12-14-16-20-...-N
```
Solution possible en PHP (proposée par [Julien21Julien](https://github.com/Julien21Julien) ) :
```PHP
$a = 21;

$i = 1;

for (;;) {
    if ($i > ($a*2))
        break;
    
    if ($i%2 == 0)
        echo $i.'<br />';
    
    $i++;
}
```
