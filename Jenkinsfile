pipeline {
    agent any

    stages {
        stage('Build Docker Image') {
            steps {
                script {
                    docker.build("my-image:${env.BUILD_ID}", "-f Dockerfile .")
                }
            }
        }
    }
}

