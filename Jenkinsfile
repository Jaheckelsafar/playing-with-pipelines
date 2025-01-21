pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Checkout step'
                git url: 'https://github.com/Jaheckelsafar/playing-with-pipelines.git', branch: 'main'
            }
        }

        stage('Build') {
            steps {
                echo 'Build step'
                // Install dependencies
                //sh 'npm install'
            }
        }

        stage('Test') {
            steps {
                echo 'Test step'
                // Run tests
                //sh 'npm test'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Delpoy step'
                // Deployment logic goes here (e.g., pushing to a cloud provider)
                echo 'Deploying application...'
            }
        }
    }

    post {
        always {
            echo 'Pipeline completed.'
        }
        failure {
            echo 'Pipeline failed!'
        }
    }
}
