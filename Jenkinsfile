pipeline {
    agent any
    stages {
        // stage('Build Docker image') {
        //     steps {
        //         sh "docker build -t new-app ."
        //     }
        // }
        // stage('Push Docker image') {
        //     steps {
        //          withCredentials([usernamePassword(credentialsId: 'docker_hub', usernameVariable: 'DOCKER_REGISTRY_USERNAME', passwordVariable: 'DOCKER_REGISTRY_PASSWORD')]) {
                    
        //             sh "echo \${DOCKER_REGISTRY_PASSWORD} | docker login -u \${DOCKER_REGISTRY_USERNAME} --password-stdin"
        //             sh "docker tag new-app nader12bp/new-app:v1"

        //             sh "docker push nader12bp/new-app:v1"
        //         }
        //     }
        // }
        stage('Deploy to OpenShift Cluster') {
            steps {
                 sh "oc get pods"
            }
        }
    }
}

