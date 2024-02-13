node {    
  stage('Deploy to Cluster') {
    steps {
      sh 'envsubst < deploy.yaml | kubectl apply -f -'
    }
  }
}
