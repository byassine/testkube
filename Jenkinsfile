node {    
    stage('Clone Repo') {
      git 'https://github.com/byassine/testkube.git'
    }
    stage('Deploy to Cluster') {
        steps {
          sh 'envsubst < deploy.yaml | kubectl apply -f -'
        }
    }
}
