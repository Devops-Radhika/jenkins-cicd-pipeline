pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Checking out code from GitHub...'
                checkout scm
            }
        }
        stage('Build') {
            steps {
                echo 'Building Application...'
                // Example: sh './mvnw clean package'
            }
        }
        stage('Docker Build & Push') {
            steps {
                echo 'Building Docker Image...'
                // Example: sh 'docker build -t my-app:latest .'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying to Staging/Production...'
            }
        }
    }
}
