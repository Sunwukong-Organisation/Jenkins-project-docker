# Jenkins-project-docker
Voici un exemple de README.md pour un mini-projet utilisant Jenkins avec un Dockerfile pour construire une image Docker contenant un serveur Nginx :

---

# Mini-projet Jenkins avec Dockerfile pour Nginx

Ce projet contient un ensemble de fichiers pour déployer un serveur Nginx à l'aide de Jenkins et Docker.

## Fichiers du projet

- `Jenkinsfile`: Script Jenkins Pipeline pour construire et déployer l'image Docker.
- `Dockerfile`: Fichier Dockerfile pour construire l'image Docker du serveur Nginx.
- `default.conf.template`: Modèle de configuration Nginx pour le serveur.
- `nginx.conf`: Configuration Nginx principale.

## Instructions

1. **Clonage du projet**:

   ```bash
   git clone https://github.com/votre-utilisateur/mini-projet-jenkins-nginx.git
   ```

2. **Construction de l'image Docker**:

   Assurez-vous que vous avez Docker installé et exécutez la commande suivante dans le répertoire du projet:

   ```bash
   docker build -t mon-nginx .
   ```

3. **Exécution du conteneur Docker**:

   Une fois l'image construite, vous pouvez exécuter le conteneur Docker en utilisant la commande suivante :

   ```bash
   docker run -d -p 8080:80 mon-nginx
   ```

   Cela démarre un conteneur Nginx qui écoute sur le port 8080.

4. **Accès au serveur Nginx**:

   Ouvrez un navigateur Web et accédez à [http://localhost:8080](http://localhost:8080) pour voir le serveur Nginx en action.

5. **Utilisation de Jenkins**:

   Utilisez le fichier `Jenkinsfile` pour créer un pipeline Jenkins qui automatise la construction et le déploiement de l'image Docker.

---

Ce README fournit des instructions de base pour utiliser le projet avec Docker et Jenkins. Vous pouvez personnaliser les fichiers et le pipeline Jenkins en fonction de vos besoins spécifiques.
