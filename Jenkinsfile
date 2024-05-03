pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo "Build the code using Maven application"
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
                echo "Deploy the application to AWS Code Deploy"
            }
        }
        stage('Integration Tests on Staging') {
            steps {
                echo "Run integration tests on staging environment in Selenium"
            }
        }
        stage('Deploy to Production') {
            steps {
                echo "Deploy the application to AWS Code Deploy"
            }
        }
    }
    post {
        success {
            mail to: "salykeu2017@gmail.com",
            subject: "Build Status Email",
            body : "Build was successful!"
        }
    }
}
