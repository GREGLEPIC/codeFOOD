# My Code FOOD pour HTML


## Structure de base d'une page HTML5
```
<!DOCTYPE html>
<html>
    <head>
        <meta charset="utf-8" />
        <title>Titre</title>
    </head>

    <body>

    </body>
</html>
```


## Créer un commentaire
```
<!-- Ceci est un commentaire -->
```


## Créer un paragraphe dans body
```
<p>Bonjour et bienvenue sur mon site !</p>
```


## Aligner à la ligne
```
Balise orpheline </br >
```


## Les titres
```
<h1> </h1>: signifie « titre très important ». En général, on s'en sert pour afficher le titre de la page au début de celle-ci.

<h2> </h2>: signifie « titre important ».

<h3> </h3>: pareil, c'est un titre un peu moins important (on peut dire un « sous-titre » si vous voulez).

<h4> </h4>: titre encore moins important.

<h5> </h5>: titre pas important.

<h6> </h6>: titre vraiment, mais alors là vraiment pas important du tout.
```
```
<!DOCTYPE html>
<html>
    <head>
        <meta charset="utf-8" />
        <title>Niveaux de titres</title>
    </head>

    <body>
        <h1>Titre super important</h1>
        <h2>Titre important</h2>
        <h3>Titre un peu moins important (sous-titre)</h3>

        <h4>Titre pas trop important</h4>
        <h5>Titre pas important</h5>
        <h6>Titre vraiment pas important du tout</h6>
    </body>
</html>
```


## Mise en valeur de certains mots

### italique
```
<em> </em>
```


### Gras
```
<strong></strong>
```

## Les listes

### liste à points
```
<ul>
    <li>Fraises</li>
    <li>Framboises</li>
    <li>Cerises</li>
</ul>
```


### liste à chiffres
```
<ol>
    <li>Fraises</li>
    <li>Framboises</li>
    <li>Cerises</li>
</àl>
```

## Créer des liens
```
<a href="page2.html">OpenClassrooms</a>
```
on peut insérer cette balise dans un titre, un paragraphe.
Le lien peut envoyer vers un autre site, une autre page de notre site ou ça peut être un lien de téléchargement.

IMPORTANT : si c'est une autre page de notre site, bien faire attention à afficher le bon lien.
si les pages sont dans le même dossier juste mettre : page2.HTML
si la nouvelle page est dans un autre dossier, juste mettre : dossier/page2.HTML


## Créer un lien vers une ancre

Une ancre est une sorte de point de repère que vous pouvez mettre dans vos pages HTML lorsqu'elles sont très longues.
En effet, il peut alors être utile de faire un lien amenant plus bas dans la même page pour que le visiteur puisse sauter directement à la partie qui l'intéresse.

