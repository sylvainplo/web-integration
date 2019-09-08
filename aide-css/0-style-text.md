# Les styles de texte

Pour gérer la mise en forme du texte, il existe de nombreuses propriétés. Les plus utilisées restent :
* `font-size`
* `font-family`
* `font-weight`
* `text-transform`
* `text-decoration`

###Font-size :
La propriété `font-size` va vous permettre de gérer la taille du texte. Elle s'exprime principalement en pixel ou en em.
* Les pixels vont définir une valeur fixe
* Les ems vont définir une valeur relative à la `font-size` du parent : si le parent à une taille de `14px` et que l'on défini la taille de son enfant à `1.1em`, sa font-size sera le résultat de `14px * 1.1`

Pour plus d'informations, consulter ce [guide](https://developer.mozilla.org/fr/docs/Web/CSS/font-size)

###Font-family :
La propriété `font-family` va vous permettre de gérer grâce à une liste ordonné par prioriété les polices à utiliser pour la mise en forme du site :

    font-family: Arial, Helvetica, sans-serif;
    
###Font-weight :
La propriété `font-weight` va vous permettre de gérer la graisse de la police.
On peut définir avec les valeurs principales `normal` ou `bold` ou des valeurs numérique :` 100, 200, 300, 400, 500, 600, 700, 800, 900, 1000`.
Pour les valeurs numériques, tout dépend de la police de votre site mais certaines valeurs ne seront peut-être pas disponibles.
A savoir que `400` correspond à la graisse `normal`, `700` à la graisse `bold`. En dessous de `400`, ce sera des graisses plus fines.
Pour plus d'informations, consulter ce [guide](https://developer.mozilla.org/fr/docs/Web/CSS/font-weight)

###Text-transform :
La propriétés `text-transform` va vous permettre de gérer l'utilisation des lettres capitales pour un texte.
On va pouvoir ainsi mettre un texte en capitale `uppercase`, seulement sa première lettre `capitalize` ou forcer le texte en miniscule `lowercase`

###Text-decoration :
La propriétés `text-decoration` va vous permettre de décorer le texte comme son nom l'indique.
On va pouvoir ajouter un soulignement `underline`, un soulignement par point `underline dotted` ou différents styles à retrouver [ici](https://developer.mozilla.org/fr/docs/Web/CSS/text-decoration)

