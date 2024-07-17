################################################
#        installe OpenTofu windows                    #
################################################

Prérequis

# Installer Git :
Téléchargez Git pour Windows depuis git-scm.com.
Exécutez l'installeur et suivez les instructions à l'écran.

# Installer Go :
Téléchargez l'installeur Go depuis golang.org/dl/.
Exécutez l'installeur et suivez les instructions à l'écran.
Configuration du PATH
Assurez-vous que les chemins vers Git et Go sont ajoutés à votre variable d'environnement PATH. L'installeur Go le fait normalement automatiquement.

# Installation d'OpenTofu
Ouvrez Git Bash (installé avec Git) ou une autre ligne de commande comme PowerShell.

# Clonez le dépôt OpenTofu depuis GitHub :
git clone https://github.com/opentofu/opentofu.git
cd opentofu

# Compiler OpenTofu :
go build -o opentofu.exe

# Déplacer l'exécutable :
Déplacez l'exécutable opentofu.exe vers un répertoire inclus dans le PATH de votre système. Par exemple :
move opentofu.exe C:\Windows\System32

Vous pouvez également ajouter le répertoire de votre projet actuel au PATH pour exécuter OpenTofu directement depuis ce répertoire.


# Vérifier l'installation
Pour vérifier qu'OpenTofu est correctement installé, ouvrez une nouvelle ligne de commande et exécutez :
opentofu --version
Cette commande devrait afficher la version d'OpenTofu que vous avez installée.

Utiliser OpenTofu
Vous pouvez maintenant commencer à utiliser OpenTofu. Par exemple, pour initialiser un nouveau projet, vous pouvez créer un fichier de configuration et utiliser les commandes OpenTofu pour gérer votre infrastructure.
