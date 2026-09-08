pipeline {
    agent any

    stages {

        stage('Build') {
            steps {
                echo 'Task: Build the code using a build automation tool to compile and package the application.'
                echo 'Tool: Maven'
            }
        }

        stage('Unit and Integration Tests') {
            steps {
                echo 'Task: Run unit tests to verify individual components, and integration tests to verify components work together.'
                echo 'Tool: JUnit (unit tests), Postman/Newman (integration tests)'
            }
        }

        stage('Code Analysis') {
            steps {
                echo 'Task: Analyse the code to ensure it meets industry coding standards and identify code smells.'
                echo 'Tool: SonarQube'
            }
        }

        stage('Security Scan') {
            steps {
                echo 'Task: Scan the code and its dependencies to identify known security vulnerabilities.'
                echo 'Tool: OWASP Dependency-Check'
            }
        }

        stage('Deploy to Staging') {
            steps {
                echo 'Task: Deploy the application to a staging server for pre-production validation.'
                echo 'Tool: AWS EC2 (staging instance)'
            }
        }

        stage('Integration Tests on Staging') {
            steps {
                echo 'Task: Run integration tests against the staging environment to confirm production-like behaviour.'
                echo 'Tool: Postman/Newman'
            }
        }

        stage('Deploy to Production') {
            steps {
                echo 'Task: Deploy the application to the production server.'
                echo 'Tool: AWS EC2 (production instance)'
            }
        }
    }
}
