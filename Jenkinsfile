pipeline {
    agent any

    triggers {
        githubPush()
    }
    stages {
        stage('Checkout') {
            steps {
                // Checkout the repository
                checkout scm
            }
        }
        stage('Build') {
            steps {
                // Run your build commands here
                echo 'Building...'
            }
        }
        stage('Test') {
            steps {
                // Run your test commands here
                echo 'Testing...'
            }
        }
        stage('Deploy') {
            steps {
                // Run your deployment commands here
                echo 'Deploying...'
            }
        }
    }
    post {
        success {
            echo 'Build succeeded!'
        }
        failure {
            echo 'Build failed!'
        }
    }
}
//Changes to check automatic build by making a push


