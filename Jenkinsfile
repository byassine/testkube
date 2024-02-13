node {  
   
  
   stage('Clone repository') {

      steps {

        git 'https://github.com/byassine/testkube.git'

      }

    }
    
    stage('Deploy to Kubernetes') {

      steps {

        kubernetesDeploy(

          configs: 'deploy.yaml',

          kubeconfigId: 'my-kubeconfig'

        )

      }

    }
}
