1- Historique

En 1991, l'anglais T.B Lee développe le premier "serveur" 
Capable de transmettre une page de texte sur un reseau mondial d'ordinateur 
(le World Wide Web ou "www" ou web).

Pour consulter la page de texte depuis un "client" il faut en pratique 
un logiciel/une application dediée: ( Edge,Safari,Opéra GX,Google...)

Pour écrire la page, il faut un éditeur de texte/codes (Visual Studio Codes, SublimText,)

Lee invente un langage déclaratif capable de produire du texte améliorer qu'il 
appelle HyperText : une partie du texte est cliquable pour accéder à d'autres
pages de texte.

Les fichiers HyperText portent l'extention .HTML (HyperText Markup Language)

2- Généralité sur HTML

HTML n'est pas un langage de programation, C'est un langage de balises qui
décrit ce que l'utilisateur doit voir dans son navigateur.

Une balise s'écrit < nom de la balise >. Il en existe en 2025 des dizaines de balise
https://developer.mozilla.org/en-US/docs/Web/HTML

La plupart des balises sont pairées (en couple) mais il en existe quelquels balises
orphelines.
Ex:
- <body>    </body>
-<br> (à noter que <br/> est autorisé)

HTML est un langage declaratif. Il faut indiquer ce que l'on veut voir, par exemple:
saut de ligne, gras, indentation, lien, HyperText....

Ex: La balise <br> premet de casser les lignes.

Remarque importante, les balises couplées possèdent un ou plusieurs attributs
(toujours dans la balise ouvrante).
Exemple : <a href="une valeur"></a>
mais il esiste aussi des attributs généraux (valables avec toutes les balises : id et class)

3. Un fichier plus complet

En général, la première page d'un site web est nommé index.HTML
=> voir le fichier correspondant 

La balise orpheline <img> permet d'inserer une image sur sa page 
Il faut indiquer la source de l'image avec l'attribut src 

Par defaut le navigateur cherche les fichiers dans le dossier courant qui se note. /

ex : <img src"./image poitou.jpeg">
Le symbole ./ n'est pas obligatoire car la recherche se fait là par defaut. 

1er cas: Si l'image se trouve dans un dossier directement descendant par rapport au dossier courant:
<img src="nomDuDossier/images.jpeg">

2eme cas : Si l'image se trouve dans un dossier que l'on peut atteindre
en remontant l'arborescence : 
<img src="../IMG/images.jpeg">

Un chemin vers un fichier qui commence par ./ ou ../ 
est appelé un chemin relatif.

- La balise couplée  <table>/</table> pour réaliser un tableau. Le tableau se remplit
ligne par ligne puis case par case grâce aux balises <tr></tr> puis <td></td>.
Il est possible de definir une case comme un tête avec la balise <th></th>.

Par defaut, le navigateur n'ajoute aucune bordure aux tableaux.
=> Il faut ajouter du style => langage CSS 
Chapitre : Le language CSS

1. Le CSS donne du style à la place du style par défault

=> Cascading Style Sheet
=> https://developer.mozilla.org/en-US/docs/Web/CSS

=> synthaxe : 
nomElementHTML {
    propriete1 : valeur1;
    propriete2 : valeur2;
    ...
}

Les propriétés sont très nombreuses et il ne faut pas toutes les connaîtres.

Exemple: solid;

Remarques: Certaines propriétés peuvent contenir plusieurs valeur (l'ordre des valeurs peut compter)

2. Oû écrire le CSS ?
1ere méthode: Directement dans le fichier HTML, entre un paire de balises <style></style>
Quelques propriétés à connaître:
-border
-color (couleur du texte)
-background-color-width
-width(largeur d'un élément)
-height(hauteur d'un élément)
-text align
-text-decoration (souligner,surligner,...)
-font-size (taille de la police de caractères)
-font-family
-display ( pour choisir le mode d'affichage)
-padding (marge entre bordure et élément)
-margin (marge externe à la bordure)
-text-align (pour positioner le texte)
-font (pour la police de caractère)

Il est possible d'ajouter des commentaires entre /* ...*/

Remarques : Les couleurs peuvent avoir soit un nom (ex: chartreuse) soit un code 
(ex: rgb(109, 138, 230) ) soit un code héxadécimal (ex: #ECB20A).

Si la hauteur et la largeur sont fixés alors le contenu peut déborder.
Les longueurs peuvent s'exprimer en pourcentage de la page.

-2e méthode : Dans un fichier à part avec l'extention .CSS
Pour faire le line entre le fichier CSS et le fichier HTML, on utilise
(dans HTML) la balise orpheline <link>

3. Les balises HTML universelles
Le style (CSS) s'applique en "cascade", au plus près de l'élément:
*ex: une propriété color pour body et hl s'appliquera différent (pour hl).
‌deuxieme methode:
Dans un fichier à part avec l'extension .css

Pour faire le lien entre le fichier css et le html, on utilise (dans html), la balise orpheline <link>

Problèmes: Parfois nous avons plusieurs éléments identique mais leur appliquer le meme style:
=> on utilise les attributs généraux html class ou identique
=> un élément peut appartenir à plusieurs classes
-avec une classe:
.nomClasse{
    propriété:valeur;
}

-avec un id:
#nomID{
    propriete:valeur;
}

Pour englober (faire un conteneur) plusieurs HTML
on peut utiliser la balise universelle <div></div>
