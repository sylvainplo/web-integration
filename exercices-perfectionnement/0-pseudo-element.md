# Les pseudo-element CSS
En HTML, il existe des pseudo-element qui vont permettre de mettre en forme une certaine partie de l'élement ciblé.

## :before & :after
Ces sélecteurs vont créer un pseudo-element qui sera le premier enfant de l'élement ciblé pour `:before` et le dernier pour `:after`.

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

Ces pseudo-element vont le plus souvent nous permettre de créer des formes sans pour autant rajouter des élements HTML dans le DOM.

