pipeline {
    agent any

    stages {
        stage('Clone Code') {
            steps {
                git 'https://github.com/arafathalde/jenkins_test.git'
            }
        }

        stage('Deploy to Apache') {
            steps {
                sh '''
                    rm -rf /var/www/html/*
                    cp -r * /var/www/html/
                '''
            }
        }
    }
}
