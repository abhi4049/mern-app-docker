pipeline {
    agent any 

    stages {
        stage('check') {
            steps {
                // -d runs it in background, --remove-orphans cleans up old stuff
                sh 'docker ps -a'
            }
        }
    }
}