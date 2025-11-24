pipeline {
    agent any

    stages {
        stage('Build & Deploy') {
            steps {
                script {
                    echo ' Démarrage du déploiement...'
                    
                    sh 'docker compose up -d --build --no-deps quest-angular'
                }
            }
        }
    }
}