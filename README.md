# Templates-bazar : des templates à utiliser dans bazar
### Présentation des templates
 - **vignette_description.tpl.html** : présentation sous forme de vignettes d'image, puis de titre, courte description (bf_description) et boutons de visualisation et d'édition
  - **material-card.tpl.html** : présentation sous forme de vignettes graphiques souvent utilisées pour réaliser des annuaires visuels 
    - pour ce template, il est nécessaire d'ajouter un dossier javascripts contenant le fichier lazyload.min.js et un autre dossier nommé styles avec le fichier material-card.css
  - **liste_mails_seuls.tpl.html** : ce template permet de récupérer sour forme de liste les emails d'un formulaire afin de pouvoir facilement les copier-coller dans un webmail
  - **liste_fiches_horscarte.tpl.html** : ce template permet de récupérer sour forme de liste les titres des fiches (avec une carte cartogoogle) pour lesquelles les utilisateurs ont oubliés de cliquer sur le bouton "placer le point sur la carte"
  - **liste_accordeon_triee_date.tpl.html** : ce template permet d'afficher sous forme de liste toutes les fiches contenant une date ultérieure à "aujourd'hui" sous format Le date / titre (pratique pour afficher un calendrier en mode liste avec uniquement les évènements à venir)
  - **liste_act_avenir_details.tpl.html** : ce template permet d'afficher sous forme de liste toutes les fiches contenant une date ultérieure à "aujourd'hui" sous format Le date - heure / titre et à la ligne une courte description de l'activité (bf_chapeau) 
  
  
### Installation
A partir de la racine du wiki, copiez les fichiers dans le répertoire /themes/tools/bazar/ (à créer si inexistant)
Attention, certains templates nécessitent l'ajout de dossiers supplémentaires comportant des fichiers (images, bibliothèques javascript, css...)
