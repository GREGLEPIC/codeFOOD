# My CodeFOOD for git and github

```
touch checklist-vacances.md
```
créer un fichier

```
mkdir monPremierRepo
```
créer un dossier

```
git add checklist-vacances.md
git add monPremierRepo
git add .
```
```
git commit -m "Ajouté ma checklist-vacances.md (woohoo!)"
```

```
git commit -a -m "Ajouté itinéraire dans checklist-vacances.md"
```
L'option   -a demande à Git de mettre à jour les fichiers déjà existants dans son index. Pratique, non ?

```
git status
git log
```

```
git checkout SHADuCommit
```
Se positionner sur un ancien Commit

```
git checkout master
```
Pour revenir au commit le plus récent

```
git revert SHADuCommit
```
"revert" un commit, c'est-à-dire créer un nouveau commit qui fait l'inverse du précédent

```
git commit --amend -m "Votre nouveau message"
```
modifier le message de votre dernier commit

```
git reset --hard‌
```
annuler tous les changements que je n'ai pas encore commités.

```
git clone lienFourniParGitHub
```
Récuperer le lien d'un GitHub

```
git pull origin master
git push origin master
```

```
git branch nouvelle-branche
git checkout nouvelle-branche
git checkout -b ma-branche
```

```
git checkout brancheA
git merge brancheB
```
On ajoute dans une branche A les mises à jour que vous avez faites dans une autre branche B.
celui qu'on merge vient remplacer celui sur lequel nous sommes


```
git blame nomdufichier.extension
git show 05b1233 (début du SHA)
```
Pour retrouver qui a fait une modification
