pipeline {
  tools {
    'org.jenkinsci.plugins.docker.commons.tools.DockerTool' 'docker'
  }
  stages {
    stage('build') {
      steps {
        sh 'docker build .'
      }
    }
  }
}
