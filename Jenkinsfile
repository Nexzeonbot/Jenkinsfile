stage('Deploy') {
    steps {
        sh '''
        ssh -o StrictHostKeyChecking=no ec2-user@47.131.250.87 "
            cd /usr/share/nginx/html &&
            sudo git pull origin main
        "
        '''
    }
}
