node("kubeagent") {
    git branch: "*/main", url: "https://github.com/woohwan/docker-build-test.git"
    stage ('kaniko') {
        container('kaniko') {
            script {
                sh '''
                /kaniko/executor --dockerfile `pwd`/Dockerfile \
                --context `pwd` \
                --destination=whpark70/kanio-build:v1
                '''
            }
         }
     }
}

