#!groovy
// Uses Declarative syntax to run commands inside a container.
pipeline {
    stages {
        stage('Main') {
            steps {
                container('kubectl') {
                    kubernetesDeploy(configs: "angular.yml", kubeconfigId: "kubeconfig")
                }
            }
        }
    }
}
