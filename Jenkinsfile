pipeline {
    agent any
    stages {
        stage('Build Docker Image') {
            steps {
                sh 'docker build -t nextjsapp:latest .'
            }
        }
        stage('Upload Docker Image') {
            steps {
                sh 'docker tag nextjsapp:latest 844595556253.dkr.ecr.us-east-1.amazonaws.com/nextjsapp'
                sh 'docker push 844595556253.dkr.ecr.us-east-1.amazonaws.com/nextjsapp'
            }
        }
    }
}