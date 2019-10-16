# Exercices
## Consigne
L'entrée peut se faire par saisie de l'utilisateur, ou simplement par initialisation d'une variable. Le résultat doit être affiché avec le formatage demandé.

## Exercice 05
>Ecrire un programme qui affiche la date courante en respectant le format.
```
Entrée : -
Sortie : Nous sommes aujourd'hui le mercredi 9 septembre 2019
```
-----------------------------------------------------
Solution possible en Javascript  :
```javascript
// date du jour
let dt = new Date(); 
// numéro du jour de 0 a 6
let jour = dt.getDay();
// numéro du mois de 0 a 11
let mois = dt.getMonth();
// l'année de la date
let annee = dt.getFullYear();

let tabJour = ["lundi", "mardi", "mercredi", "jeudi", "vendredi", "samedi", "dimanche"];
let tabMois = ["janvier", "février", "mars", "avril", "mai", "juin", 
	       "juillet", "aout", "septembre", "octobre", "novembre", "decembre"];

console.log("Nous sommes aujourd'hui le " + 
			tabJour[jour] + " " +
			jour + " " + 
			tabMois[mois] + " " + annee);
```
-----------------------------------------------------
Solution possible en Ruby (proposée par [Loic](https://github.com/EuryX) )  :
```Ruby
j = ['lundi', 'mardi', 'mercredi', 'jeudi', 'vendredi', 'samedi', 'dimanche']

m = ['janvier', 'fevrier', 'mars', 'avril', 'mai', 'juin', 
     'juillet', 'aout', 'septembre', 'octobre', 'novembre', 'decembre']

d = Time.now.strftime("Nous sommes aujourd'hui le %A %d %m %Y" )

s = d.split(" ")

if"#{s[4]}"=="Monday" then
  s[4] = j[0]

elsif"#{s[4]}"=="Tuesday" then
   s[4] = j[1]

elsif"#{s[4]}"=="Wednesday" then
   s[4] = j[2]

elsif"#{s[4]}"=="Thursday" then
   s[4] = j[3]

elsif"#{s[4]}"=="Friday" then
   s[4] = j[4]

elsif"#{s[4]}"=="Saturday" then
   s[4] = j[5]

elsif"#{s[4]}"=="Sunday" then
   s[4] = j[6]

end

v="#{s[6]}".to_i
  s[6] = m[v-1]

def r (array)
  array.join(' ').capitalize << "."
end

r(s)
```
