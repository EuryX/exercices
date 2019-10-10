# Exercices
## Consigne
L'entrée peut se faire par saisie de l'utilisateur, ou simplement par initialisation d'une variable. Le résultat doit être affiché avec le formatage demandé.

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
-----------------------------------------------------
Solution possible en C (proposée par [Christophe](https://github.com/StickHash) ) :
```C
#include <stdio.h>

int main()
{
    int x = 21;
    int y = 3;
    int z = 7;
    
    if (isMultiple(x, y) && isMultiple(x, z)) 
    {
        printf("%d est multiple de %d et %d", x, y, z);
    }
    else if (isMultiple(x, y))
    {
        printf("%d est multiple de %d", x, y);
    }
    else if (isMultiple(x, z))
    {
        printf("%d est multiple de %d", x, z);
    }
    else
    {
        printf("%d n'est pas multiple de %d ni de %d", x, y, z);  
    }
    return 0;
}

int isMultiple(int x, int y)
{
    return x % y == 0;
}
```
-----------------------------------------------------
Solution possible en C# (proposée par [Loic](https://github.com/EuryX) ) :
```C#
public class Program {

    public static void Main() {
    
        int n = 19;
        String message = "pas multiple de 7 ou 3";
		
        if (n % 3 == 0 && n % 7 == 0) {
            message = "multiple de 7 et de 3";	
        } else if (n % 3 == 0) {
            message = "multiple de 3";	
        } else if (n % 7 == 0) {
            message = "multiple de 7";	
        }
	
        Console.WriteLine(message);		
    }
}
```
-----------------------------------------------------
Solution possible en Ruby (proposée par [Loic](https://github.com/EuryX) ) :
```Ruby
n = 19
if n % 3 == 0 and n % 7 == 0
  puts "multiple de 3 et 7"
elsif n % 7 == 0
  puts "multiple de 7"
elsif n % 3 == 0
  puts "multiple de 3"
else
  puts "pas multiple de 3 ni de 7"
end
```
-----------------------------------------------------
Solution possible en PHP (proposée par [Julien21Julien](https://github.com/Julien21Julien) ) :
```PHP
$n=21;
Echo 'Donnez une valeur à $n';
  
 if (($n % 7 == 0) and ($n % 3 == 0)) {
  echo 'Multiple de 3 et de 7';
} elseif (($n % 3) == 0) {
     echo 'Multiple de 3';
} elseif (($n % 7) == 0){
     echo 'Multiple de 7';
} else {
  echo 'Pas de multiple de 3 et de 7';
}
```
