# My codeFOOD for ruby !

```
variable = age_de_ruby
```

```
annee_de_ruby = 2015 - age_de_ruby
```
on peut faire un calcul avec un nomvre et une autre variable

```
message = "Bravo, tu as reçu un " + cadeau + " !"
```
on peut additionner un string avec une variable

## Les tableaux

Les tableaux permettent de ranger des données de façon ordonnée que l'on retrouve à l'aide d'un index.
Pour créer un tableau, on utilise les crochets, par exemple :
```
mes_escales_tour_du_monde = [ "Paris", "Toronto", "NYC", "Rio", "Sydney", "Hong-Kong", "Berlin" ]
```

On peut appliquer des méthodes à une variable contenant un tableau de la façon suivante :
```
nom_du_tableau.nom_de_la_methode
mes_escales_tour_du_monde.size
mes_escales_tour_du_monde.reverse
```

### accéder à un élément dans un tableau
on précise la position (ou index) de l'élément entre crochets. Par exemple,
```
mes_escales_tour_du_monde[2]
```
renverra la ville de "NYC".


### ajouter un élément dans un tableau
on utilise deux chevrons <<. Si je veux prolonger mon tour du monde à Londres, je taperai donc :
```
mes_escales_tour_du_monde << "Londres"
```

### modifier l'élément d'un tableau
on lui affecte la valeur souhaitée avec le signe =. Je peux donc remplacer Berlin par Barcelone si je parle mieux l'espagnol que l'allemand :
```
mes_escales_tour_du_monde[6] = "Barcelone"
```

## Les tables de hashage
Les tables de hashage (ou hashes) permettent de ranger des données que l'on retrouve à l'aide d'une clé.
Pour créer une table de hashage, on utilise des accolades {}. Chaque valeur rangée dans cette table est associée à une clé qui permettra de la retrouver :
```
table_de_hashage = { clé_1: valeur_1, clé_2: valeur_2, ... }
```

### Pour accéder à la valeur d'un élément dans un hash
on précise sa clé entre crochets. Si je ne me souviens plus combien de temps j'ai prévu pour mon escale à Toronto, il me suffit d'appeler :
```
jours_voyage[:toronto]
```
qui me renverra 7 jours.

### Pour ajouter ou modifier un élément dans un hash
on utilise l'opérateur =. Par exemple en ajoutant :  
```
jours_voyage[:rio] = 5
```
mon hash jours_voyage contiendra la durée de mon séjour à Rio en plus :
```
{ paris: 0, toronto: 7, nyc: 3, rio: 5 }
```

## Pour exécuter un fichier Ruby à partir de la console
placez votre console dans le répertoire contenant le fichier et tapez :
```
ruby nom_du_fichier.rb
```

### Une boucle permet d'effectuer des actions répétitives de manière simple à l'aide du mot-clé each
par exemple pour parcourir un tableau ou encore refaire plusieurs fois la même action.

Exemple de boucle pour parcourir un tableau :  
```
jours_ouvres = [
  "lundi","mardi","mercredi","jeudi","vendredi"
]

i=5

jours_ouvres.each do |jour|
  if jour == "vendredi"
    puts jour + " : Bon weekend !"
  elsif jour == "lundi"
    puts jour + " : Bon courage !"
  else
    puts jour + " : Weekend dans #{i} jours !"
  end
  i-=1
end
```
Résultat dans la console :
```
lundi : Bon courage !
mardi : Weekend dans 4 jours !
mercredi : Wekeend dans 3 jours !
jeudi : Weekend dans 2 jours !
vendredi : Bon weekend !
```
Exemple de boucle de répétition :
```
7.times do
  puts "tourner sa langue"
end
puts "... et parler !"
```
Résultat dans la console :
```
tourner sa langue
tourner sa langue
tourner sa langue
tourner sa langue
tourner sa langue
tourner sa langue
tourner sa langue
... et parler !
```

## On peut ajouter des conditions pour réaliser différentes actions dans Ruby selon le cas à l'aide des mots-clés if, else, elsif :
```
if trajet_minutes > 120
  puts "Prends un film avec toi"
elsif trajet_minutes < 5
  puts "Pas le temps de t'asseoir..."
else
  puts "Tu as le temps de lire au moins quelques chapitres d'un bouquin !"
end
```

### On peut combiner des conditions à l'aide des signes &&  (pour "ET") et || (pour "OU").

### Les booléens sont des variables utiles pour tester si une condition est vraie ou fausse.
Dans l'exemple ci-dessous, code_indenté est un booléen qui vaut "true" ou "false".
```
if code_indenté
  puts "Bravo, ton code est bien indenté !"
else
  puts "Pense à bien indenter ton code pour améliorer sa lisibilité !"
end
```
Pour vérifier une condition d'égalité, il faut utiliser deux signes égal (==). Faites attention à ne pas confondre avec le signe égal tout seul (=) qui sert à affecter une valeur à une variable :
```
age = 18 #range la valeur 18 dans la variable age et renvoie donc 18
age == 18 #booléen qui renvoie True si age vaut 18, False sinon
```


Math.sqrt
Math est un module
sqrt est la méthode
. permet de savoir qui doit recevoir le "message"

```
Math.sqrt(9)
```
Nous cherchons la racine carré du chiffre 9
Pour Ruby, ce message consiste à appeler la méthode sqrt, avec le paramètre 9, et à retourner le résultat.


def a pour role de commencer la 'def'inition d'une méthode.
```
def h (la méthode s'appellera donc h
  puts "Hello World!" (le code a executé)
 end (fin de définition de la méthode)
```

Pour donner un parametre à la méthode
```
def h(name)
 puts "Hello #{name}!"
end

h("Matz")
Hello Matz!
```

class définit plusieurs méthode
@name est une variable d'instance, c'est à dire qu'elle sera disponible pour toutes les méthodes de la class Greeter
```
class Greeter
   def initialize(name = "World")
     @name = name
   end
   def say_hi
     puts "Hi #{@name}!"
   end
   def say_bye
     puts "Bye #{@name}, come back soon."
   end
end
```

Création d'un objet de la class Greeter
```
g = Greeter.new("Pat")



