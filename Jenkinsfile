pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Cloning repository'
                checkout scm
            }
        }

        stage('Build') {
            steps {
                echo 'Build stage started'
                sh 'echo "Build successful"'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests'
                sh 'echo "Tests passed"'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying application'
                sh 'echo "Deploy done"'
            }
        }
    }

    post {
        success {
            echo 'Pipeline SUCCESS 🎉'
        }
        failure {
            echo 'Pipeline FAILED ❌'
        }
    }
}
