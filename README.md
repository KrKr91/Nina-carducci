# Portfolio Nina Carducci - Optimisation SEO & Accessibilité

Ce projet consiste en l'optimisation technique du site vitrine de Nina Carducci, une photographe professionnelle basée à Bordeaux. Le site initial présentait des problèmes de lenteur, d'accessibilité et de référencement, ainsi que quelques bugs d'interface.

L'objectif de ce projet a été de fournir un code propre, performant et optimisé pour les moteurs de recherche et les utilisateurs.

## Performances (WebPerf)
Le temps de chargement a été drastiquement réduit (Score Lighthouse passé à **98-100/100**) grâce aux actions suivantes :
- **Optimisation des images :** Redimensionnement et conversion de toutes les images du format JPEG/PNG vers le format moderne **WebP**.
- **Chemin critique de rendu :** Déplacement des balises `<script>` en bas de la balise `<body>` pour débloquer l'affichage immédiat du HTML et du CSS.
- **Minification :** Utilisation de fichiers CSS et JS minifiés pour réduire le poids des requêtes.

## SEO (Référencement Naturel & Local)
Le code a été enrichi pour améliorer la compréhension du site par Google :
- **Sémantique HTML :** Correction de la hiérarchie des titres (un seul `<h1>` sur la page).
- **SEO Local (JSON-LD) :** Intégration de données structurées `Schema.org` (type `LocalBusiness`) incluant l'adresse à Bordeaux, les horaires et la zone d'intervention (Paris/Bordeaux) pour favoriser l'apparition dans le *Local Pack* de Google.
- **Social Media (SMO) :** Ajout des balises Meta `Open Graph` (Facebook, LinkedIn) et `Twitter Cards` pour générer des aperçus propres lors du partage du lien.

## Accessibilité 
Le site a été audité avec l'outil **WAVE** et mis en conformité avec les normes d'accessibilité :
- **Contrastes :** Modification du code CSS pour assurer un ratio de contraste lisible sur les boutons de navigation de la galerie.
- **Lecteurs d'écran :** Ajout d'attributs `alt` pertinents sur l'ensemble des images et liaison sémantique des balises `<label>` et `<input>` du formulaire de contact.
- **Composants personnalisés :** Remplacement des icônes du carrousel Bootstrap (images de fond) par des entités textuelles HTML (`&#10094;`, `&#10095;`) avec un fond contrasté pour garantir leur visibilité.

## Débogage JavaScript & UI
Réparation du fichier `maugallery.js` et de la mise en page :
- **Filtres de la galerie :** Correction de la logique d'attribution de la classe `.active` lors du clic sur les catégories.
- **Lightbox (Modale) :** Correction de l'algorithme de calcul de l'index des images, permettant une navigation infinie et sans erreur via les flèches "Suivant" et "Précédent".
- **Responsive Design :** Application de la propriété `object-fit: cover` sur les images du slider mobile pour empêcher leur déformation.

## Stack Technique
- HTML5 / CSS3
- JavaScript (jQuery)
- Bootstrap 5
- Outils : Lighthouse, WAVE, Google Rich Results Test

## Installation et exécution en local
 Clonez ce dépôt GitHub :
   ```bash
   git clone [Lien de ton repo GitHub]

    Ouvrez le dossier du projet dans votre éditeur de code (ex: VS Code).

    Lancez le fichier index.html dans votre navigateur (ou utilisez l'extension Live Server).
