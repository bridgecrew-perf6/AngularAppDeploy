#!groovy
// Uses Declarative syntax to run commands inside a container.
pipeline {
    stages {
        stage('Main') {
            steps {
                container('kubectl') {
                    withKubeConfig([kubeconfigId: "kubeconfig"]) {
                        sh 'kubectl apply -f .'
                    }
                    kubernetesDeploy(configs: "angular.yml", kubeconfigId: "kubeconfig")
                }
            }
        }
    }
}
