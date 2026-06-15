pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                echo 'Repository Cloned Successfully'
            }
        }

        stage('Build Docker Image') {
            steps {
                sh 'docker build -t demo-app .'
            }
        }

        stage('Push to ECR') {
            steps {
                echo 'Image Push Stage'
            }
        }

        stage('Deploy to Kubernetes') {
            steps {
                echo 'Deployment Stage'
            }
        }
    }
}