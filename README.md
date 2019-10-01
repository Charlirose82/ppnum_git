 
```ls``` => lister les fichiers 

```cd``` = changer de dossier ( ex: ```cd monDossier``` ) 

```touch``` : créer un fichier  ( ex: ```touch index.html``` ) 

```mkdir``` => créer un dossier ( ex : ```mkdir git-test``` )

```pwd``` => voir le dossier courant

```rm``` => supprimer un fichier / dossier ( avec le flag -r ) 
( ex : ```rm monFile.html``` / ex : ```rm -r monDossier```


```git status``` pour voir l'état du dossier de travail

```git log``` pour voir l'historique des commit

```git add``` pour ajouter un fichier avant de pouvoir le commiter ( ex: ```git add index.html``` ) 

```git commit -m 'mon message'``` pour l'ensemble des fichiers ajoutés avec ```git add```





pensez à renseigner vos informations via les commandes :
    
    git config --global user.email 'votre mail'
    git config --global user.name 'mon nom'
    
 =====  travail en local ( sur le poste de travail uniquement )

les autres commandes ( git ) sont sur la ressource indiquée : http://rogerdudler.github.io/git-guide

1) créez un dossier ( avec ```mkdir``` )
2) cd leNomDuDossierCréé
3) git init
4) créer un fichier ( ```touch nomDeFichier.html``` )
5) apporterdes modifications au fichier en écrivant quelque chose dedans( en ouvrant le fichier avec un éditeur de texte ou le bloc note + penser à le sauvegarder )
6) git add leNomDuFichier 
7) git commit -m  'le message de commit qui donne la raison de vos modifications '

=======


répéter pour avoir plusieurs commits 

=====  branches et conflits ======

```git branch maBranche``` pour créer une branche

```git checkout maBranche``` pour se déplacer sur une branche

```git merge maBranche```  pour merger la branche nommée sur la branche actuelle

1) créez une branche
2) faites un commit sur master ( en modifiant la ligne 1 de votre fichier )
3) changez de branche 
4) nouveau commit sur la meme ligne 
5) mergez ensuite master sur votre branche
6) résolvez les conflits !
7) commitez :)




========= faire le lien avec github ====

- créez un repo
- récupérer la commande exposée par github quand vous avez créé votre repo ( le ```git remote add origin URLDeMonRepoCréé``` )
( celle qui fait git remote add origin en https, pas ssh )

- lancez la dans le terminal uniquement quand vous êtes bien dans le dossier de travail de tout à l'heure

vérifiez avec ```git remote -v```


===== faire un push =====

pour envoyer les commit sur le serveur, on fait un ```git push origin master```
Si vous avez créé une autre branche et que vous êtes dessus, il faudrait indiquer le nom de cette branche à la place de master



========= jouer avec le serveur =====

/!\ modifiez toujours la même ligne pour les commits à venir pour ce tp ( ligne 1 typiquement )

1) créer une nouvelle branche avec 
git branch 'nomDeMaBranche'
2) aller sur la nouvelle branche avec la commande git checkout 'leNomDeMaBranche'
3) faites des modifications sur votre fichier
4) add + commit et vérifier avec ```git log```
5) revenez sur la branche master avec  la commande git checkout master en vérifiant avec git log que le commit fait sur l'autre branche n'existe pas sur master
6) refaites un nouveau commit sur master ( en modifiant un fichier + add + commit ) et vérifiez que ce commit est ok avec git log
7) tentez de fusionner les deux branches, en faisant un git merge NomDeMABranche via master
8) résolvez les conflits 
9) commitez pusher


================ RESOURCES ==========

explication pas à pas :
https://perso.liris.cnrs.fr/pierre-antoine.champin/enseignement/intro-git/

rappel des commandes utiles : 
https://www.hostinger.fr/tutoriels/commandes-git/

description du workflow et des commandes :
https://www.hostinger.fr/tutoriels/tuto-git/
divisée en articles assez complets : https://carlchenet.com/category/debuter-avec-git/

les branches :
https://carlchenet.com/debuter-avec-git-partie-4-les-commits-et-les-branches/
avec la doc officielle ( pour comprendre la théorie derrière, peut aider à structurer la compréhension ) : https://git-scm.com/book/fr/v2/Les-branches-avec-Git-Les-branches-en-bref

cours OpenClassrooms :
https://openclassrooms.com/fr/courses/1233741-gerez-vos-codes-source-avec-git

git expliqué avec des schémas visuels ( et rappel des commandes )
https://blog.lesieur.name/comprendre-et-utiliser-git-avec-vos-projets/
https://marklodato.github.io/visual-git-guide/index-fr.html


slides :
https://raspberry-pi.fr/cours/slides-git.html#/10/1
http://slides.com/moji3000/git_presentation/fullscreen#/15

vidéos :
https://www.grafikart.fr/tutoriels/git-presentation-1090
