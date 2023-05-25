pipeline {
    agent { dockerfile true }
    stages {
        stage('Build Docker Image') {
            steps {
                sh 'docker build -t nextjsapp:latest .'
            }
        }
    }
}