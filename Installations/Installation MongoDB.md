🍃 Installation de MongoDB
Ce guide vous accompagne pour installer MongoDB sur un système Windows, macOS ou Linux, et démarrer un serveur MongoDB local.

✅ Installation sur Windows
1. Télécharger MongoDB Community Server

Rendez-vous sur la page officielle :
https://www.mongodb.com/try/download/community

Sélectionnez la version stable pour Windows et téléchargez le .msi.

2. Installer MongoDB
Lancez l’installateur et suivez les étapes.

Cochez “Install MongoDB as a Service” pour démarrer automatiquement MongoDB.

Optionnel : Installez MongoDB Compass (interface graphique).

3. Démarrer MongoDB (si pas en service)
Ouvrez PowerShell ou CMD et tapez :

"C:\Program Files\MongoDB\Server\<version>\bin\mongod.exe"
(Remplacez <version> par la version installée, ex: 6.0)

✅ Installation sur macOS
1. Installer Homebrew (si nécessaire)
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

2. Installer MongoDB Community Edition
brew tap mongodb/brew
brew install mongodb-community@6.0

3. Démarrer MongoDB
brew services start mongodb-community@6.0

5. Vérifier que MongoDB tourne
mongo --eval 'db.runCommand({ connectionStatus: 1 })'

✅ Installation sur Linux (Ubuntu/Debian)

1. Importer la clé publique
wget -qO - https://www.mongodb.org/static/pgp/server-6.0.asc | sudo apt-key add -

2. Ajouter le dépôt
echo "deb [ arch=amd64,arm64 ] https://repo.mongodb.org/apt/ubuntu focal/mongodb-org/6.0 multiverse" | sudo tee /etc/apt/sources.list.d/mongodb-org-6.0.list

4. Mettre à jour et installer MongoDB
sudo apt-get update
sudo apt-get install -y mongodb-org

6. Démarrer MongoDB
sudo systemctl start mongod
sudo systemctl enable mongod

8. Vérifier le service
sudo systemctl status mongod

🔧 Utilisation basique
Lancer le shell MongoDB :

mongo

Créer une base de données :

use maBase

Ajouter un document dans une collection :

db.maCollection.insertOne({ nom: "Alice", age: 30 })

📚 Liens utiles

MongoDB Documentation Officielle

MongoDB Community Server

MongoDB University (formations gratuites)
