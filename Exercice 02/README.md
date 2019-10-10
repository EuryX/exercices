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
