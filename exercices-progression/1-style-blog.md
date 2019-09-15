# Construire un blog stylé

### Style de base
Maintenant que la structure de notre blog est bien en place, nous pouvons le styliser.

Inspirez vous d'internet pour faire un design sympa :
* [Liste de blog en cas de panne d'inspi](http://www.siteduzero.com)
* [Liste d'autres blog en cas de grosse panne d'inspi](https://www.elegantthemes.com/blog/resources/web-design-blogs-to-follow)

### Style responsive
Après avoir stylisé notre blog nous allons le rendre responsive.
Le but étant que notre blog s'adapte à la fois sur mobile, tablet & desktop.

Pour cela, en CSS, nous allons pouvoir définir des propriétés propres à certaines résolutions d'écran.

Pour ce faire, en bas de votre fichier `style.css` ajoutez : 

    .myClass {
        color: #fff
    }
    
    @media (max-width: 767px) {
        .myClass {
            color: #000
        }
    }
    
Ces propriétés vont appliquer une couleur de texte blanche en desktop et noir pour les devices ayant une taille d'écran inférieure ou égale à 767px donc les mobiles.

Pour déclarer une résolution minimun ou maximum, nous allons utiliser les "media-queries" `@media` suivi de `max-width` ou de `min-width` pour une taille d'écran minimum.

Exemple pour une `max-width`: 
       
    .myClass {
        color: #fff; //couleur blanche par défaut
    }

    @media (max-width: 767px) {
        .myClass {
            color: #000; //couleur noir en mobile
        }
    
        .myClass .myText {
            font-weight: 700; //le texte sera en gras en mobile
        }
    }
    
Exemple pour une `min-width`:

    .myClass {
        color: #fff; //couleur blanche par défaut
    }
    
    @media (min-width: 768px) {
        .myClass {
            color: #000; //couleur noir en tablet et desktop
        }
    
        .myClass .myText {
            font-weight: 700; //le texte sera en tablet et desktop
        }
    }
    
Il est préferable d'utilisé les `media-queries` avec une `min-width`. 
Nous allons définir toutes les propriétés par défaut pour le mobile et, en fonction, ajouter des propriétés les résolutions supérieure.
Nous aurons donc un `(min-width:768px)` pour ce qui va être tablet & desktop et `(min-width: 992px)` pour cibler seulement le desktop.

C'est l'approche "Mobile first".

A savoir que les medias-queries peuvent être multiples tel que :

    .myClass {
        color: #fff
    }
        
    @media (min-width: 768px) and (max-width:991px) {
        .myClass {
            color: #000
        }
    }
    
La couleur noir s'appliquera seulement pour les devices avec une taille comprise entre 768px et 991px soient la plupart des tablets.

Maintenant, il ne nous reste plus qu'à rendre notre blog responsive en y ajoutant les ajustements nécessaires pour mobile. 