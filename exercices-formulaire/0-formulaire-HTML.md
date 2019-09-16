# Les formulaires

Après avec styliser notre blog et l'avoir rendu assez sympa, nous allons pouvoir ajouter un bandeau d'inscription à la newsletter.

Dans ce bandeau, nous allons devoir récuperer l'email de l'utilisateur grâçe à un formulaire HTML.

Pour ce faire, ajoutons ce code HTML :

    <form action="index.html" method="POST">
        <label for="email-input">Email *</label>
        <input type="email" name="email" id="email-input">
    </form>
    
Dans cet extrait, nous venons d'ajouter, un formulaire <form> avec un champ pour renseigner son email `<input>`.
Ce champ possède un type (text, email, number,...) et un name pour récupérer la valeur à la soumission du formulaire.

On peut lier à ce champ un label `<label>` qui servira de légende au champ. On lie un `label` et un `input` ensemble en ajoutant l'attribut for au `label` (il aura alors pour valeur l'id de l'`input`) ou en insérant directement le input dans le `label`

Après avoir ajouter le champ utile pour l'email, on va pouvoir ajouter un bouton pour soumettre le  formulaire. 
La encore, on va utiliser la balise `<input>` mais en lui attribuant cette fois un type `submit`.
Dans cet input, nous allons aussi ajouter un attribuant `value` qui va contenir le texte du bouton de validation.
Ajoutons donc notre input de validation à la fin de notre formulaire :
        
    <input type="submit" value="M'inscrire">

Et voila, nous venons de créer un formulaire d'inscription à la newsletter. 
Il ne nous reste plus qu'à le styliser an ajoutant des classes.

