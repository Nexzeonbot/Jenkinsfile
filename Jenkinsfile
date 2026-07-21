pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                checkout scm
                echo 'Checkout completed'
            }
        }

        stage('Build') {
            steps {
                echo 'Build completed'
            }
        }

        stage('Test') {
            steps {
                echo 'Test completed'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Application deployed successfully.'
            }
        }
    }
}
