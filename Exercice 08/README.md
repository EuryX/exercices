# Exercices
## Consigne
L'entrée peut se faire par saisie de l'utilisateur, ou simplement par initialisation d'une variable. Le résultat doit être affiché avec le formatage demandé.

## Exercice 08
>Ecrire un programme qui enlève toutes les voyelles d'un mot saisie.
```
Entrée : neptune
Sortie : nptn
```
Solution possible en Ruby (proposée par [Loic](https://github.com/EuryX) )  :
```Ruby
a = 'neptune'
b = a.chars
c = ['a','e','i','o','u','y']
for i in (0..a.length) do 
  if c.include? b[i] then
  b[i] = ''
end
end
a = b.join()
puts a

```
