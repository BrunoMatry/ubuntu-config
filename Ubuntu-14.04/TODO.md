	TODO au lancement

# Installation de vim
sudo apt-get install vim

# Générer clés SSH pour GitHub
mkdir ~/.ssh
ssh-keygen -t rsa -C "brunomatry@gmail.com"
eval "$(ssh-agent -s)"
ssh-add ~/.ssh/id_rsa
cat ~/.ssh/id_rsa

# Paramétrer Git
git config --global user.name "Bruno MATRY"
git config --global user.email brunomatry@gmail.com

# Installer des outils Git utils
sudo apt-get install tig gitg

# Désactiver les suggestions commerciales du dash
gsettings set com.canonical.Unity.Lenses disabled-scopes "['more_suggestions-amazon.scope', 'more_suggestions-u1ms.scope', 'more_suggestions-populartracks.scope', 'music-musicstore.scope', 'more_suggestions-ebay.scope', 'more_suggestions-ubuntushop.scope', 'more_suggestions-skimlinks.scope']"

# Retirer les icônes superflues sur le côté

# Supprimer les paquets superflus
sudo apt-get purge thunderbird

# Modifier le fichier /etc/apt/sources.list (voir fichier ./sources.list)
sudo mv /etc/apt/sources.list /etc/apt/sources.list.old
sudo cp ./sources.list /etc/apt/

# Mettre a jour les dépôts
sudo apt-get update
sudo apt-get upgrade
sudo apt-get dist-upgrade

# Activer Firefox Sync
# Installer Adblock (https://adblockplus.org/fr)
# Installer Ghostery (https://addons.mozilla.org/fr/firefox/addon/ghostery/)

# Installer les softs essentiels
sudo apt-get install gimp vlc flashplugin-installer rar unrar zip unzip

# Installer les drivers

# Nettoyer
sudo apt-get autoclean
sudo apt-get autoremove

# Changer la couleur de la console
