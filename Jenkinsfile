pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                // Build the Docker image
                sh 'docker build -t my-python-app .'
            }
        }
        stage('Test') {
            steps {
                // Run tests here
                sh 'echo "Running tests"'
            }
        }
        stage('Deploy') {
            steps {
                // Push the image to a Docker registry
                sh 'docker push my-python-app'
                // Deploy to the server
                sh 'echo "Deploying application"'
            }
        }
    }
}
