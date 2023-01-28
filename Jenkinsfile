pipeline {
    agent any 

    stages {

        stage ('Build Docker Image'){
            steps {
                script {
                    dockerapp = docker.build("giannio/kube-news:${env.BUILD_ID}", '-f /opt/desafio2-kubenews/kube-news/src/Dockerfile /opt/desafio2-kubenews/kube-news/src')

                }
            }
        }
    }
}
