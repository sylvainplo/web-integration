# Les pseudo-classe CSS

Comme nous l'avons vu dans la section précédente, il existe des pseudo-classe comme :hover.
Cette dernière va permettre de modifier les propriétés d'un élement à son survol.

Il existe aussi des pseudo-classe qui vont permettre d'ajouter un contenu HTML, le plus souvent utile pour l'esthétisme.

## :before & :after
Ces deux pseudo-classe vont créer un pseudo-élement qui sera le premier enfant de l'élement ciblé pour `:before` et le dernier pour `:after`.

Un pseudo-élement existe à partir du moment où il possède la propriété `content` en CSS.

Exemple d'utilisation :

    <p class="class-before">Un texte avec un carré devant</p>
    
    .class-before::before {
        content: '';
        width: 5px;
        height: 5px;
        display: inline-block;
        background: blue;
    }
    
Dans cet exemple, nous allons placer devant le texte un carré bleu.

Ces pseudo-classe vont le plus souvent nous permettre de créer des formes sans pour autant rajouter des élements HTML dans le DOM.

