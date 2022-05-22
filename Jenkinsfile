#!groovy
// Uses Declarative syntax to run commands inside a container.
pipeline {
    agent {
        kubernetes {}
    }
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
