pipeline {
    agent any 

    stages {
        stage('Deploy') {
            steps {
                // -d runs it in background, --remove-orphans cleans up old stuff
                sh 'docker compose -f mern-docker-compose.yaml up -d'
            }
        }
    }
}