#!groovy
// Uses Declarative syntax to run commands inside a container.
pipeline {
    agent any
    stages {
        stage('Deploy angular app') {
            steps {
                script {
                    sh '''ls'''
                    kubernetesDeploy(configs: "angular.yml", kubeconfigId: "kubeconfig")
                }
            }
        }
    }
}
