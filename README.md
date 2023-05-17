# KT-IT-Responsible
Knowledge Transfer Poste IT CECI-BEST

# Pourquoi Latex ?
Il est vrai que Latex est pas la premiere choses que on pense pour faire un KT mais Latex apporte beaucoup d'avantes que Google docs n'ont pas.

1) C'est tres pro, respecte un format défini, facile a changer sans casser la structure.
2) Pas n'importe qui peut venir dessus et faire n'importe quoi ou supprimer des parties sans nous en rendre comptes
3) Associer avec Github impossible de se tromper, on peut revenir en arriere, voir qui a fait les modification
2) On est a l'EPL quand meme

# Comment télécharger le KT pour le modifier 
2 possibilités :
premiere pour les gens a laise avec Git
l'autre pour des gens pas trop a laise

## Git clone

Il suffit de cloner le repos Github sur votre ordinateur, pour se faire 2 possibilités :
Et une 3eme pour ceux qui sont pas dutout a laise avec Github

### avec un lien HTTP :

Vous ouvrez un terminal dans le dossier que vous voulez installer le KT (il faut avoir Git d'installer sur votre ordi) 
Ensuite vous Cloner le repo Github avec cette commande
    
```bash
git clone <Lien-de-clone-HTTP>
```

Le lien peut etre optenu sur la page de repo Github ![](https://github.com/CECI-BEST-LLN/KT-IT-Responsible/blob/main/img/GitClone.png?raw=true)

un fois la commande lancer dans votre terminal vous devriez avoir vos fichiers.

Attention une fois le clone effectuer, il n'est plus necessaire d'en refaire un pour faire d'autre modification dans le future. Si vous avez toujours les fichiers clone sur votre ordinateur il vous suffit de mettre a jour vos fichier au cas ou il y a eu des modifications autre que les votre. Pour ce faire il suffit dans lancer la commande : 

    git pull

Avec cette commande vous aurrer la dernier version des fichier qui sont présent sur le github.

### avec un lien SSH

c'est pour les KOG de l'info ça, je ne vais pas expliquer comment avoir une cles SSH mais sachez que si vous ne savez pas de quoi je parle laisson tomber cette méthode ou alors aller voir sur Google comment cloner un repo git avec une clef SSH

Pour ceux qui utilise cette methode c'est la meme chose que HTTP mais il faut mettre le lien du SSH a la place 

```bash
git clone <Lien-de-clone-SSH>
```

### Télécharger en ZIP

Il est possible de télécharger les fichier du Latex dans une archive ZIP, il suffit de cliquer sur *Download ZIP* dans le bouton *<>Code* comme montrer sur l'image au desssu.

Vous n'avez plus cas extraire vos fichier de l'archive et voila mais nous verrons plus tard que cela ne sera pas la methode la plus facile pour mettre a jour le KT

# modification

Ici c'est un peu comme vous le sentez pour modifier le KT (surtous mes fautes d'orthographes). Il existe plusieur outils pour faire du Latex tel que TexMaker, Visual Studio code possède des plugins pour faire du Latex. 

Le plus facile reste cependant [Overleaf](https://www.overleaf.com) en ligne qui est asser facile a prend en main et donc parfait pour les nouveaux.

# Mettre la nouvelle version sur le Github

La aussi plusieur possibilités en fonction de ce que vous avez fait précédemment

## Vous avez fait un Git clone

Si vous avez fait un git clone et donc que vos fichier sont dans votre PC, il suffit de remplacer ou de modifier ce que vous avez télécharger par le git clone par la nouvelle version du KT

ouvrez un terminal dans le dossiers qui contient le KT et il suffi maintenant d'ajoute vos nouveaux fichier avec la commande

    git add -A

une fois cela fait, il faut "commit" vos modification, pour cela, il suffit de faire :

    git commit -m "Votre message qui résume vos modifcations (ex : ajout section Github)"

Un fois cela fait, il suffit de pousser vos modification sur le repo github avec la commande

    git push

Et voila tous est a jour maintenant

Si vous rencontrer des probleme google est votre amis ou alors passer a la section suivante



## Vous avez téléchargé avec une archive ZIP

Si vous avez téléchager l'archive ZIP sur le site Github il est impossible de faire ce qui est dit précedemment

La technique est facile mais peut amener a des probleme si mal réalisé.

Il vous suffi de selectionner tous vos fichier nouveau ou modifier que vous voulez ajouter au repo Github et de de les déplacer sur la page du repo Github comme montrer si dessous

![](https://github.com/CECI-BEST-LLN/KT-IT-Responsible/blob/main/img/Upload.png?raw=true)

on arrive sur cette page et il suffit d'ajouter les fichiers necessaire et de donner un titre au commit, pas besion de remplir description optionnel, ensuite il faut cliquer sur commit change
![](https://github.com/CECI-BEST-LLN/KT-IT-Responsible/blob/main/img/Upload1.png?raw=true)

# Autres

Pour ceux qui on facile avec Git il faut pas hesiter a jouer avec, ajouter des modifications, vous pouvez meme faire différente branche pour des versions différente. Faite comme vous voulez mais c'est vous le responsable si il y a des problemes ;)
