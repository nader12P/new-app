pipeline {
    agent any
    stages {
        stage('Build Docker image for app.py and push it to docker hub') {
            steps {
                    sh "docker build -t new-app ."
                }
            }
        }
    }
}
