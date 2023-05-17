# KT-IT-Responsible
Knowledge Transfer Poste IT CECI-BEST

# Pourquoi Latex ?
Il est vrai que Latex est pas la premiere choses que on pense pour faire un KT mais Latex apporte beaucoup d'avantes que Google docs n'ont pas.

1) C'est tres pro, respecte un format défini, facile a changer sans casser la structure.
2) Pas n'importe qui peut venir dessus et faire n'importe quoi ou supprimer des parties sans nous en rendre comptes
3) Associer avec Github impossible de se tromper, on peut revenir en arriere, voir qui a fait les modification
2) On est a l'EPL quand meme

---

Il y a beaucoup de moyen de modifier le KT je vais tenter de toutes les énoncers :

# Vous utiliser le compte Github du CECI-BEST-LLN

## Comment télécharger le KT pour le modifier 
2 possibilités :
premiere pour les gens a laise avec Git
l'autre pour des gens pas trop a laise

### Git clone

Il suffit de cloner le repos Github sur votre ordinateur, pour se faire 2 possibilités :
Et une 3eme pour ceux qui sont pas dutout a laise avec Github

#### avec un lien HTTP :

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

#### avec un lien SSH

c'est pour les KOG de l'info ça, je ne vais pas expliquer comment avoir une cles SSH mais sachez que si vous ne savez pas de quoi je parle laisson tomber cette méthode ou alors aller voir sur Google comment cloner un repo git avec une clef SSH

Pour ceux qui utilise cette methode c'est la meme chose que HTTP mais il faut mettre le lien du SSH a la place 

```bash
git clone <Lien-de-clone-SSH>
```

Attention il faut avoir une clef SSH lié au compte du CECI-BEST-LLN je vous laisse faire des recherche sur comment la créer et la setup mais rien de tres dur

#### Télécharger en ZIP

Il est possible de télécharger les fichier du Latex dans une archive ZIP, il suffit de cliquer sur *Download ZIP* dans le bouton *<>Code* comme montrer sur l'image au desssu.

Vous n'avez plus cas extraire vos fichier de l'archive et voila mais nous verrons plus tard que cela ne sera pas la methode la plus facile pour mettre a jour le KT

# Vous utilise votre propre compte Github

2 possibilités soit vous faite un Fork :

## Fork

Ici c'est un peu la meme chose mais a quelques points pres. Vu que on ne peut pas ajouter nos modifcations directement sur le repo avec notre compte perso, nous alons devoir faire un *Fork*. c'est si vous aviez le meme repo mais sur votre compte et donc vous pouvez le modifier directement et quand vous voulez le mettre a jour, il envoi une demande au vrai repo du CECI-BEST-LLN qui ensuite sera accepter ou refuser par la personne qui gerer le compte.

Pour se faire, il faut fork le repo, tres simple, il faut se rendre sur la page du repo et appuyer sur *Fork* en haut a droite.

