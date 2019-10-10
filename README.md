# Exercices
## Consigne
L'entrée peut se faire par saisie de l'utilisateur, ou simplement par initialisation d'une variable. Le résultat doit être affiché avec le formatage demandé.

## Ressources

Pour participer sans installer d'outils, vous pouvez utiliser ces interpréteurs en ligne :

python en ligne :
https://repl.it/languages/python3

documentation officielle :
https://docs.python.org/fr/3/

php en ligne :
http://www.writephponline.com

documentation officielle :
https://www.php.net/manual/fr/


## Exercice exemple :
>Ecrire un programme qui additionne deux nombres saisis.
```
Entrée : 14 6
Sortie : 20
```

Réponse possible en python :
```python
n = [14, 6]
print(sum(n))
```
Réponse possible en javascript :
```javascript
const n = [14, 6];
console.log(n.reduce((a, b) => a + b, 0));
```
Réponse possible en php :
```php
$n = [14, 6];
echo array_sum($n);
```

## Exercice 01
>Ecrire un programme qui indique si le nombre saisi est un multiple de 3 ou de 7.
```
Entrée : 14
Sortie : Multiple de 7
-------------
Entrée : 21
Sortie : Multiple de 3 et de 7
-------------
Entrée : 18
Sortie : Multiple de 3
```
-----------------------------------------------------
Solution possible en python :
```python
n = 21
message = "Pas multiple de 7 ou 3"
if (n % 7 == 0) and (n % 3 == 0):
  message = "Multiple de 3 et de 7"
else:
  if n % 3 == 0:
    message = "Multiple de 3"
  if n % 7 == 0:
    message = "Multiple de 7"

print(message)
```
-----------------------------------------------------
Solution possible en javascript :
```javascript
let n = 21;
let message = "Pas multiple de 7 ou 3";
if (n % 7 == 0 && n % 3 == 0) {
    message = "Multiple de 3 et de 7";
} else {
    if (n % 3 == 0) {
        message = "Multiple de 3";
    }
    if (n % 7 == 0) {
        message = "Multiple de 7";
    }
}
console.log(message);
```
-----------------------------------------------------
Solution possible en java (proposée par Nans) :
```java
public class Demo {
    public static void main(String[] args) {
        int saisie = 8;
        String resultat = "Ce chiffre n'est un multiple ni de 3 ni de 7";
    
        if (saisie % 3 == 0 && saisie % 7 == 0) {
            resultat = "Ce chiffre est un multiple de 3 et de 7";
        } else if (saisie % 3 == 0) {
            resultat = "Ce chiffre est un multiple de 3";
        } else if (saisie % 7 == 0) {
            resultat = "Ce chiffre est un multiple de  7";
        }
        System.out.println(resultat);
    }
}
```


## Exercice 02
>Ecrire un programme qui indique l'intervalle dans lequel se situe le nombre saisi.
>Les deux intervalles sont : 0 à 100 et 101 à 200.
```
Entrée : 85
Sortie : Intervalle 0 à 100
-------------
Entrée : 156
Sortie : Intervalle 101 à 200
```

## Exercice 03
>Ecrire un programme qui retourne la moyenne de 3 nombres, arrondie à un chiffre après la virgule.
```
Entrée : 5, 8, 12
Sortie : 12.5
```

## Exercice 04
>Ecrire un programme qui affiche les nombres pairs de 0 (inclus) à N (inclus), en respectant le format.
```
Entrée : N
Sortie : 0-2-4-6-8-10-12-14-16-20-...-N
```

## Exercice 05
>Ecrire un programme qui affiche la date courante en respectant le format.
```
Entrée : -
Sortie : Nous sommes aujourd'hui le mercredi 9 septembre 2019
```

## Exercice 06
>Ecrire un programme qui renvoi le maximum parmi 3 entiers saisis.
```
Entrée : 12, 8, 41
Sortie : 41
```

## Exercice 07
>Ecrire un programme qui retourne un mot avec alternativement des lettre en majuscule et en minuscule.
```
Entrée : gourmandise
Sortie : GoUrMaNdIsE
```

## Exercice 08
>Ecrire un programme qui enlève toutes les voyelles d'un mot saisie.
```
Entrée : neptune
Sortie : nptn
```

## Exercice 09
>Ecrire un programme qui raccourci une chaîne caractère et retourne uiquement les trois premiers et les trois derniers caractères, séparés par trois points.
```
Entrée : neptune est une planète éloignée de la terre
Sortie : nep...rre
```

## Exercice 10
>Ecrire un programme qui retourne l'âge à partir d'une date de naissance saisie.
```
Entrée : 10/08/1988
Sortie : 31
```

## Exercice 11
>Ecrire un programme qui retourne un mot inversé.
```
Entrée : maison
Sortie : nosiam
```

## Exercice 12
>Ecrire un programme qui valide si un mot saisi est composé uniquement de caractères alphanumériques.
```
Entrée : sangoku
Sortie : ok
-------------
Entrée : san!goku
Sortie : nok
```

## Exercice 13
>Ecrire un programme converti un nombre de secondes en heures, minutes et secondes.
```
Entrée : 125
Sortie : 0h2m5s
-------------
Entrée : 3728
Sortie : 1h2m8s
```

## Exercice 14
>Ecrire un programme qui détermine si un mot est un palyndrome ou non.
```
Entrée : kayak
Sortie : palyndrome
-------------
Entrée : voiture
Sortie : pas palyndrome
```
