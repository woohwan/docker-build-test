pipeline {
    agent any
    environemnt {
        tools {
            tools {
                'org.jenkinsci.plugins.docker.commons.tools.DockerTool' 'docker'
            }
        }
    }
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

