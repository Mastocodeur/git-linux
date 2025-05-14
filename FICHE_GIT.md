# 📘 Git – Toutes les commandes essentielles

Formulaire des commandes git

## 🛠️ Initialisation d’un dépôt

```bash
git --version               # Affiche la version installée de Git
git init                    # Initialise un dépôt Git local vide
git clone <url>             # Clone un dépôt distant
git config --list           # Affiche la config Git
git config --global user.name "Ton Nom"
git config --global user.email "email@exemple.com"
```


## 📂 Suivi de fichiers

```bash
git status                  # Affiche les fichiers modifiés, ajoutés, supprimés
git add <fichier>           # Ajoute un fichier à l'index (staging)
git add .                   # Ajoute tous les fichiers modifiés
git reset <fichier>         # Retire un fichier de l'index
```

## 💾 Enregistrer les modifications


```bash
git commit -m "Message"                     # Commit avec message
git amend -m "Nouveau message"              # Modifie le dernier commit
git commit -am "Message"                    # Ajoute + commit en une commande                                    (pour fichiers déjà suivis)
```

## 🔄 Historique et Branches

```bash
git log                                     # Historique des commits
git log --oneline --graph --all             # Vue condensée et graphique
git show <hash>                             # Affiche un commit spécifique

git branch                                  # Liste les branches locales
git branch <nom>                            # Crée une nouvelle branche
git checkout <branche>                      # Change de branche
git checkout -b <branche>                   # Crée + bascule sur la branche
git branch -d <branche>                     # Supprime une branche locale
                            
```


## 🔀 Fusion & Rebase

```bash
git merge <branche>                  # Fusionne une branche dans l’actuelle
git rebase <branche>                 # Rebase l’historique sur une autre branche
git merge --abort                    # Annule une fusion en cours
git rebase --abort                   # Annule un rebase en cours
git rebase --continue                # Continue après avoir résolu un conflit
```

## 🌍 Travail à distance


```bash
git remote -v                      # Liste les dépôts distants
git remote add origin <url>        # Ajoute un dépôt distant
git push -u origin <branche>       # Envoie la branche vers le dépôt distant
git pull                           # Récupère les modifications du dépôt distant
git fetch                          # Récupère sans fusionner
git push                           # Envoie les commits
```

## ⚙️ Réinitialisation & nettoyage

```bash
git reset                  # Annuler un git add (fichiers ajoutés à l'index mais pas encore commités)
git reset --soft <commit>  # Réinitialise en conservant l’index et les fichiers
git reset --mixed <commit> # Réinitialise en conservant les fichiers (by défaut)
git reset --hard <commit>  # Réinitialise tout (attention ⚠️)
git clean -fd              # Supprime les fichiers non suivis
git clean -f               # Supprimer des fichiers non suivis (non ajoutés au Git)
git clean -d               # Suprrimer en incluant les répertoires
git clean -nd              # Prévisualiser
git clean -n               # Montrer ce qui serait supprimé, sans supprimer
git clean -fd              # Supprimer tout (non suivis + dossiers)
```

## 🧪 Stash (mettre de côté temporairement)

```bash
git stash                  # Sauvegarde les modifs non commit
git stash list             # Liste les stashs
git stash apply            # Restaure les dernières modifs mises de côté
git stash drop             # Supprime un stash
```

## 🔎 Recherche et comparaison

```bash
git diff                            # Diff entre l’index et le dernier commit
git diff <brancheA> <brancheB>      # Diff entre deux branches
git blame <fichier>                 # Montre qui a modifié chaque ligne
git log -p <fichier>                # Historique détaillé d’un fichier
```

## 🪄 Divers et astuces

```bash
git tag <nom>                      # Crée un tag sur le dernier commit
git tag -a v1.0 -m "Version 1.0"   # Tag annoté
git cherry-pick <commit>           # Applique un commit spécifique sur la branche actuelle
git shortlog -sn                   # Liste les contributeurs
git reflog                         # Historique de tous les HEAD (utile pour récupérer des commits perdus)
```


## 🧼 Annuler des erreurs

```bash
git restore <fichier>       # Annule les changements dans le fichier
git checkout -- <fichier>   # Ancienne syntaxe de restauration
git revert <commit>         # Crée un commit qui annule un commit précédent
```

## 📁 Submodules (modules Git imbriqués)

```bash
git submodule add <url> <chemin>           # Ajoute un submodule
git submodule update --init --recursive    # Initialise les submodules
git submodule sync                         # Synchronise les submodules
```

#
