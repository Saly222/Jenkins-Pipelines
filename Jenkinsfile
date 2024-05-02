pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo "Build the code using Maven application are one"
            }
        }
        stage('Unit and Integration Tests') {
            steps {
                echo "Run unit tests using JUnit"
            }
        }
        stage('Code Analysis') {
            steps {
                echo "Integrate SonarQube for code analysis"
            }
        }
        stage('Security Scan') {
            steps {
                echo "Perform security scan using OWASP ZAP"
            }
        }
        stage('Deploy to Staging') {
            steps {
                echo "Deploy the application to AWS EC2 instance (staging)"
            }
        }
        stage('Integration Tests on Staging') {
            steps {
                echo "Run integration tests on staging environment"
            }
        }
        stage('Deploy to Production') {
            steps {
                echo "Deploy the application to AWS EC2 instance (production)"
            }
        }
    }
}
