pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building your project...'
                sh 'mvn clean install'  // Example: Maven build
            }
        }
        
        stage('Test') {
            steps {
                echo 'Running tests...'
                sh 'mvn test'  // Example: Run tests
            }
        }
        
        stage('Deploy') {
            steps {
                echo 'Deploying your application...'
                sh 'ssh user@server "deploy_script.sh"'  // Example: Deploy script
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