![](https://github.com/CECI-BEST-LLN/KT-IT-Responsible/blob/main/img/fork.png?raw=true)

Il faut ensuite cliquer sur *Create Fork*

![](https://github.com/CECI-BEST-LLN/KT-IT-Responsible/blob/main/img/fork1.png?raw=true)

On peut voir que il est maintenant accessible dans mes repos de mon compte perso, il ne reste plus que a le cloner et de faire les modification sur celui-ci.

![](https://github.com/CECI-BEST-LLN/KT-IT-Responsible/blob/main/img/fork2.png?raw=true)


pour le cloner aller voir au dessus comment faire pour si on etais connecter avec le compte CECI-BEST-LLN

## Collaborateur

Soit vous ajouter votres compte perso aux Collaborateur du repo du KT, pour se faire il faut aller dans Settings -> Collaborateur -> add people -> et vous ajouter votre compte,
Il faut ensuite accepter la demande avec votre compte



# Modification

Ici c'est un peu comme vous le sentez pour modifier le KT (surtous mes fautes d'orthographes). Il existe plusieur outils pour faire du Latex tel que TexMaker, Visual Studio code possède des plugins pour faire du Latex. 

Le plus facile reste cependant [Overleaf](https://www.overleaf.com) en ligne qui est asser facile a prend en main et donc parfait pour les nouveaux.

# Mettre la nouvelle version sur le Github

La aussi plusieur possibilités en fonction de ce que vous avez fait précédemment et aussi si vous avez fait avec le compte CECI-BEST-LLN ou le votre.

## Avec le Compte CECI-BEST-LLN

### Vous avez fait un Git clone

Malheureusement Git ne permet plus de push des modification si nous avons fait un git clone avec HTTP, donc cette partie ne parle que pour ceux qui on utilisé les SSH

Si vous avez fait un git clone et donc que vos fichier sont dans votre PC, il suffit de remplacer ou de modifier ce que vous avez télécharger par le git clone par la nouvelle version du KT

ouvrez un terminal dans le dossiers qui contient le KT et il suffi maintenant d'ajoute vos nouveaux fichier avec la commande

    git add -A

une fois cela fait, il faut "commit" vos modification, pour cela, il suffit de faire :

    git commit -m "Votre message qui résume vos modifcations (ex : ajout section Github)"

Un fois cela fait, il suffit de pousser vos modification sur le repo github avec la commande

    git push

Et voila tous est a jour maintenant

Si vous rencontrer des probleme google est votre amis ou alors passer a la section suivante



### Vous avez téléchargé avec une archive ZIP

Si vous avez téléchager l'archive ZIP sur le site Github il est impossible de faire ce qui est dit précedemment

La technique est facile mais peut amener a des probleme si mal réalisé.

Il vous suffi de selectionner tous vos fichier nouveau ou modifier que vous voulez ajouter au repo Github et de de les déplacer sur la page du repo Github comme montrer si dessous

![](https://github.com/CECI-BEST-LLN/KT-IT-Responsible/blob/main/img/Upload.png?raw=true)

on arrive sur cette page et il suffit d'ajouter les fichiers necessaire et de donner un titre au commit, pas besion de remplir description optionnel, ensuite il faut cliquer sur commit change
![](https://github.com/CECI-BEST-LLN/KT-IT-Responsible/blob/main/img/Upload1.png?raw=true)

## Avec mon compte perso

### Collaborateur

C'est simple comme bonjour, vous avez l'autorisation de push vos modification directement sur le repo, 

Malheureusement Git ne permet plus de push des modification si nous avons fait un git clone avec HTTP, donc cette partie ne parle que pour ceux qui on utilisé les SSH

ouvrez un terminal dans le dossiers qui contient le KT et il suffi maintenant d'ajoute vos nouveaux fichier avec la commande

    git add -A

une fois cela fait, il faut "commit" vos modification, pour cela, il suffit de faire :

    git commit -m "Votre message qui résume vos modifcations (ex : ajout section Github)"

Un fois cela fait, il suffit de pousser vos modification sur le repo github avec la commande

    git push

Et voila tous est a jour maintenant

Si vous rencontrer des probleme google est votre amis ou alors passer a la section suivante

### Fork

Si vous avez clone avec votre compte perso vous avez donc réalisé un *Fork* comme dit précedemment. Pour ce faire il faut faire comme dit juste avant, commit vos changement.

Malheureusement Git ne permet plus de push des modification si nous avons fait un git clone avec HTTP, donc cette partie ne parle que pour ceux qui on utilisé les SSH

Si vous avez fait un git clone et donc que vos fichier sont dans votre PC, il suffit de remplacer ou de modifier ce que vous avez télécharger par le git clone par la nouvelle version du KT

ouvrez un terminal dans le dossiers qui contient le KT et il suffi maintenant d'ajoute vos nouveaux fichier avec la commande

    git add -A

une fois cela fait, il faut "commit" vos modification, pour cela, il suffit de faire :

    git commit -m "Votre message qui résume vos modifcations (ex : ajout section Github)"

Un fois cela fait, il suffit de pousser vos modification sur le repo github avec la commande

    git push

Et voila tous est a jour maintenant

Si vous rencontrer des probleme google est votre amis ou alors passer a la section suivante

Apres cela, vos changement ne sont disponible que sur le repo forker qui est sur votre repos perso et non disponible sur celui du CECI-BEST-LLN, il faut donc envoyer une requette de pull pour ajouter vos modification au repos de base. Pour ce faire rien de sorcier, rendez vous sur votre compte Github perso et aller sur le repo qui vous avez fork oû vous venez de push vos modification comme dit juste avant.

On rentre dans une partie qui fait peur mais elle est asser simple, juste il y a des bouton dans tous les sens, on fait comme quand on est dans une visite d'Usine, on ne touche a rien sauf si on a l'autorisation.

Alors, on va se rendre sur sont compte perso sur le repo forker du KT, on va ensuite dans la page *Pull requests* 

![](https://github.com/CECI-BEST-LLN/KT-IT-Responsible/blob/main/img/pullRequest.png?raw=true)

On crée un nouveau *Pull request*, enfaite on va crée un proposition au repo principal de fusionnner nos modification mais vu que c'est aussi les notre ben c'est nous qui acception.

![](https://github.com/CECI-BEST-LLN/KT-IT-Responsible/blob/main/img/pullRequest1.png?raw=true)

On peut voir tous nos commits qui sont les changement que nous avons apporté et on va cloquer sur *Create pull request*

![](https://github.com/CECI-BEST-LLN/KT-IT-Responsible/blob/main/img/pullRequest3.png?raw=true)

On ajoute un titre et un petite description si vous le souhaiter et on clique sur *Create pull request*

![](https://github.com/CECI-BEST-LLN/KT-IT-Responsible/blob/main/img/pullrequest4.png?raw=true)

On peut voir que notre requete de fusion a été crée. et que il n'y a pas de conflit (heureusement sinon c'est la merde)

![](https://github.com/CECI-BEST-LLN/KT-IT-Responsible/blob/main/img/pullRequest5.png?raw=true)

On va ensuite se rendre sur le compte Github CECI-BEST-LLN et aller dans la meme page *Pull request*

![](https://github.com/CECI-BEST-LLN/KT-IT-Responsible/blob/main/img/pullRequest.png?raw=true)

maintenant on peut accepter notre requete de fusion en cliquant sur *Merge pull request*

![](https://github.com/CECI-BEST-LLN/KT-IT-Responsible/blob/main/img/pullRequest7.png?raw=true)

Et on confirm le merge

![](https://github.com/CECI-BEST-LLN/KT-IT-Responsible/blob/main/img/pullRequest8.png?raw=true)

On peut maintenant voir que no modification on bien été ajouté au repo git et maintenant tous es a jour

![](https://github.com/CECI-BEST-LLN/KT-IT-Responsible/blob/main/img/pullRequest9.png?raw=true)

Oui c'est long mais c'est vous qui avez décider de faire de cette maniere pas moi



# Autres

Pour ceux qui on facile avec Git il faut pas hesiter a jouer avec, ajouter des modifications, vous pouvez meme faire différente branche pour des versions différente. Faite comme vous voulez mais c'est vous le responsable si il y a des problemes ;)

Si vous rencontrer des problemes avec Git je vous conseille d'utiliser GitKraken qui est une interface graphique qui est facile a utiliser pour justement faire les commande a votre place 

hesiter pas a changer le README afin qu'il soit le plus clair possible

Hesiter pas aussi a demander de l'aide a un ancien IT ou a une personne qui connais Git

Voila bonne chance

