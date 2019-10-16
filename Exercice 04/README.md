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
$a=21;
for ($i = 0; $i <= $a; $i += 2) {
    echo $i.'-'; 
}
```
-----------------------------------------------------
Solution possible en Ruby (proposée par [Loic](https://github.com/EuryX) )  :
```Ruby
a = 53
for i in (0..a).step(2) do 
print "-"<<i.to_s
end
```
-----------------------------------------------------
Solution possible en Python (proposée par [Christophe](https://github.com/StickHash) ) :
```Python
n = 20
pas = 2
for nb in range(0, n, pas) :
    print("%d-" %nb, end = '')
print(n)
```
