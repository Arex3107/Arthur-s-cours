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
