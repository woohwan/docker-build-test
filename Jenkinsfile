pipeline {
  tools {
    'org.jenkinsci.plugins.docker.commons.tools.DockerTool' 'docker'
  }
  agent any
  stages {
    stage('build') {
      steps {
        sh 'docker build .'
      }
    }
  }
}
