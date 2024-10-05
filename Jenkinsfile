pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Building...'
                // Add your build steps here
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
                // Add your test steps here
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying...'
                sh 'kubectl apply -f kubernetes/sample-app-deployment.yaml'
                sh 'kubectl apply -f kubernetes/sample-app-service.yaml'
                }
            }
        }
    }
}