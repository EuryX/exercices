# Exercices
## Consigne
L'entrée peut se faire par saisie de l'utilisateur, ou simplement par initialisation d'une variable. Le résultat doit être affiché avec le formatage demandé.

## Exercice 13
>Ecrire un programme converti un nombre de secondes en heures, minutes et secondes.
```
Entrée : 125
Sortie : 0h2m5s
-------------
Entrée : 3728
Sortie : 1h2m8s
```

Solution possible en Ruby (proposée par [Loic](https://github.com/EuryX) )  :
```Ruby
a = 125
s = 0
m = 0
h = 0
for i in(1..a) do
s += 1
if s == 60 then
m +=1
s = 0
if m == 60 then
h +=1
m = 0
end
end
end
puts h.to_s<<'H ' + m.to_s<<'m ' + s.to_s<<'s'
```
