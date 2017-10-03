# Templates-bazar : des templates à utiliser dans bazar
### Présentation des templates
 - **vignette_description.tpl.html** : présentation sous forme de vignettes d'image, puis de titre, courte description (bf_description) et boutons de visualisation et d'édition
  - **material-card.tpl.html** : présentation sous forme de vignettes graphiques souvent utilisées pour réaliser des annuaires visuels 
    - pour ce template, il est nécessaire d'ajouter un dossier javascripts contenant le fichier lazyload.min.js et un autre dossier nommé styles avec le fichier material-card.css
  - **liste_mails_seuls.tpl.html** : ce template permet de récupérer sour forme de liste les emails d'un formulaire afin de pouvoir facilement les copier-coller dans un webmail
  - **liste_fiches_horscarte.tpl.html** : ce template permet de récupérer sour forme de liste les titres des fiches (avec une carte cartogoogle) pour lesquelles les utilisateurs ont oubliés de cliquer sur le bouton "placer le point sur la carte"
  - **liste_accordeon_triee_date.tpl.html** : ce template permet d'afficher sous forme de liste toutes les fiches contenant une date ultérieure à "aujourd'hui" sous format Le date / titre (pratique pour afficher un calendrier en mode liste avec uniquement les évènements à venir)
  - **liste_act_avenir_details.tpl.html** : ce template permet d'afficher sous forme de liste toutes les fiches contenant une date ultérieure à "aujourd'hui" sous format Le date - heure / titre et à la ligne une courte description de l'activité (bf_chapeau) 
  - **compteurs.tpl.html** : ce template permet d'afficher la somme du champ bf_nombre (si pas dans votre formulaire, utilisez correspondance="bf_nombre=votre champ")
  - **galerie_photos.tpl.html** : ce template permet d'afficher une galerie de photos "classique" en 6 colonnes avec la photo et le titre par dessous. 
  - **livredor-droite-gauche.tpl.html** : ce template permet d'afficher un recueil d'infos sous forme de bulles (gauche-droite).
  - **liste_galerie.tpl.html** : ce template permet d'afficher une galerie photo en deux colonnes. Celle de gauche reprend en mini vignettes toutes les photos disponibles et sur celle de droite, une vue agrandie de la photo sélectionnée dans la partie gauche.
  - **mails_maj.tpl.html** : ce template affiche les fiches non mises à jour depuis x jours (180 par défaut, paramètre : nbjour="x") et d'envoyer un mail paramétrable aux contacts des fiches.
  - **map-date-futures.tpl.html** : ce template affiche sous forme de carte les fiches événements avec une date future.
  
### Installation
A partir de la racine du wiki, copiez les fichiers dans le répertoire /themes/tools/bazar/ (à créer si inexistant)
Attention, certains templates nécessitent l'ajout de dossiers supplémentaires comportant des fichiers (images, bibliothèques javascript, css...)
