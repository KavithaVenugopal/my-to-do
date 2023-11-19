pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Checkout the code from your version control system (e.g., Git)
                git 'https://github.com/KavithaVenugopal/my-to-do.git'
            }
        }

        stage('Build') {
            steps {
                // Install dependencies and build the Node.js application
                sh 'npm install'
            }
        }

        stage('Test') {
            steps {
                // Run automated tests
                sh 'npm test'
            }
        }

        stage('Deploy') {
            steps {
                // Perform deployment actions, e.g., creating deployable artifacts
                sh 'npm run deploy'
            }
        }
    }
}
