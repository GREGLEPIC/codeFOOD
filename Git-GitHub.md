# My CodeFOOD for git and github

Créer un fichier
```
touch checklist-vacances.md
```

Créer un dossier
```
mkdir monPremierRepo
```

Permet d'ajouter nom_fichier à ton futur commit

```
git add fichier.md
git add dossier
git add . (Rajoute tous les fichiers/dossiers créer ou modifier)
```

Enregistrer son travail avec un commentaire
```
git commit -m "Ajouté ma checklist-vacances.md (woohoo!)"
```

L'option   -a demande à Git de mettre à jour les fichiers déjà existants dans son index. Pratique, non ?
```
git commit -a -m "Ajouté itinéraire dans checklist-vacances.md"
```

Permet d'afficher l'état de tes fichiers par rapport au commit que tu es en train de réaliser (⚠ commande très pratique, à faire tout le temps)
```
git status
```


Permet d'afficher l'historique des commits
```
git log
```

Se positionner sur un ancien Commit
```
git checkout SHADuCommit
```

Pour revenir au commit le plus récent
```
git checkout master
```

"revert" un commit, c'est-à-dire créer un nouveau commit qui fait l'inverse du précédent
```
git revert SHADuCommit
```

modifier le message de votre dernier commit
```
git commit --amend -m "Votre nouveau message"
```

annuler tous les changements que je n'ai pas encore commités.
```
git reset --hard‌
```

Récuperer le lien d'un GitHub
```
git clone lienFourniParGitHub
```

Permet de récupérer ta branche nom_branche de ta remote nom_remote
```
git pull origin master
```

Permet de pousser ta branche nom_branche vers ta remote nom_remote
```
git push origin master
```

Création d'une nouvelle Branche
```
git branch nouvelle-branche
```

Aller sur une branche
```
git checkout nouvelle-branche
```

Création + aller sur la nouvelle branche (option -b)
```
git checkout -b ma-branche
```

On ajoute dans une branche A les mises à jour que vous avez faites dans une autre branche B.
celui qu'on merge vient remplacer celui sur lequel nous sommes
```
git checkout brancheA
git merge brancheB
```


Pour retrouver qui a fait une modification
```
git blame nomdufichier.extension
git show 05b1233 (début du SHA)
```


Pour ignorier des fichers
 ```
 créer un fichier .gitignore
 ```

 Pour sauvergarder son code sans faire un commit inutile et revenir plus tard à son code.
 ```
 git stash
 git stash pop
 ```
