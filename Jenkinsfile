#!groovy
node {
  stage('List pods') {
    withKubeConfig([namespace: "cicd"]) {
          sh 'kubectl apply -f .'
        }
    }
}
