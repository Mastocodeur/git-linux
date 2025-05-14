# 🧪 Atelier Git – Premières commandes


## 🎯 Objectif :
Savoir utiliser Git en ligne de commande pour gérer un projet simple : versionner un fichier, explorer l’historique, utiliser des branches, et synchroniser avec GitHub.


## Installer git


Dans un premier temps, on commence par installer la commande git sur notre pc. 

Pour ça, on suivra le tableau suivant : 

<table style="border-collapse: collapse; width: 100%;">
  <tr>
    <th style="border: 1px solid black; padding: 8px; text-align: left;">💻 Linux</th>
    <th style="border: 1px solid black; padding: 8px; text-align: left;">🪟 Windows</th>
    <th style="border: 1px solid black; padding: 8px; text-align: left;">🍎 macOS</th>
  </tr>
  <tr>
    <td style="border: 1px solid black; padding: 8px;">1. Mettre à jour les dépôts :</td>
    <td style="border: 1px solid black; padding: 8px;">1. Télécharger Git :</td>
    <td style="border: 1px solid black; padding: 8px;">1. Installer avec Homebrew :</td>
  </tr>
  <tr>
    <td style="border: 1px solid black; padding: 8px;"><pre><code>sudo apt update</code></pre></td>
    <td style="border: 1px solid black; padding: 8px;"><a href="https://git-scm.com">git-scm.com</a></td>
    <td style="border: 1px solid black; padding: 8px;"><pre><code>brew install git</code></pre></td>
  </tr>
  <tr>
    <td style="border: 1px solid black; padding: 8px;">2. Installer Git :</td>
    <td style="border: 1px solid black; padding: 8px;">2. Lancer l'installateur et suivre les étapes par défaut.</td>
    <td style="border: 1px solid black; padding: 8px;">2. Ou utiliser :</td>
  </tr>
  <tr>
    <td style="border: 1px solid black; padding: 8px;"><pre><code>sudo apt install git</code></pre></td>
    <td style="border: 1px solid black; padding: 8px;"></td>
    <td style="border: 1px solid black; padding: 8px;"><pre><code>xcode-select --install</code></pre></td>
  </tr>
  <tr>
    <td style="border: 1px solid black; padding: 8px;">3. Vérifier l'installation :</td>
    <td style="border: 1px solid black; padding: 8px;">3. Ouvrir Git Bash ou PowerShell puis vérifier :</td>
    <td style="border: 1px solid black; padding: 8px;">3. Vérifier :</td>
  </tr>
  <tr>
    <td style="border: 1px solid black; padding: 8px;"><pre><code>git --version</code></pre></td>
    <td style="border: 1px solid black; padding: 8px;"><pre><code>git --version</code></pre></td>
    <td style="border: 1px solid black; padding: 8px;"><pre><code>git --version</code></pre></td>
  </tr>
</table>


Parfois, il faudra redémmarer le PC ou juste votre VS Code pour que la commande git soit reconnue dans vos terminaux.

## 🔨 Créer un dépôt et intéragir avec 

