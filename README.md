# MalwareAnalyse

L'outil MalwareAnalyse est un analyseur de malware basé sur Python.

![App Screenshot](https://i.ibb.co/5MP5LWC/Scanner-Yura.png)


# Fonctionnalités principales

- La fonctionnalité basique est de pouvoir selectionner un fichier pour le scanner, et savoir si ce dernier est désigné malveillant ou non en suivant une ou plusieurs règles.

- Au lancement du script, vous avez la possibilité de faire un scan ``Simple`` et ``Avancée``.
- Le ``Simple`` va passer le(s) fichier(s) dans une rule qui permet de flag les plus communs outils malveillants.
- Le ``Avancée`` fait passer dans de nombreuses règles (409) pour augmenter les chances de trouver un outil malveillant.

- La notion de multithreadings a été ajouté pour permettre de lancer plusieurs fichiers à la fois et donc de scanner plusieurs fichiers potentiellement malveillants.

# Fonctionnalités annexes

- Une interface GUI permets une interface graphique plus jolie et simple d'utilisation, avec un background personalisable.

- Le rajout de règles pour les ransomwares ont été ajoutés. Vous pouvez donc avant de commencer votre scan selectionnez si vous souhaitez scanner un ransomware ou un malware.

- Un barre de progrès a été ajouté pour vous indiquez approximativement le temps restant pour votre scan.

- Une génération de rapport a été ajouté, pouvant servir de log également. Le chemin du fichier scan s'enregistre si il est détecter comme étant malveillant avec les règles qui l'ont flag.

# Installation

- Dans un premier temps, il faut clone le github.
- Installer la librairie Yara : ``pip install yura``
- En suite, il faut modifier dans les fichiers "malwares_index.yar" et "ransomware_index.yar" le chemin vers le fichiers ``malware`` et ``ransomware``. *(Possibilité de faire un rechercher remplacer)*
- Vous pouvez également customiser le ``background.jpg`` qui est le fond de l'interface GUI du script.

Pour finir, vous n'avez qu'à lancer le script ``malware_analyse_gui.py``.

**Enjoy ! :D**

![Enjoy](https://c.tenor.com/BP70qe8X0J8AAAAC/tenor.gif)
