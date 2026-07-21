pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Deploy') {
            steps {
                sh '''
                cp index.html /usr/share/nginx/html/
                cp style.css /usr/share/nginx/html/
                cp script.js /usr/share/nginx/html/

                sudo systemctl restart nginx
                '''
            }
        }
    }
}