Pour créer une ancre, il suffit de rajouter l'attributidà une balise qui va alors servir de repère. Ce peut être n'importe quelle balise, un titre par exemple.
Utilisez l'attribut id pour donner un nom à l'ancre. Cela nous servira ensuite pour faire un lien vers cette ancre. Par exemple :
```
<h2 id="mon_ancre">Titre</h2>
```
Ensuite, il suffit de créer un lien comme d'habitude, mais cette fois l'attributhrefcontiendra un dièse (#) suivi du nom de l'ancre. Exemple :
```
<a href="#mon_ancre">Aller vers l'ancre</a>
```
Normalement, si vous cliquez sur le lien, cela vous amènera plus bas dans la même page (à condition que la page comporte suffisamment de texte pour que les barres de défilement se déplacent automatiquement).
Voici un exemple de page comportant beaucoup de texte et utilisant les ancres (j'ai mis n'importe quoi dans le texte pour remplir ) :
```
<h1>Ma grande page</h1>

<p>
    Aller directement à la partie traitant de :<br />
    <a href="#cuisine">La cuisine</a><br />
    <a href="#rollers">Les rollers</a><br />
    <a href="#arc">Le tir à l'arc</a><br />
</p>
<h2 id="cuisine">La cuisine</h2>

<p>... (beaucoup de texte) ...</p>

<h2 id="rollers">Les rollers</h2>

<p>... (beaucoup de texte) ...</p>

<h2 id="arc">Le tir à l'arc</h2>

<p>... (beaucoup de texte) ...</p>
```
S'il ne se passe rien quand vous cliquez sur les liens, c'est qu'il n'y a pas assez de texte. Dans ce cas, vous pouvez soit rajouter du blabla dans la page pour qu'il y ait (encore) plus de texte, soit réduire la taille de la fenêtre de votre navigateur pour faire apparaître les barres de défilement sur le côté.

## Créer un lien vers une autre page de son site avec une ancre

```
<a href="ancres.html#rollers">
```

## Créer un lien avec une info bulle

il suffit de rajouter un attribut title="" dans la balise <a>

```
<p>Bonjour. Souhaitez-vous visiter <a href="https://openclassrooms.com" title="Vous ne le regretterez pas !">OpenClassrooms</a> ?</p>
```


## Un lien qui ouvre une nouvelle fenêtre

Il est possible de « forcer » l'ouverture d'un lien dans une nouvelle fenêtre. Pour cela, on rajoutera

```
target="_blank<a>:
```

exemple :
```
<p>Bonjour. Souhaitez-vous visiter <a href="https://openclassrooms.com" title="Vous ne le regretterez pas !" target="_blank">OpenClassrooms</a> ?</p>
```

## Un lien pour envoyer un email

Si vous voulez que vos visiteurs puissent vous envoyer un e-mail, vous pouvez utiliser des liens de type mailto. Rien ne change au niveau de la balise, vous devez simplement modifier la valeur de l'attribut href comme ceci :

```
<p><a href="mailto:votrenom@bidule.com">Envoyez-moi un e-mail !</a></p>
```

## Un lien pour télécharger un fichier

Beaucoup d'entre vous se demandent comment cela se passe pour le téléchargement d'un fichier… En fait, il faut procéder exactement comme si vous faisiez un lien vers une page web, mais en indiquant cette fois le nom du fichier à télécharger.

Par exemple, supposez que vous vouliez faire téléchargermonfichier.zip. Placez simplement ce fichier dans le même dossier que votre page web (ou dans un sous-dossier) et faites un lien vers ce fichier :
```
<p><a href="monfichier.zip">Télécharger le fichier</a></p>
```



## Les images

Il existe un format adapté à chaque image
Si on résume, voici quel format adopter en fonction de l'image que vous avez :

### Une photo : utilisez un JPEG.

### N'importe quel graphique avec peu de couleurs (moins de 256) : utilisez un PNG 8 bits ou éventuellement un GIF.

### N'importe quel graphique avec beaucoup de couleurs : utilisez un PNG 24 bits.

### Une image animée : utilisez un GIF animé.

## Balise de l'insertion d'une image

```
<img />
```

## La balise doit être accompagnée de deux attributs obligatoires :
```
src="images/fleur.png"
```

```
alt="Une fleur"
```


## Les images doivent se trouver obligatoirement à l'intérieur d'un paragraphe (<p></p>).
Voici un exemple d'insertion d'image :
```
<p>
    Voici une photo que j'ai prise lors de mes dernières vacances à la montagne :<br />
    <img src="images/montagne.jpg" alt="Photo de montagne" />
</p>
```

## Ajouter une infobulle à votre image
L'attribut permettant d'afficher une bulle est  title.

Voici ce que cela peut donner :

```
<p>
    Voici une photo que j'ai prise lors de mes dernières vacances à la montagne :<br />
    <img src="images/montagne.jpg" alt="Photo de montagne" title="C'est beau les Alpes quand même !" />
</p>
```

## Ajouter un lien dans une image

Pour cela, je vais rentrer ma balise <img > à l'intérieur de ma balise <a >, à la place du texte.

Voici le code HTML que je vais utiliser pour cela :

```
<p>
    Vous souhaitez voir l'image dans sa taille d'origine ? Cliquez dessus !<br />
    <a href="img/montagne.jpg"><img src="img/montagne_mini.jpg" alt="Photo de montagne" title="Cliquez pour agrandir" /></a>
</p>
```

## Les figures

Grace à elle, une image peut etre situé en dehors d'un paragraphe (de toute façon on peut utiliser un <div)

```
<figure>
    <img src="images/blocnotes.png" alt="Bloc-Notes" />
</figure>
```

Les figures peuvent être de différents types :

 - images ;
 - codes source ;
 - citations ;
etc.

Pour ajouter une légende, utilisez la balise  <figcaption> à l'intérieur de la balise  <figure>, comme ceci :
```
<figure>
    <img src="images/blocnotes.png" alt="Bloc-Notes" />
    <figcaption>Le logiciel Bloc-Notes</figcaption>
</figure>
```
