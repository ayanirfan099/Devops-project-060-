pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                git 'https://github.com/ayanirfan099/Devops-project-060-.git'
            }
        }

        stage('Build') {
            steps {
                echo 'Building the app (if applicable)...'
                // sh 'your build command here'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests (if any)...'
                // sh 'pytest' or 'npm test'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying to Azure VM...'
                // Example: Copy files to /var/www/html
                sh '''
                cp -r * /var/www/html/
                '''
            }
        }
    }
}
