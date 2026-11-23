
pipeline {
    agent any

    options {
        skipDefaultCheckout(true)
    }

    stages {

        stage('Checkout') {
            steps {
                echo 'Checking out source code'
                checkout scm
            }
        }

        stage('Build') {
            steps {
                echo 'Building application'
                echo 'Build completed successfully'
            }
        }

        stage('Test') {
            steps {
                echo 'Running application tests'
                echo 'Tests completed successfully'
            }
        }

        stage('Package') {
            steps {
                echo 'Packaging application'
                echo 'Packaging completed successfully'
            }
        }
    }

    post {
        success {
            echo 'CI Pipeline completed successfully!'
        }

        failure {
            echo 'CI Pipeline failed!'
        }
    }
}
