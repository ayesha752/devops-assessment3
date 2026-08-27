pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                echo 'Source code checked out successfully'
            }
        }

        stage('Build') {
            steps {
                echo 'Building application...'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
            }
        }

        stage('Package') {
            steps {
                echo 'Packaging application...'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying application...'
            }
        }
    }

    post {

        success {
            echo "Pipeline ${BUILD_NUMBER} completed successfully!"
        }

        failure {
            echo "Pipeline ${BUILD_NUMBER} failed!"
        }

        always {
            echo 'Pipeline finished.'
        }
    }
}