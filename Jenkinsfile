
pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Source code is already checked out from GitHub'
            }
        }

        stage('Build') {
            steps {
                bat 'mvn clean package'
            }
        }

        stage('Test') {
            steps {
                bat 'mvn test'
            }
        }
    }
}
