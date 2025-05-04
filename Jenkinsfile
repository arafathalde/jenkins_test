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
                script {
                    sh 'sudo rm -rf /var/www/html/*'
                    sh 'sudo cp -r * /var/www/html/'
                }
            }
        }
    }
}
