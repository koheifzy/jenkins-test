pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello from GitHub Jenkinsfile!'
            }
        }

        stage('Build') {
            steps {
                echo 'Building...'
                sh 'echo "This is Build stage"'
            }
        }

        stage('Test') {
            steps {
                echo 'Testing...'
                sh 'echo "All tests passed!"'
            }
        }
    }

    post {
        success {
            echo 'Pipeline SUCCESS!'
        }

        failure {
            echo 'Pipeline FAILED!'
        }
    }
}
