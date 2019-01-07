# Ceci est mon code FOOD pour CSS

On crée un fichier CSS souvent nommé style.css
On le link à notre fichier html dans la balise <head>
La balise est
```
<link rel="style.css" href="style.css" />
```

## selectionné les balises et donner leur des propriétés css

exemple :
```
p
{
    color: blue;
}
```

- selection de la balise : p
- propriété css donné : couleur
- valeur : ici le bleu

la couleur des paragraphes sera bleu


exemple général :
```
balise1
{
    propriete1: valeur1;
    propriete2: valeur2;
    propriete3: valeur3;
}

balise2
{
    propriete1: valeur1;
    propriete2: valeur2;
    propriete3: valeur3;
    propriete4: valeur4;
}

balise3
{
    propriete1: valeur1;
}
```

## on peut aussi selectionné plusieurs balises
```
h1, p, em
{
    propriete1: valeur1;
    propriete2: valeur2;
    propriete3: valeur3;
}
```

## commentaires dans CSS
```
/*
mon commentaire
*/
```


## Attribut : class=""

Permet de cibler quelles balises vont avoir quels changements

exemple :

Dans html :
```
 <p class="introduction">Bonjour et bienvenue sur mon site !</p>
```

Dans css
```
.intriduction
{
  color: blue;
}
```

Ce qui permet d'attribuer des class à plusieurs balises.

## Balise universelle pour donner des attribut à tout ce qu'on veut

Balise block
```
<div> </div>
```

Balise inline (pour un mot par exemple)
```
<span></span>
```


## Sélecteur avancé

Sélectionne toutes les balises

```
*
{

}
```

## A + B : une balise qui en suit une autre
```
h3 + p
{

}
```

## A[attribut] : une balise qui possède un attribut`
Sélectionne tous les liens<a>qui possèdent un attribut title.
```
a[title]
{

}
```

Exemple :
```
<a href="http://site.com" title="Infobulle">
```

## A[attribut="Valeur"] : une balise, un attribut et une valeur exacte
```
a[title="Cliquez ici"]
{

}
```
Idem, mais l'attribut doit en plus avoir exactement pour valeur « Cliquez ici ».

## A[attribut*="Valeur"] : une balise, un attribut et une valeur

```
a[title*="ici"]
{

}
```
Idem, l'attribut doit cette fois contenir dans sa valeur le mot « ici » (peu importe sa position).
