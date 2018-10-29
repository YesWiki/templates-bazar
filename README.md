# Templates-bazar : des templates à utiliser dans bazar

### Installation
A partir de la racine du wiki, copiez les fichiers dans le répertoire /themes/tools/bazar/templates (à créer si inexistant)
Attention, certains templates nécessitent l'ajout de dossiers supplémentaires comportant des fichiers (images, bibliothèques javascript, css...)

### Présentation des templates
 - **vignette_description.tpl.html** : présentation sous forme de vignettes d'image, puis de titre, courte description (bf_description) et boutons de visualisation et d'édition. Les champs nécessaires minimaux sont
    - bf_titre
    - bf_image optionnelle
    - bf_description
  - **material-card.tpl.html** : présentation sous forme de vignettes graphiques souvent utilisées pour réaliser des annuaires visuels 
    - pour ce template, il est nécessaire d'ajouter un dossier javascripts contenant le fichier lazyload.min.js et un autre dossier nommé styles avec le fichier material-card.css. Les champs nécessaires minimaux sont
    - bf_titre
    - bf_image optionnelle
    - bf_baseline
    - bf_description
    - paramètre possible : nbcol="1, 2, 3, 4 ou 6" 
  - **liste_mails_seuls.tpl.html** : ce template permet de récupérer sour forme de liste les emails d'un formulaire afin de pouvoir facilement les copier-coller dans un webmail. Les champs nécessaires minimaux sont
    - bf_titre
    - bf_mail
  - **liste_fiches_horscarte.tpl.html** : ce template permet de récupérer sour forme de liste les titres des fiches (avec une carte cartogoogle) pour lesquelles les utilisateurs ont oubliés de cliquer sur le bouton "placer le point sur la carte". Les champs nécessaires minimaux sont
    - bf_titre
    ainsi que les éléments standard d'adressage
  - **liste_accordeon_triee_date.tpl.html** : ce template permet d'afficher sous forme de liste toutes les fiches contenant une date ultérieure à "aujourd'hui" sous format Le date / titre (pratique pour afficher un calendrier en mode liste avec uniquement les évènements à venir). Les champs nécessaires minimaux sont
    - bf_titre
    - bf_date_debut_evenement
    - bf_date_fin_evenement
  - **liste_act_avenir_details.tpl.html** : ce template permet d'afficher sous forme de liste toutes les fiches contenant une date ultérieure à "aujourd'hui" sous format Le date - heure / titre et à la ligne une courte description de l'activité (bf_chapeau). Les champs nécessaires minimaux sont
    - bf_titre
    - bf_date_debut_evenement
    - bf_date_fin_evenement
    - bf_chapeau
  - **compteurs.tpl.html** : ce template permet d'afficher la somme du champ bf_nombre (si pas dans votre formulaire, utilisez correspondance="bf_nombre=votre champ"). Les champs nécessaires minimaux sont
    - bf_nombre
  - **galerie_photos.tpl.html** : ce template permet d'afficher une galerie de photos "classique" en 6 colonnes avec la photo et le titre par dessous. Les champs nécessaires minimaux sont
    - bf_titre
    - bf_image
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
  - **map-date-futures.tpl.html** : ce template affiche sous forme de carte les fiches événements avec une date future. Les champs nécessaires minimaux sont
    - bf_titre
    - bf_date_debut_evenement
    - bf_date_fin_evenement
    - tous les éléments permettant un adressage
  - **liste_liens_editables.tpl.html** : ce template affiche sous forme de liste cliquable le contenu d'un formulaire. Si on clique, on ouvre un autre onglet avec la fiche en mode édition. Les champs nécessaires minimaux sont
    - bf_titre
  - **semi-ouvert.tpl.html** : ce template affiche sous forme de liste des "blocs" le contenu du formulaire avec une image à gauche et des champs (bf-titre et ... ) à droite + télécharger fichier, lien vers url et bouton en savoir pkus pour ouvrir la fiche complètement (tous les champs de ce template sont cachés si ils ne contiennent pas de données / ou image par défaut). Les champs nécessaires minimaux sont
    - bf_titre
    - bf_image optionnelle
    - bf_date_debut_evenement optionnel
    - bf_description
    - bf_site_internet optionnel
    - champ fichierstage à télécharger optionnel
  - **actu.tpl.html** : il montre les actus comprises entre deux dates de parution (titre + image arrière fond). Lors du survol => description et au clic ouverture de la fiche (en modal ou pas). Les champs nécessaires minimaux sont
    - bf_titre
    - bf_date_debut_evenement
    - bf_description_courte
    - bf_date_debut_publication
    - bf_date_fin_publication
    - paramètre possible : modal="1" nbcol="1, 2, 3, 4 ou 6"
  - **agenda.tpl.html** : il montre les évènements à venir (titre + date + image arrière fond). Lors du survol => description et au clic ouverture de la fiche (en modal ou pas). Les champs nécessaires minimaux sont
    - bf_titre
    - bf_image optionnel
    - bf_date_debut_evenement
    - bf_description_courte
    - paramètre possible : agenda="futur" modal="1" nbcol="1, 2, 3, 4 ou 6"
  - **post-it.tpl.html** : il montre les données sous forme de post-it (3 couleurs aléatoires). Le contenu affiché dans le post-it est bf_titre et bf_aide (textelong).  Les champs nécessaires minimaux sont
    - bf_titre
    - bf_aide
  - **blog.tpl.html** : Ce template permet d'afficher des actualités :
     - dernier aticle mis en avant
     - affiche la date et l'auteur del'article sous le titre
     - le résumé affiché est un champ "bf_chapo" - car on ne voulait pas avoir une description tronquée
     Plus d'infos https://yeswiki.net/?BlogTplHtml
