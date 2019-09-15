# Les animation CSS

En CSS, il est possible de créer différentes animations que ce soit au survol d'un élement, au focus, ou même au chargement d'un élement.

Pour cela, il existe différent propriété CSS :

## La pseudo-classe :hover
Cette pseudo-classe va permettre de modifier l'apparence d'un élement HTML au moment où l'utilisateur va le survoler avec sa souris.

Exemple pour un bouton:
Créer un élement `<button></button>` avec la class `.btn`.
Après avoir créé ce bouton, allons le cibler dans notre fichier CSS. en ajoutant ces propriétés :
        
    .btn {
        padding: 6px 12px;
        background-color: #0000ff;
        color: #fff;
        border: 0;
    }
    
Une fois son style par défaut appliqué, nous allons pouvoir créer un changement de couleur au survol :

    .btn:hover {
        background-color: #fff;
        color: #0000ff
    }
    
En ajoutant la pseudo-classe à la suite de la class `.btn`, on va cibler le bouton seulement au hover (survol de la souris).

Le background et la couleur de texte vont s'échanger au survol et se remettre à la valeur par défaut une fois la souris sortie de l'élement.
Ce changement va cependant se faire de manière assez brutale. Pour ajouter une transition, il suffit de rajouter la propriété CSS `transition` comme ceci :

    .btn {
        padding: 6px 12px;
        background-color: #0000ff;
        color: #fff;
        border: 0;
        
        transition: background-color 1s linear, color 1s linear;
    }
    
Grâce à cette propriété, la transition va se faire sur la propriété `background-color` et `color` et va durer 1s et se faire de façon linéaire.

Cette animation va se faire au survol d'un élement. Maintent, nous allons voir comment créer une animation en continu au chargement de la page.
Imaginons une image tel que :

    <img src="https://cdn.icon-icons.com/icons2/37/PNG/512/wheel_theapplication_2969.png" alt="une roue" class="class-animation"

Puis ajoutons ce style

    .class-animation {
        width: 200px;
        animation: turn 3s linear infinite;
    }
    
    @keyframes turn {
        0% {
            transform: rotate(0);
        }
    
        100% {
            transform: rotate(360deg);
        }
    }
    
Dans cet extrait de code CSS, on constate la présence de `@keyframes`. Cette règle va nous permettre de définir les propriétés relatives à une animation.
Exemple ici avec une rotation de l'image allant de 0 degré à 360. Ce changement se fait de manière progressive tout au long de l'animation. 

Pour relier la `@keyframes` à la classe voulue, il nous suffit de définir la propriété animation en indiquant le nom de la `@keyframes`, sa durée, son timing(de façon linéaire par exemple) ainsi que son nombre d'itération. 

Pour plus d'info, vous pouvez consulter [ce guide](https://developer.mozilla.org/fr/docs/Web/CSS/animation)

Maintenant il ne vous reste plus qu'à animer votre blog.
