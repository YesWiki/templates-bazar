# Templates-bazar : des templates à utiliser dans bazar

### Installation
A partir de la racine du wiki, copiez les fichiers dans le répertoire `custom/templates/bazar/` (à créer si inexistant)
Attention, certains templates nécessitent l'ajout de dossiers supplémentaires comportant des fichiers (images, bibliothèques javascript, css...)

### Présentation des templates
 - **bingo.twig** : permet de générer un bingo en mode collaboratif pour l'imprimer et jouer avec les participants. Ne nécessite que le champ bf_titre (max 45 caractères). n'est pas intégré au template accessible dans le composant. Il faut donc indiquer soi-même le nom du template dans le bazarliste

 - **glossaire.tpl.html** : présentation sous forme d'annuaire alphabétique de défintions de mots (un glossaire quoi ;-). Quand on survol le mot, sa définition apparaît, on clique sur le mot, on ouvre une page avec sa défintion. Le formulaire idéal se compose des champs suivants (le label permet de cacher le titre afin d'éviter qu'il ne s'affiche deux fois) : 
```
labelhtml*** *** *** <div style="display:none">
texte***bf_titre***Le mot***35***35*** *** *** ***1***0***
labelhtml*** *** *** </div> <!-- ferme le div .hide -->***
textelong***bf_description***Définition***10***2*** *** ***wiki *** *** ***
lien_internet***bf_url***Lien pour en savoir plus***40***255***http://*** *** ***0***0
```

  - **compteurs.tpl.html** : ce template permet d'afficher la somme du champ bf_nombre (si pas dans votre formulaire, utilisez correspondance="bf_nombre=votre champ"). Les champs nécessaires minimaux sont
    - bf_nombre
  - **livredor-droite-gauche.tpl.html** : ce template permet d'afficher un recueil d'infos sous forme de bulles (gauche-droite). Les champs nécessaires minimaux sont
    - bf_titre
    - bf_image
    - bf_description
    - dans files, un fichier nommé user.png
  - **liste_galerie.tpl.html** : ce template permet d'afficher une galerie photo en deux colonnes. Celle de gauche reprend en mini vignettes toutes les photos disponibles et sur celle de droite, une vue agrandie de la photo sélectionnée dans la partie gauche. Les champs nécessaires minimaux sont
    - bf_titre
    - bf_image
    - bf_description

- **mails_maj.tpl.html** : ce template affiche les fiches non mises à jour depuis x jours (180 par défaut, paramètre : nbjour="x") et d'envoyer un mail paramétrable aux contacts des fiches. Les champs nécessaires minimaux sont
    - bf_titre
    - bf_mail
    - paramètre possible : nbjour=" " 

- **post-it.tpl.html** : il montre les données sous forme de post-it (3 couleurs aléatoires). Le contenu affiché dans le post-it est bf_titre et bf_aide (textelong).  Les champs nécessaires minimaux sont
    - bf_titre
    - bf_description

 - **photo-oxygen.tpl.html** : Ce template permet d'afficher une galerie de photos :
     Les champs nécessaires minimaux sont : 
     - bf_image
     - bf_auteur
    

