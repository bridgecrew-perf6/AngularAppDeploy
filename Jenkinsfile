#!groovy
node {
  stage('List pods') {
    withKubeConfig([namespace: "default"]) {
          sh 'kubectl apply -f .'
        }
    }
}
