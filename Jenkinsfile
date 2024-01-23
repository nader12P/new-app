pipeline {
    agent any

    stages {
        stage('Build and Push Docker Image') {
            steps {
                    // Build Docker image for app.py
                    sh "docker build -t new-app ."
                }
            }
        }
    }
    
}
