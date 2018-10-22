#  Syntaxe du Markdown
![Markdown Lover](https://www.bettertechtips.com/wp-content/uploads/2017/07/markdown-linux-640x300.png)

-----------------
>## Headers (titres)
Les titres peuvent être écrit grâce au hashtag (#). Les titres peuvent être organisés par taille, du plus grand au plus petit.  
 - \# Titre de niveau 1
 - \#\# Titre de niveau 2
 - \#\#\# Titre de niveau 3
 - \#\#\#\# Titre de niveau 4
 - \#\#\#\#\# Titre de niveau 5
 - \#\#\#\#\#\# Titre de niveau 6

-----------------

>## Emphases
Les emphases mettent en "page" des morceaux de textes. Il est donc possible de mettre des parcelles de texte en *italique*, en **gras** ou **_les deux_**.
 - \**Italique*\* ou \__Italique_\_
 - \*\***Gras**\*\* ou \_\___Gras__\_\_
 - \*\_\_*__Italique Gras__*\_\_\* ou \*\*\_**_Gras Italique_**\_\*\*

----------------
>## Les Listes

>### Ordonnées
1. Premier élément
2. Second élément
    1. Premier élément imbriqué
    2. Second élément imbriqué
3. Troisème élément
4. Quatrième élément

La syntaxe est simplement **1.** devant chaque ligne, en indentant pour les lignes imbriquées (mais quel langage intelligent  :sunglasses:).

>### Non ordonnées
- Un élément
- Un élément
    - Un élément imbriqué
    - Un élément imbriqué
- Un élément
- un élément

La syntaxe est simplement **-** devant chaque ligne et utiliser l'indentation pour faire les éléments imbriqués.

------------
>## Les tableaux
Pour faire des tableaux, la syntaxe est un peu spécial, voyons d'abord le résultats:

| Titre 1       |  Titre 2        |  Titre 3    | 
| :------------ | :-------------: | ----------: |
| Colonne       |     Colonne     |    Colonne  |
| Alignée à     |   Alignée au    |   Alignée à |
| Gauche        |     Centre      |      Droite |

\| Titre 1       |  Titre 2        |  Titre 3    |  
\| :------------ | :-------------: | ----------: |  
\| Colonne       |     Colonne     |    Colonne  |  
\| Alignée à     |   Alignée au    |   Alignée à |  
\| Gauche        |     Centre      |      Droite |  

Chaque caractère ici à sa place. Les **:** devant ou après chaque ligne signifie la justification du texte, comme c'est indiqué dans le tableau.
Hors de ça, les **|** délimitent les cellules du tableau et les **-----** délimitent les cellules titres.

------------
>## Les liens
Pour donner un exemple de lien, voici le lien vers les consignes de **l'exercice** : 
[Lien vers les consignes](https://github.com/becodeorg/LIE-Hamilton-1.7/blob/master/01-La-prairie/00-terminal-git-markdown/markdown/group-work.md).

Pour faire le lien, je lui ai donné un nom entre **[]** (dans ce cas-ci [Lien vers les consignes]) et ensuite, j'ai mit le lien entre **( )** (dans ce cas-ci \(https://github.com/becodeorg/LIE-Hamilton-1.7/blob/master/01-La-prairie/00-terminal-git-markdown/markdown/group-work.md\)).

On peut le faire de manière directe aussi en mettant simplement le lien en brut comme ceci: https://github.com/becodeorg/LIE-Hamilton-1.7/blob/master/01-La-prairie/00-terminal-git-markdown/markdown/group-work.md.

----------
>## Images et images animées

>### Image
![Image normale](https://static.hitek.fr/img/actualite/2013/07/12/1373633772evolutionofgeek.jpg)

Pour afficher une image, il faut mettre un **!** devant des **[]** (qui contiendront le texte alternatif si l'image ne peut être trouvée) et mettre le lien vers l'image entre **()**.

Dans ce cas, ça donne: \![Image normale]\(https://static.hitek.fr/img/actualite/2013/07/12/1373633772evolutionofgeek.jpg).

>### Image animée (GIF)
![GIF](http://image.noelshack.com/fichiers/2012/10/1331044596-1330976121741.gif)

Exactement pareil que pour l'image non animée.

------------
>## Code
Je vais ici mettre un bout de Javascript, et comme je suis gentil, je vais le commenter (je simulerait l'utilisation de JQuery):
```javascript
$(document).ready(() => {
    $("#unId").on('click', function(event){
        $("#idMenu").toggle();
    });

    const uneFonction = (param) => {
        console.log("J'aime me compliquer la vie!");
    };

    function uneAutreFonction(param){
        console.log("Ici, je me facilite la vie!");
    }
}
```