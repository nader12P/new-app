pipeline {
    agent any
    stages {
        stage('Build Docker image') {
            steps {
                sh "docker build -t new-app ."
            }
        }
        stage('Push Docker image') {
            steps {
                 withCredentials([usernamePassword(credentialsId: 'dockerhub', usernameVariable: 'DOCKER_REGISTRY_USERNAME', passwordVariable: 'DOCKER_REGISTRY_PASSWORD')]) {
                    
                    sh "echo \${DOCKER_REGISTRY_PASSWORD} | docker login -u \${DOCKER_REGISTRY_USERNAME} --password-stdin"

                    sh "docker push nader12repo/new-app:v1"
                }
            }
        }
    }
}

