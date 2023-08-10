# Instructions - ⚒️ Exercice #03 - Typographie

Sephine Bembaka est une romancière qui écrit sur ses voyages depuis près de deux décennies. Avant le lancement de son nouveau roman *Eaux Noires*, qui raconte l'histoire de personnages réels au Maroc, l'auteur souhaite donner un coup de jeune à son site Web professionnel. Vous modifierez la typographie sur son site, en changeant la taille, le style et les familles de polices, pour rendre la page plus facile à lire.

En utilisant votre compréhension de la typographie, aidez Sephine à améliorer la lisibilité de son site pour ses lecteurs.
## Tâches
1. La section d'en-tête du site de Sephine contient le nom de l'auteur, ainsi que le texte "Voyages", "Fiction" et "Contact".
<br>Modifiez l'épaisseur de la police de l'en-tête afin que le texte apparaisse en **gras**.
2. En descendant la page, la section `banner` contient une superbe image, deux blocs de texte, une balise `h2` avec le texte "DÉC 2023" et une balise `h1` avec le texte "Maroc".
<br>Donnez à la balise `h2` une épaisseur de police de 500 et à la balise `h1` une épaisseur de police de 900.
3. Après avoir examiné le projet, l'auteur suggère que la hauteur de la ligne semble un peu décalée et doit être modifiée tout au long de la page.
<br>Travaillez vers le bas de la page et donnez à l'attribut `line-height` des éléments suivants comme recommandé :
    * Le paragraphe dans la section du journal doit avoir une hauteur de ligne de 1,4 fois la taille de la police.
    * La première lettre de la section journal doit avoir une hauteur de ligne de 0,87 fois la taille de la police.
    * La citation doit avoir une hauteur de ligne de 1,2 fois la taille de la police.
    * Le contenu du pied de page doit avoir une hauteur de ligne égale à 1,5 fois la taille de la police.
4. Le site utilise actuellement des polices `serif` et `sans-serif` communes trouvées sur les ordinateurs des utilisateurs. Depuis que l'auteur a publié le site pour la première fois, un certain nombre de nouvelles bibliothèques de polices ont créé des polices qui, selon vous, conviendraient mieux au site.
<br>À l'aide de l'API Google Fonts, ajoutez les polices suivantes au fichier `index.html` :
    * **Abril Fatface**
    * **Work sans** en poids de police 400, 500 et 800.
    * **Merriweather** en font-weight 400 et 400 *italique*

    <br>Vous pouvez soit lier ces polices dans une seule balise `<link>`, soit trois balises distinctes.

5. Vous pouvez maintenant utiliser les polices nouvellement ajoutées de [Google Fonts](https://fonts.google.com/) dans notre projet. En descendant à nouveau sur la page, définissez la `font-family` et la propriété comme recommandé :
    * Définissez la police de caractères de la balise `h2` dans la section `banner` sur **"Work Sans"**
    * Définissez la police de caractères de la balise `h1` dans la section `banner` sur **"Abril Fatface"**
    * Définissez la police de la section du journal sur **Work Sans**
    * Définissez la police de caractères de la légende de la photo sur **Merriweather**
6. La page a fière allure, mais vous devez également tenir compte des utilisateurs qui ne peuvent peut-être pas accéder aux polices Google. Trouvez-leur plusieurs polices de secours à utiliser au cas où l'accès aux polices d'un tiers leur serait interdit :
Définissez les polices de secours comme suit :
    * balise `h2` dans la section banner : "**Arial**" et **sans-serif**
    * balise `h1` dans la section banner : **sans-serif**
    * La section journal : **serif**
    * La légende de la photo : **serif**
7. Au lieu de lier la police depuis `index.html`, vous réalisez qu'il serait préférable d'importer les polices Google dans les fichiers directement dans les feuilles de style avec la propriété `@font-face`.	
<br>Utilisez la propriété `@font-face` pour importer les polices directement dans les feuilles de style et supprimez les balises `<link>` qui font référence aux polices Google de la page `index.html`.
8. En regardant la page, l'auteur suggère que la page serait vraiment plus belle si nous utilisions une police spécifique, **CroissantOne-Regular.ttf**, dans le pied de page. Les fichiers ont été téléchargés et ajoutés à notre projet dans le répertoire des polices du répertoire `styles/` où nos fichiers CSS sont stockés.
<br>Pour terminer la tâche, vous devez utiliser la propriété `@font-face` pour rendre ces polices accessibles dans les feuilles de style. Nommez la police "Croissant One".
10. Maintenant que vous avez une règle `@font-face`, définissez la propriété `font-family` du pied de page sur "Croissant One" avec "Merriweather" et serif comme polices de secours.