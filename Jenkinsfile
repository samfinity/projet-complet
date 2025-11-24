pipeline {
    agent any

    stages {
        stage('Déploiement Angular') {
            steps {
                script {
                    echo '🚀 Mise à jour du conteneur Angular...'
                    // --build : force la reconstruction de l'image
                    // --no-deps : ne redémarre pas mysql ou java, juste angular
                    // quest-angular : le nom du service dans le fichier yaml
                    sh 'docker compose up -d --build --no-deps quest-angular'
                }
            }
        }
    }
}