pipeline {
    agent any

    stage('Build Docker Image') {
            steps {
                script {
                    sh 'docker build -t new-app .'
                }
            }
        }
    
}
