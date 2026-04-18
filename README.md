# DevStart Agency — Analyse de Code
# Bloc 2 · Module 1 · Académie de Programmation


# Contexte du projet

Dans le cadre du   Bloc 2 — Génie Logiciel   de l'Académie de Programmation IFRI, notre groupe a analysé le code source de la page d'accueil d'une startup fictive,   DevStart Agency  .

Un stagiaire a développé cette page avant de partir, sans laisser de documentation. Notre mission :   analyser, comprendre et documenter ce code   sans le modifier.


# Notre groupe

 N'DA Prielle Arifath
 GBESSEMEHLAN Senami Leoncelle
 KPATINVOH Charis
 SOSSOU Merveilles de Dieu 
 AKPANON Ange-Miguel 

# Structure du dépôt

devstart-analyse/

 original/
        index.html         :Code HTML original (non modifié)
        style.css          :CSS original (non modifié)
  
   annotated/
        index.html         :HTML avec nos commentaires d'analyse
        style.css          :CSS avec nos commentaires d'analyse
  
   rapport_analyse_devstart.pdf   :Rapport d'analyse complet (7 pages)
  
   README.md              :Ce fichier


# Livrables

| Livrable       | Statut   | Fichier                          |
|  Rapport PDF   | Produit  |   rapport_analyse_devstart.pdf   |
|  Code original |  Archivé |   original/                      |
|  Code annoté   | Commenté |   annotated/                     |
|  Présentation  | Jour 5   | Slides à préparer                |

# Résumé de notre analyse

Le code analysé constitue une page d'accueil complète pour une agence web. 
Elle comporte 7 sections (navigation, héro, services, à propos, témoignages, contact, footer), développées en HTML et CSS pur avec Flexbox.

# Ce qui est bien fait 
- Palette de couleurs cohérente et visuellement professionnelle
- Structure de page logique et facile à suivre visuellement
- Bon usage de Flexbox pour la mise en page multi-colonnes

# Problèmes identifiés 

Critiques (bloquants) :
- Formulaire de contact non fonctionnel (absence de balise   <form>  )
- Email dans le footer obfusqué par Cloudflare (code copié depuis un site en ligne)

Majeurs :
- Nommage de classes CSS illisible (  .b1  ,   .c  ,   .d  ,   .e  ... au lieu de   .navbar  ,   .hero  ,   .services  ...)
- Duplication massive dans le CSS : ~80 lignes répétées inutilement
- Pas de balises   <meta charset>   ni   <meta viewport> 
- Aucune media query → site non responsive sur mobile
- Images sans attribut   alt 

Mineurs :
- Liens de navigation tous non fonctionnels (tous   href="#"  )
- Titre de page :   <title>site</title>   au lieu d'un titre descriptif
- Pas de balises sémantiques HTML5 (  <nav>  ,   <main>  ,   <section>  ,   <footer>  )

# Notre démarche

1. Jour 1 — Prise en main du code, ouverture dans le navigateur, initialisation du dépôt GitHub
2. Jour 2 — Lecture ligne par ligne, écriture des annotations (fichiers   /annotated  )
3. Jour 3 — Analyse critique : liste des problèmes, argumentation, propositions
4. Jour 4 — Rédaction du rapport PDF + préparation des slides
5. Jour 5 — Répétition + présentation devant l'académie

# Règle respectée
Nous n'avons pas modifié le code original.
Les fichiers dans   /original   sont identiques à ce qui nous a été fourni. 
Seul le dossier   /annotated   contient nos ajouts (commentaires uniquement).
