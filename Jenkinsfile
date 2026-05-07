// coment
pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Stage 1: Build'
                echo 'Task: Compiling and packaging the application code.'
                echo 'Tool: Maven - a build automation tool used for Java projects.'
            }
        }

        stage('Unit and Integration Tests') {
            steps {
                echo 'Stage 2: Unit and Integration Tests'
                echo 'Task: Running unit tests to verify individual components and integration tests to ensure components work together.'
                echo 'Tools: JUnit for unit testing, Selenium for integration testing.'
            }
        }

        stage('Code Analysis') {
            steps {
                echo 'Stage 3: Code Analysis'
                echo 'Task: Analysing code quality and ensuring it meets industry standards.'
                echo 'Tool: Checkstyle - a static code analysis tool that checks Java code against a set of coding standards.'
            }
        }

        stage('Security Scan') {
            steps {
                echo 'Stage 4: Security Scan'
                echo 'Task: Scanning the code for known vulnerabilities and security issues.'
                echo 'Tool: OWASP Dependency-Check - identifies project dependencies with known vulnerabilities.'
            }
        }

        stage('Deploy to Staging') {
            steps {
                echo 'Stage 5: Deploy to Staging'
                echo 'Task: Deploying the application to a staging environment for pre-production testing.'
                echo 'Tool: AWS CLI - used to deploy the application to an AWS EC2 staging instance.'
            }
        }

        stage('Integration Tests on Staging') {
            steps {
                echo 'Stage 6: Integration Tests on Staging'
                echo 'Task: Running integration tests on the staging environment to validate the application in a production-like setting.'
                echo 'Tool: Selenium - automates browser-based integration testing against the staging server.'
            }
        }

        stage('Deploy to Production') {
            steps {
                echo 'Stage 7: Deploy to Production'
                echo 'Task: Deploying the verified application to the live production environment.'
                echo 'Tool: AWS CLI - used to deploy the application to an AWS EC2 production instance.'
            }
        }
    }

    post {
        success {
            echo 'Pipeline completed successfully!'
        }
        failure {
            echo 'Pipeline failed. Please check the console output.'
        }
    }
}
