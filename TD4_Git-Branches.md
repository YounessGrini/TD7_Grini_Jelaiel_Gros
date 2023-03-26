# TD7/9: Git Branches

# Exercice 1 : Clone a Git repository

## 3. Using only command-line in your Linux shell, clone it to a local repository.
git clone https://github.com/YounessGrini/TD7_Grini_Jelaiel_Gros.git

# Exercice 2 : Push files to common repository

## 1. Create a branch named after you.
git branch YounessGrini

## 2. Create a new text file named after you (with the content you want).
touch YounessGrini.txt    
git add YounessGrini.txt  

## 3. Commit this new file.
git commit -m  "Nous faisons le TD7 avec Héloise et Elyes"

## 4. Push your branch to the remote repository.
git checkout YounessGrini    
git push --set-upstream origin YounessGrini  
git branch -a


# Exercice 3 : Merge simple changes

## 1. Merge your branch into the ’master’ branch.
git merge main

## 2. Push your changes in the ’master’ branch to the remote repository.
git push --set-upstream origin YounessGrini

# Exercice 4 : Resolve merge conflicts

## 1. Switch back to your own branch (not including the latest changes from the master branch).
git checkout YounessGrini

## 2. Edit the lines 2 to 6 of the README.md file with a text you like
nano README.md
#crtl+O 
#crtl+X

## 3. Commit this change
git add README.md

## 4. Pull latest status from the remote repository ’master’ branch into your local ’master’ branch.
git pull origin main

## 5. Merge your branch into the local ’master’ branch.
git merge YounessGrini

## 7. Push your changes in the ’master’ branch to the remote repository.
git push origin main

# Exercice 5 : Take latest changes from master in local branch

## 1. Pull the latest changes in the ’master’ branch, check the README.md
git pull origin main

## 2. Switch back to your own branch (not including the latest changes fromthe master branch).
git checkout YounessGrini

## 3. Merge the changes from ’master’ to your own branch.
git merge main

## 4. Commit this change
git add README.md  
git commit -m "Commit"

# Exercice 6 : Delete a branch

## 1. Delete your branch on local repository.
git branch -d YounessGrini

## 2. Delete your branch on distant repository.
git push --delete origin YounessGrini

# Exercise 7: Rebase interactively to have a clean history

## 1. Pull the latest changes in the ’master’ branch.
$ git pull origin main

## 2. Create a new local branch named after you and switch to it.
$ git checkout -b YounessGrini
