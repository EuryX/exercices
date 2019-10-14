# Exercices
## Consigne
L'entrée peut se faire par saisie de l'utilisateur, ou simplement par initialisation d'une variable. Le résultat doit être affiché avec le formatage demandé.

## Exercice 03
>Ecrire un programme qui retourne la moyenne de 3 nombres, arrondie à un chiffre après la virgule.
```
Entrée : 5, 8, 12
Sortie : 12.5
```
-----------------------------------------------------
Solution possible en PHP (proposée par [Julien21Julien](https://github.com/Julien21Julien) )  :
```PHP
$a = array(5, 8, 12);
$moy = array_sum($a) / count($a);
echo round($moy, 3);
```
-----------------------------------------------------
Solution possible en Ruby (proposée par [Loic](https://github.com/EuryX) )  :
```Ruby
a = [14, 32, 27]
moy= (a.inject{ |sum, el| sum + el }.to_f / a.size).round(2)
```
-----------------------------------------------------
Solution possible en C (proposée par [Christophe](https://github.com/StickHash) ) :
```C
#include <stdio.h>

//En C pour pouvoir faire une moyenne il faut travailler avec des types double (comme en Java)

double x = 15;
double y = 10;
double z = 12;

// Il n'existe pas de fonction permettant de faire la moyenne d'un tableau en C. Il faut donc la creer
// Pour pouvoir passer un tableau en parametre d'une fonction, 
// il faut declarer le pointeur du tableau lors de la creation de la fonction
// Comme la fonction a un retour, ici un double, il faut declarer la fonction avant le "main"

double moy(double *tab , int size)
{
    int i;
    double moy;
    
    for(i = 0 ; i < size ; i++)
    {
       moy += tab[i] / size;
    }
    
    return moy;
}

int main()
{
    // Declaration et instanciation du tableau
    
    double tab[] = {x, y, z};
    
    // Pour connaitre la taille d'un tableau (son nombre d'elements), il faut la calculer
    // On divise donc la taille du tableau (en memoire) par la taille du type d'element qu'il contient
    
    int size = sizeof(tab) / sizeof(double);
    
    //Et voila!
    
    printf("la moyenne est %.1f", moy(tab, size));
    
    return 0;
}
```
