pipeline {
    agent any

    stages {

        stage('Build Cocker Image') {
            steps {
                script {
                    dockerapp = docker.build("lpampolha/kube-news:${env.BUILD_ID}", '-f ./src/Dockerfile ./src')
                }
            }
        }

    }
}