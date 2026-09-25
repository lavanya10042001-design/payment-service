pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'feature/health-check',
                    url: 'https://github.com/lavanya10042001-design/payment-service.git'
            }
        }

        stage('Build & Test') {
            steps {
                bat 'mvnw.cmd test'
            }
        }
    }
}