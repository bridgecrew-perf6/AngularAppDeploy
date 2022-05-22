#!groovy
node {
  stage('List pods') {
    
    withKubeCredentials([
        [credentialsId: 'kubeconfig']
    ]){
          sh 'kubectl apply -f .'
      }
    }
}
