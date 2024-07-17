################################################
#        installe OpenTofu windows                    #
################################################

#  Lancer powershell en tant que administrateur:

# Lancer powershell en tant que administrateur et telecharger le script d'installation:
Invoke-WebRequest -outfile "install-opentofu.ps1" -uri "https://get.opentofu.org/install-opentofu.ps1"


# Exécuter le script:
& .\install-opentofu.ps1 -installMethod standalone -skipVerify



# Vérifier l'installation
Pour vérifier qu'OpenTofu est correctement installé, ouvrez une nouvelle ligne de commande et exécutez :
tofu --version

Vous pouvez maintenant commencer à utiliser OpenTofu. Par exemple, pour initialiser un nouveau projet, vous pouvez créer un fichier de configuration et utiliser les commandes OpenTofu pour gérer votre infrastructure.

# Pour désinstaller OpenTofu exécuter la commande:
Remove-Item install-opentofu.ps1
