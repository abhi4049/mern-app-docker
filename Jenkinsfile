pipeline {
    agent any 

    stages {
        stage('Checkout') {
            steps { 
                checkout scm 
            } 
        }
        stage('Deploy') {
            steps {
                // -d runs it in background, --remove-orphans cleans up old stuff
                sh 'docker compose -p mern-app -f mern-docker-compose.yaml up -d'
            }
        }
    }
}