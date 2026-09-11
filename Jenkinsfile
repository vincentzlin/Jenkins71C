pipeline {
    agent any
    
    environment {
        DIRECTORY_PATH = 'C:/Documents/'
        TESTING_ENVIRONMENT = 'test-environment1'
        PRODUCTION_ENVIRONMENT = 'production-environment1'
    }
    
    stages {
        stage('Build') {
            steps {
                echo 'Using tool: Maven'
                echo 'Compile and package the code'
            }
        }
        stage(' Unit and Integration Tests') {
            steps {
               echo 'Using tools: JUnit and Selenium'
               echo 'Run Unit tests and Integratiohuyukgyuujkljklin tests to ensure the code is functioning as expected'
            }
        }
        stage('Code Analysis') {
            steps {
                echo 'Using tool: SonarQube'
                echo 'Analyse and check the quality of the code, output any errors'
            }
        }
        stage('Security Scan') {
            steps {
                echo 'Using tool: Snyk'
                echo 'Perform a security scan on the code to identify any vulnerabilities'
            }
        }
        stage('Deploy to Staging') {
            steps {
                echo 'Deploy application to AWS EC2 instance'
            }
        }
        stage('Integration Tests on Staging') {
            steps {
                echo 'Using tool: Selenium'
                echo 'Rerun Integration tests against the staging environment'
            }
        }
        stage('Deploy to Production') {
            steps {
                echo 'Deploying to production environment on AWS EC2 instance'
            }
        }
    }
}
