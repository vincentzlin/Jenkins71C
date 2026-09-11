pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }
        stage('Build') {
            steps {
                echo 'Building...'
                // your build commands, e.g. sh 'make' or sh './gradlew build'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
                // e.g. sh 'pytest' or sh 'npm test'
            }
        }
    }
}