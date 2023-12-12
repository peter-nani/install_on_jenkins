pipeline {
    agent any

    stages {
        stage('Install Docker') {
            steps {
                script {
                    sh 'apt update'
                    sh 'apt install -y docker.io'
                    sh 'systemctl start docker'
                    sh 'systemctl enable docker'
                }
            }
        }

        stage('Build and Push Docker Image') {
            steps {
                script {
                    // Your Docker build and push commands go here
                }
            }
        }
    }
}
