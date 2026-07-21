pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                echo 'Checking out source code...'
                checkout scm
            }
        }

        stage('Build') {
            steps {
                echo 'Building the application...'
                sh 'echo Build completed successfully'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
                sh 'echo All tests passed'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying application...'
                sh 'echo Application deployed successfully.'
            }
        }

    }

    post {
        always {
            echo 'Pipeline execution completed.'
        }

        success {
            echo 'Build SUCCESS'
        }

        failure {
            echo 'Build FAILED'
        }
    }
}
