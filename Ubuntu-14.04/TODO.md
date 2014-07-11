	TODO au lancement

# installation de vim
sudo apt-get install vim

# générer clés SSH pour GitHub
mkdir ~/.ssh
ssh-keygen -t rsa -C "brunomatry@gmail.com"
eval "$(ssh-agent -s)"
ssh-add ~/.ssh/id_rsa
cat ~/.ssh/id_rsa

# Désactiver les suggestions commerciales du dash
gsettings set com.canonical.Unity.Lenses disabled-scopes "['more_suggestions-amazon.scope', 'more_suggestions-u1ms.scope', 'more_suggestions-populartracks.scope', 'music-musicstore.scope', 'more_suggestions-ebay.scope', 'more_suggestions-ubuntushop.scope', 'more_suggestions-skimlinks.scope']"

# retirer les icônes superflues sur le côté

# supprimer les paquets superflus
sudo apt-get purge thunderbird

# mettre a jour les dépôts
sudo apt-get update
sudo apt-get upgrade
sudo apt-get dist-upgrade

# activer Firefox Sync

# installer les sofs essentiels
sudo apt-get install gimp vlc flashplugin-installer oracle-java8-installer rar unrar zip unzip

# install les drivers

# nettoyer
sudo apt-get autoclean
sudo apt-get autoremove
