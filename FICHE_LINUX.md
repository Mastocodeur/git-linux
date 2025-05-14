# 📖 Linux - Commandes de Base

Ce document regroupe les principales commandes Linux utiles pour la navigation, la gestion des fichiers, les permissions, les processus, le réseau, etc.

---

## 📁 Navigation dans le système de fichiers

| Commande           | Description                                |
|--------------------|--------------------------------------------|
| `pwd`              | Affiche le chemin du répertoire courant    |
| `ls`               | Liste les fichiers/dossiers du répertoire  |
| `ls -l`            | Affiche les fichiers avec détails          |
| `ls -a`            | Affiche les fichiers, y compris les cachés |
| `cd [dossier]`     | Change de répertoire                       |
| `cd ..`            | Remonte d’un niveau                        |
| `cd ~`             | Va dans le dossier personnel               |
| `tree`             | Affiche une structure arborescente (si installé) |

---

## 📦 Gestion des fichiers et dossiers

| Commande                 | Description                            |
|--------------------------|----------------------------------------|
| `touch [fichier]`        | Crée un fichier vide                   |
| `mkdir [dossier]`        | Crée un dossier                        |
| `rm [fichier]`           | Supprime un fichier                    |
| `rm -r [dossier]`        | Supprime un dossier et son contenu     |
| `cp [src] [dest]`        | Copie un fichier ou dossier            |
| `mv [src] [dest]`        | Déplace ou renomme un fichier/dossier |
| `cat [fichier]`          | Affiche le contenu d’un fichier        |
| `more [fichier]`         | Affiche un fichier page par page       |
| `less [fichier]`         | Affiche page par page                  |
| `head -n 10 [fichier]`   | Affiche les 10 premières lignes        |
| `tail -n 10 [fichier]`   | Affiche les 10 dernières lignes        |

---

## 🔍 Recherche

| Commande                           | Description                              |
|------------------------------------|------------------------------------------|
| `find [chemin] -name "nom"`        | Recherche un fichier/dossier par nom     |
| `grep "mot" [fichier]`             | Recherche un mot dans un fichier         |
| `grep -r "mot" [dossier]`          | Recherche récursive dans les fichiers    |

---

## 🔑 Permissions

| Commande                           | Description                              |
|------------------------------------|------------------------------------------|
| `ls -l`                            | Affiche les permissions                  |
| `chmod [options] [fichier]`        | Modifie les permissions                  |
| `chown [user]:[groupe] [fichier]`  | Change le propriétaire                   |

---

## 🧠 Gestion des processus

| Commande             | Description                            |
|----------------------|----------------------------------------|
| `ps`                 | Affiche les processus en cours         |
| `top`                | Affiche les processus en temps réel    |
| `htop`               | Version améliorée de `top` (si installé) |
| `kill [PID]`         | Termine un processus                   |
| `kill -9 [PID]`      | Force l’arrêt d’un processus           |

---

## 🌐 Réseau

| Commande              | Description                            |
|-----------------------|----------------------------------------|
| `ping [adresse]`      | Vérifie la connectivité                |
| `ifconfig` / `ip a`   | Affiche les interfaces réseau          |
| `netstat -tulpn`      | Affiche les ports ouverts              |
| `curl [url]`          | Effectue une requête HTTP              |
| `wget [url]`          | Télécharge un fichier depuis une URL   |

---

## 📦 Gestion des paquets (Debian/Ubuntu)

| Commande                     | Description                              |
|------------------------------|------------------------------------------|
| `sudo apt update`            | Met à jour la liste des paquets          |
| `sudo apt upgrade`           | Met à jour les paquets installés         |
| `sudo apt install [paquet]`  | Installe un paquet                       |
| `sudo apt remove [paquet]`   | Supprime un paquet                       |
| `dpkg -i [fichier.deb]`      | Installe un paquet `.deb` manuellement   |

---

## 🛠️ Divers

| Commande                    | Description                                |
|-----------------------------|--------------------------------------------|
| `man [commande]`            | Affiche le manuel d’une commande           |
| `history`                   | Affiche l’historique des commandes         |
| `clear`                     | Nettoie le terminal                        |
| `alias ll='ls -la'`         | Crée un alias pour une commande            |
| `exit`                      | Quitte le terminal ou une session SSH      |

---

## 🧪 Redirections & Pipes

| Syntaxe     | Description                                 |
|-------------|---------------------------------------------|
| `>`         | Redirige la sortie vers un fichier (écrase) |
| `>>`        | Redirige la sortie vers un fichier (ajoute) |
| `<`         | Utilise un fichier en entrée                |
| `|`         | Envoie la sortie d’une commande vers une autre |

---

## 🧭 Navigation avancée

| Commande                       | Description                            |
|--------------------------------|----------------------------------------|
| `basename /chemin/fichier`     | Affiche juste le nom du fichier        |
| `dirname /chemin/fichier`      | Affiche le chemin sans le fichier      |

---

## 📊 Commandes `du` (Utilisation du disque)

| Commande                         | Description                               |
|----------------------------------|-------------------------------------------|
| `du`                             | Affiche l’espace disque utilisé par un fichier ou un dossier |
| `du -h`                          | Affiche l’espace disque utilisé en format lisible (Ko, Mo, Go) |
| `du -sh [dossier]`               | Affiche l’espace total utilisé par un dossier |
| `du -a [dossier]`                | Affiche l’espace utilisé pour chaque fichier dans le dossier |
| `du --max-depth=1 [dossier]`     | Affiche l’espace utilisé pour chaque sous-dossier (niveau 1) |
| `du -c [dossier]`                | Affiche l’espace utilisé total et détaille les sous-dossiers |

---

