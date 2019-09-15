# La page HTML

### Création d'une page simple
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

Dans cet extrait, on constate la présence de balises HTML avec :
* La balise `<html></html>` va représenter la racine du document. Tous les élements constituant notre page vont se trouver dans cette balise.
* La balise `<head></head>` qui contient la "tête" du document. Ses élements ne seront pas affichés par le navigateur mais pourront lui donner des informations sur certaines données utiles à l'affichage et à l'ergonomie.
* La balise `<body></body>` qui contient le "corp" du "document. C'est dans cette balise que l'on va placer le contenu visible du document.

En HTML, les élements sont représentés par des balises. 
Selon la nature de notre élement, on va utiliser différentes balises comme par exemple la balise `<p></p>` pour tout ce qui va être texte.
Pour la plupart des balises, nous allons retrouver la syntaxe suivante :

    <p>Exemple de texte</p>

Dans cet exemple, nous trouvons une balise ouvrante `<p>` et une fermante `</p>` avec du contenu de type texte au milieu.
Certaines sont cependant appelées "auto-fermante" notament quand elles ne contiennent pas de texte.
Exemple pour une image : 

    <img src="mon-image.png" alt="Texte de substitution">

Chaque balise possède un sens et peut ou non avoir des attributs.
Il existe un grand nombre de balises mais les plus courantes sont :
* `<p> Mon texte </p>` Pour du texte
* `<h1> Mon titre </h1>` Descends jusqu'à `<h6></h6>` pour les titres de différents niveaux
* `<a href="maPage.html"> Mon lien </a>` pour un lien vers ma page html
* `<div></div>` & `<span></span>` pour aider à styliser la page à travers ces deux balises sans significations particulières
* `<img src="monimage.png" alt="texte de remplacement">` Pour une image
* Une succession de `<li></li>` dans une balise `<ol></ol>` pour une liste numérotée ou `<ul></ul>` pour une liste à puces.

Essayez maintenant d'ajouter chacune de ces balises dans votre page HTML.