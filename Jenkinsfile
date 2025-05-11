pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                echo 'Compile and package the app'
                echo 'Tool: npm'
            }
        } 
        stage('Test') {
            steps {
                echo 'Unit tests'
                echo 'Integration tests'
            }
        }
        stage('Code Quality Check') {
            steps {
                echo 'Check the quality of the code'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploy the application to a testing environment specified by the environment variable'
            }
        }
        stage('Approval') {
            steps {
                sleep 10
            }
        }
        stage('Deploy to Production') {
            steps {
                echo 'Deployed the project to $PRODUCTION_ENVIRONMENT'
            }
        }
    }
}