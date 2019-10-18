# Exercices
## Consigne
L'entrée peut se faire par saisie de l'utilisateur, ou simplement par initialisation d'une variable. Le résultat doit être affiché avec le formatage demandé.

## Exercice 07
>Ecrire un programme qui retourne un mot avec alternativement des lettre en majuscule et en minuscule.
```
Entrée : gourmandise
Sortie : GoUrMaNdIsE
```

Solution possible en Ruby (proposée par [Loic](https://github.com/EuryX) )  :
```Ruby
a = 'gourmandise'
b = a.chars
for i in (0..a.length).step(2) do 
b[i] = b[i].upcase
end
a = b.join()
print a
```
