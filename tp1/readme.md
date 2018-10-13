<p align="center">
  <a href="https://galilee.univ-paris13.fr/master/master-ingenierie-innovation-images-reseaux-m3ir/">
     <img src="https://github.com/bilelz/tpaw/blob/master/galilee.png?raw=true" alt="Logo Master" width=100/>
  </a>  
  <br/>
 Master² 3IR | <a href="https://3ir2019.slack.com/messages/aw">3ir2019.slack.com</a>


<p align="center">
<kbd><img src="img/index.png" width="300"></kbd><br/>
<h3 align="center">TP1 : CV<br/>
</p>

</h3>
Référence technique [w3schools.com](https://www.w3schools.com/) 

</p>



<!-- TOC -->

- [1. Prérequis](#1-prérequis)
- [2. Plate-forme de developpement :](#2-plate-forme-de-developpement-)
- [3. HTML (index.html)](#3-html-indexhtml)
- [4. CSS](#4-css)

<!-- /TOC -->

# 1. Prérequis

* Lire **tout** l'énnoncé avant de commencer le TP.

❓❓Si vous avez des questions ou des erreurs dans votre code : 
* formater (indenter) bien votre code (raccourci Visual Studio Code : Ctrl + K puis Ctrl + F)
* demander à Google 🔍
* demander à vos camarades 👩‍🎓👨‍🎓
* demander au professeur 🙋




# 2. Plate-forme de developpement : 

> Node.js nous permet d'utiliser le langage JavaScript sur le serveur... Il nous permet donc de faire du JavaScript en dehors du navigateur !

Éditeur de texte (Visual studio code, notepad++,  emacs, …)
Navigateur web (Google Chrome, Mozilla Firefox)

* Éditeur de texte
    * Visual studio code (recommandé)
    * Atom (installé sur les ordinateus de l'université)
    * notepad++

* Workspace
    * Votre code source devrait etre écrit dans ce répertoire TP1
    * * index.html

* Affichage de la page web
* * Ouvrir le fichier index.html avec un navigateur web (Chrome ou Firefox)


# 3. HTML (index.html)
* Écrire la structure de base d’un document HTML 

```html
<html>
    <head>...</head>
    <body> ...</body>
</html>
```

* Chaque catégorie du CV sera écrite via la balise H1

* Le détail de chaque catégorie sera écrite dans un tableau TABLE
   * pour avoir un tableau qui s’affiche sur toute la largeur de la page
    ```html
    <table width="100%" border="1">  ... </table>
    ```
* Mettre un lien vers le site internet de chacune de vos formations ou expériences professionnels.

# 4. CSS

* Créer un fichier cv.css dans le dossier "TP1"
* Entre les balises HEAD du  document cv.html ajouter une référence au fichier CSS 
  
```html
<link rel="stylesheet" href="cv.css" />
```

* Écrivez vos règles CSS pour customiser le design de votre CV.
    * Exemple simple : 
        *    ```<body>``` avec un background-color gris 
        *    les tableaux ```<table>``` avec un background-color blanc
        * les liens ```<a>``` avec une couleur de texte orange au survol de la souris (:hover)
        * illustration : exemple de CV avec la feuille de style cv.css	 
        * Au survol de la souris, changer la couleur de fond de chaque ligne du tableau
        * Au survol de la souris, agrandir les images présentés
           * 1er technique : en changeant la taille de l’image (width)
           * 2eme technique : en utilisant une transformation CSS  https://www.w3schools.com/cssref/css3_pr_transform.asp
           ```css
           transform : scale(2);
           ```
    * Utilisation des mediaquery
        * Les mediaquery permettent d’appliquer du CSS seulement quand l’écran de l’utilisateur a une certaine largeur ou hauteur.
        * Ecrire des règles qui :
            * change la couleur de fond, quand l’écran à une taille max de 300px, max 600px, max 900px et plus de 900px
            ```css
            @media only screen and (max-width: 600px) {
                body {
                    background-color: lightblue;
                }
            }
            ```
        * adapte la taille du tableau pour qu’il soit toujours visible sur toute sa largeur

  
<div align="center">
 --- FIN ---
 </div>
