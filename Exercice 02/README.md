# Exercices
## Consigne
L'entrée peut se faire par saisie de l'utilisateur, ou simplement par initialisation d'une variable. Le résultat doit être affiché avec le formatage demandé.

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
-----------------------------------------------------
Solution possible en Java (proposée par Nans )  :
```java
public class Demo {
    public static void main(String[] args) {

        int minInterval1 = 0;
        int maxInterval1 = 100;
        int maxInterval2 = 200;
        int saisie = 50;
        String message = "Votre saisie doit être comprise entre 0 et 200.";

        if (saisie >= minInterval1 && saisie <= maxInterval1) {
            message = "Intervalle 0 à 100";
        } else if (saisie > maxInterval1 && saisie <= maxInterval2) {
            message = "Intervalle 101 à 200";
        }
        System.out.println(message);

    }
}
```
-----------------------------------------------------
Solution possible en Javascript :
```javascript
let n = 80;
message = (n >= 0 && n <= 200) ? (n <= 100) ? "Intervalle 0 à 100" : "Intervalle 100 à 200" : "Choisir un nombre entre 0 et 200";
console.log(message);
```
-----------------------------------------------------
Solution possible en python (proposée par [Loic](https://github.com/EuryX) )  :
```python
n = 2
message = "choisir un nombre entre 0 et 200"
if (n >= 0) and (n <= 100):
   message = "Intervalle 0 à 100"
elif(n >= 101) and (n <= 200):
    message = "Intervalle 101 à 200"
print(message)
```
-----------------------------------------------------
Solution possible en Ruby (proposée par [Loic](https://github.com/EuryX) )  :
```Ruby
n = 190
if n >= 0 and n <= 100
  mess = "intervalle 0 a 100"
elsif n >= 101 and n <= 200
  mess = "intervalle 101 a 200"
else 
  mess = "choisir un nombre entre 0 et 200"
puts mess
end
```
-----------------------------------------------------
Solution possible en PHP (proposée par [Julien21Julien](https://github.com/Julien21Julien) )  :
```PHP
$n=15;

if (($n >= 0) and ($n <= 100)) {
   echo 'Intervalle 0 à 100';
} elseif (($n >= 101) and ($n <= 200)) {
    echo 'Intervalle 101 à 200';
}
```
-----------------------------------------------------
Solution possible en C (proposée par [Christophe](https://github.com/StickHash) ) :
```C
#include <stdio.h>

int x = 0;
int y = 100;
int z = 200;
int n = 85;

int main()
{
    if(n < x || n > z)
    {
        printf("%d est hors plage. Le nombre doit être compris entre %d et %d",n,x,z);
    }
    else if(n > y)
    {
        printf("%d est compris entre %d et %d",n,y+1,z);
    }
    else
    {
       printf("%d est compris entre %d et %d",n,x,y); 
    }
    return 0;
}
```
