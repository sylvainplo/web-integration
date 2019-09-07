# La page HTML

###Création d'une page simple
Pour débuter nous allons créer notre page HTML5.
Pour cela, créez un nouveau document `index.html` et insérez-y ce code :

    <!doctype html>
    <html lang="fr">
    <head>
        <meta charset="utf-8">
        <title>Ma page html</title>
    </head>
    <body>
        <!--Mon contenu web-->
    </body>
    </html>

Ajoutez-y par exemple des titres de différents niveaux avec les balises `<h1>`, `<h2>`,...
Du texte avec la balise `<p>` ou des images avec la balise `<img/>`.

Pour la plupart des balises, nous allons retrouver la syntaxe suivante :

    <p>Cours Astérixsme</p>

Avec une balise ouvrante `<p>` et une fermante `</p>`.
Certaines sont cependant appelées "auto-fermante" notament quand elles ne contiennent pas de textes.
Exemple pour une image : 

    <img src="Bogdanov.png" alt="Un Bogdanov avant sa chirurgie">

Chaque balise possède un sens et peut ou non avoir des attributs.
Ils existent un grand nombre de balises mais les plus courantes sont :
* `<p> mon texte </p>` Pour du texte
* `<h1> mon titre </h1>` Descends jusqu'à `<h6></h6>` pour les titres de différents niveaux
* `<a href="maPage.html"> mon lien </a>` pour un lien vers ma page html
* `<div></div>` & `<span></span>` pour aider à styliser la page à travers ces deux balises sans significations particulières
* `<img src="monimage.png" alt="texte de remplacement">` Pour une image
* Une succession de `<li></li>` dans une balise `<ol></ol>` pour une liste numérotée ou `<ul></ul>` pour une liste à puces.

Essayez maintenant d'ajouter chacune de ces balises dans votre page HTML.