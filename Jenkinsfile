pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                // Checkout the source code from your version control system
                git 'https://github.com/your/repository.git'
            }
        }
        
        stage('Build') {
            steps {
                // Build your application (e.g., compile code, run tests)
                sh 'mvn clean package'
            }
        }

        stage('test') {
            steps {
                // Build your application (e.g., compile code, run tests)
                sh 'test for code'
            }
        }
        
        stage('Deploy to Production') {
            when {
                // Define conditions for deploying to production (e.g., manual approval)
                expression { currentBuild.resultIsBetterOrEqualTo('SUCCESS') {
            
            }
        }
    }

