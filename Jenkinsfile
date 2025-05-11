pipeline {
    agent any
    
    environment {
        DIRECTORY_PATH = './portfolio'
        TESTING_ENVIRONMETN = 'test-env'
        PRODUCTION_ENVIRONMENT = 'clupai-prod'
    }
    
    stages {
        stage('Build') {
            steps {
                echo 'Fetch the source code from the dire ctory path specified by the environment variable'
                echo 'Compile the code and genreate any necessary artefacts'
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