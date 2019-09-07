# La feuille de style

###Création de propriétés simples
Après avoir créé une page HTML et ajouté un peu de contenu, nous allons pouvoir styliser la page.
Pour cela, créez le fichier `style.css` dans un dossier `/css`. 
Dans ce fichier `style.css` vous pouvez initialiser les premières propriétés de style de votre page.

Nous allons pouvoir enlevez les `padding` & `margin` par défaut de chaque élement et définir les valeurs de la police et de la font de notre page.

    * {
        margin: 0;
        padding: 0;
    }
    
    body {
        font-family: Arial sans-serif;
        font-size: 14px;
    }

Ensuite, il vous faut charger votre fichier de style dans votre fichier HTML.
Pour cela dans la balise `<head></head>`, insérez :

    <link href="css/style.css" type="text/css" rel="stylesheet">
    
Vos propriétés CSS seront maintenant liées à vos élements HTML.

Retournez maintenant dans votre fichier `index.html` et ajoutez un attribut `class` aux balises que nous venons d'ajouter.

Une balise de texte `<p>` ressemblera ainsi à ça :

    <p class="text">Dis moi pas que c'est pas vrai !</p>
    
Après ça, dans notre fichier `style.css`, ajoutez le code suivant :

    .text {
        color: #00ff00;
        text-transform: uppercase;
    }

Il ne reste plus qu'a actualiser le navigateur pour voir apparaitre les modifications.

Les premières constatations sont :
* On cible une balise HTML par son nom comme nous l'avons fait pour le `<body>`
* On cible un class HTML en précedant le nom de celle-ci par un point : `.text`

Pour styliser vos élements, de très nombreuses propriétés existent, elles rentreront dans votre tête à force de les utiliser mais en attendant, Google est votre ami.

Vous êtes maintenant en capacité de styliser votre page en HTML en ajoutant des `class` et du style à celle-ci.

###Les propriétés en cascade
CSS signifie "Cascade StyleSheet" soit en français: "Feuille de Style en Cascade".
Prenons l'exemple du code suivant : 

    <div class="content">
        <p class="text">Plutot PES ou FIFA ?</p>
    </div>
    <p class="text">Plutot BattleField ou Call of Duty ?</p>
    
Nous allons pouvoir cibler la class `.text`  de manières indépendantes même si elle se trouvent à 2 endroits.

Si nous écrivons dans notre fichier CSS cela :

    .text {
        color: #ff0000;
    }
    
Les deux balises de class `.text` auront un texte rouge.
Maintenant, écrivons cette extrait en dessous de la propriété précédente :

    .content .text {
        color: #0000ff
    }

Nous constatons que la balise dans la class `.content` est maintenant bleu et que le texte à l'extérieur est rouge.

Logique puisque nous avons ciblé la class `.text` se trouvant dans la balise de class `.content`. C'est ce processus qu'on appelle cascade.
Les cascades allant toujours d'un point haut à un point bas, nous écrivons de la balise qui englobe à celle qui est englobée (de la plus "haute" à la plus "basse").



