TODO après l'installation d'Ubuntu
==================================
Installation de vim
-------------------	
    sudo apt-get install vim

Git
---
Installation et configuration de Git :

    sudo apt-get install git
    git config --global user.name "Bruno MATRY"
    git config --global user.email brunomatry@gmail.com

Générer clés SSH pour GitHub :

    mkdir ~/.ssh
    ssh-keygen -t rsa -C "brunomatry@gmail.com"
    eval "$(ssh-agent -s)"
    ssh-add ~/.ssh/id_rsa
    cat ~/.ssh/id_rsa.pub

Installer des outils Git utils :

	sudo apt-get install tig gitg

Désactiver les suggestions commerciales du dash
-----------------------------------------------
    gsettings set com.canonical.Unity.Lenses disabled-scopes "['more_suggestions-amazon.scope', 'more_suggestions-u1ms.scope', 'more_suggestions-populartracks.scope', 'music-musicstore.scope', 'more_suggestions-ebay.scope', 'more_suggestions-ubuntushop.scope', 'more_suggestions-skimlinks.scope']"

Dépôts apt
----------
Modifier le fichier /etc/apt/sources.list (voir fichier ./sources.list) :

    sudo mv /etc/apt/sources.list /etc/apt/sources.list.old
    sudo cp ./sources.list /etc/apt/

Mettre a jour les dépôts :

    sudo apt-get update
    sudo apt-get upgrade
    sudo apt-get dist-upgrade

Nettoyer :

    sudo apt-get autoclean
    sudo apt-get autoremove

Installer java
--------------
Récupérer la [dernière version de java](http://www.oracle.com/technetwork/java/javase/overview/index.html).

    sudo mkdir -p -v /opt/java
    cd ~/Downloads
    tar xvzf ~/Downloads/jre-****-linux-i586.tar.gz
    sudo mv -v jre****/opt/java
    sudo update-alternatives --install "/usr/bin/java" "java" "/opt/java/jre****/bin/java" 1
    sudo update-alternatives --set java /opt/java/jre****/bin/java 


Installer les softs essentiels
------------------------------
    sudo apt-get install gimp vlc flashplugin-installer rar unrar zip unzip

Configuration de Firefox
------------------------
Activer Firefox Sync, installer [Adblock](https://adblockplus.org/fr) et [Ghostery](https://addons.mozilla.org/fr/firefox/addon/ghostery/).

Les petits plus
---------------
* Retirer les icônes superflues sur la barre latérale
* Installer les drivers
* Changer la couleur de la console
* Installer sublime Text
* Installer les polices Windows