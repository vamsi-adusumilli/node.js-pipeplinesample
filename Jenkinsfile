pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building your project...'
                // Add your build commands here
                sh 'echo "Build stage"'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
                // Add your test commands here
                sh 'echo "Test stage"'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying your application...'
                // Add your deployment commands here
                sh 'echo "Deploy stage"'
            }
        }
    }

    post {
        success {
            echo 'Pipeline executed successfully!'
        }
        failure {
            echo 'Pipeline execution failed!'
        }
    }
}


