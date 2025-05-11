pipeline {
    agent any
    
    stages {
        stage('Tester') {
            steps {
                echo "Testing poll SCM"
            }
        }
        stage('Build') {
            steps {
                echo 'Compile and package the app'
                echo 'Tool: npm'
                echo 'Updated build'
            }
        } 
        stage('Unit and Integration Tests') {
            steps {
                echo "Run automated unit and integration tests"
                echo "Tool: Jest"
            }
        }
        stage('Code Analysis') {
            steps {
                echo 'Perform static code analysis to make sure the code meets industry standards'
                echo "ESLint"
            }
        }
        stage('Security Scan') {
            steps {
                echo 'Scan dependecies for vulnerabilities'
                echo "Tool: `npm audit`"
            }
        }
        stage('Deploy to Staging') {
            steps {
                echo 'Deploy to staging environment'
                echo "Tool: AWS EC2"
            }
        }
        stage('Integration Tests on Staging') {
            steps {
                echo "Verify end-to-end functionality"
                echo "Tool: Selenium"
            }
        }
        stage('Deploy to Production') {
            steps {
                echo 'Push to production server'
                echo 'Tool: Docker'
            }
        }
    }
}