# Exercices
## Consigne
L'entrée peut se faire par saisie de l'utilisateur, ou simplement par initialisation d'une variable. Le résultat doit être affiché avec le formatage demandé.

## Exercice 05
>Ecrire un programme qui affiche la date courante en respectant le format.
```
Entrée : -
Sortie : Nous sommes aujourd'hui le mercredi 9 septembre 2019
```

Solution possible en Ruby (proposée par [Loic](https://github.com/EuryX) )  :
```Ruby
d = Time.now.strftime("Nous sommes aujourd'hui le %A %d %B %Y" )

s = d.split(" ")

if"#{s[4]}"=="Monday" then
  s[4] = "Lundi"

elsif"#{s[4]}"=="Tuesday" then
  s[4] = "Mardi"

elsif"#{s[4]}"=="Wednesday" then
  s[4] = "Mercredi"

elsif"#{s[4]}"=="Thursday" then
  s[4] = "Jeudi"

elsif"#{s[4]}"=="Friday" then
  s[4] = "Vendredi"

elsif"#{s[4]}"=="Saturday" then
  s[4] = "Samedi"

elsif"#{s[4]}"=="Sunday" then
  s[4] = "Dimanche"

end

if"#{s[6]}"=="January" then
  s[6] = "Janvier"

elsif"#{s[6]}"=="February" then
  s[6] = "Fevrier"

elsif"#{s[6]}"=="March" then
  s[6] = "Mars"

elsif"#{s[6]}"=="April" then
  s[6] = "Avril"

elsif"#{s[6]}"=="May" then
  s[6] = "Mai"

elsif"#{s[6]}"=="June" then
  s[6] = "Juin"

elsif"#{s[6]}"=="July" then
  s[6] = "Juillet"

elsif"#{s[6]}"=="August" then
  s[6] = "Aout"

elsif"#{s[6]}"=="September" then
  s[6] = "Septembre"

elsif"#{s[6]}"=="October" then
  s[6] = "Octobre"

elsif"#{s[6]}"=="November" then
  s[6] = "Novembre"

elsif"#{s[6]}"=="December" then
  s[6] = "Decembre"
  
end

def r (array)
  array.join(' ').capitalize << "."
end

r(s)
```
