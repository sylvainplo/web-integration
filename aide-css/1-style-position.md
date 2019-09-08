# Les positions en CSS

Nous pouvons appliquer des `positions` en CSS à chaque élements HTML.
Pour cela rien de plus simple, il vous suffit de définir la propriétés `position: relative;` par exemple.

Cette propriétés est importantes en CSS et peut vous être assez utiles grâce à ses différentes valeurs.
Elle va pouvoir définir comment un élement doit se placer dans un document grâce à ses valeurs associés : `top`, `left`, `right` et `bottom`

###Position: relative
Cette valeur ne va pas modifier sa disposition dans le document directement mais grâce à elle, on va pouvoir être changer avec les propriétés `left`, `top`, `bottom` et `right`.

###Position: absolute
Cette valeur va retirer l'élements du flux normal et va positionner l'élement par rapport à son parent le plus proche qui possédera une position `relative`.
Sa position sera alors défini grâce aux propriétés de disposition (`left`, `right`,...) qui seront calculées par rapport au parent en position `relative`.

###Position: fixed
Cette valeur va aussi retirer l'élement du flux mais ne va le positionner que par rapport à la fenêtre et non pas par rapport à un parent.
Prenons cet exemple :

    .monFixed {
        position: fixed;
        bottom: 15px;
        right: 15px;
        width: 50px;
        height: 50px;
        background: #000;
    }

L'élement va se positionner à 15px en bas à droite de ma fenêtre et ne va pas bouger quelques soient l'endroit de la page ou je me trouve. Il va ainsi rester "fixé" en bas à droite.

Pour les autres valeurs ou pour plus d'informations, consulter ce [guide](https://developer.mozilla.org/fr/docs/Web/CSS/position)