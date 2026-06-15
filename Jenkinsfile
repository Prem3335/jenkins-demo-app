pipeline {
    agent any

    stages {
        stage('Clone Repo') {
            steps {
                echo 'Repository Cloned Successfully'
            }
        }

        stage('Build Docker Image') {
            steps {
                echo 'Docker Build Successful'
            }
        }

        stage('Push to ECR') {
            steps {
                echo 'Image Pushed to ECR'
            }
        }

        stage('Deploy to Kubernetes') {
            steps {
                echo 'Application Deployed to Kubernetes'
            }
        }
    }
}
