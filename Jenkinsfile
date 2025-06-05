pipeline {
    agent any
    tools {
        jdk 'JDK-17'
        maven 'Maven 3.9.9'
    }
    stages {
        stage('Checkout') {
            steps {
                echo 'Checking out source code...'
                checkout scm
            }
        }
        stage('Build') {
            steps {
                echo 'Building the application...'
                bat 'mvn clean compile'
            }
        }
        stage('Test') {
            steps {
                echo 'Running tests...'
                bat 'mvn test'
            }
        }
        stage('Package') {
            steps {
                echo 'Packaging the application...'
                bat 'mvn package' 
            }
        }
        stage('Deploy to Tomcat') {
            steps {
                echo 'Deploying to Tomcat...'
                deploy adapters: [tomcat9(credentialsId: 'Tomcat',
                                         path: '',
                                         url: 'http://localhost:8080/manager/')],
                       contextPath: '/brightmind-tech',
                       war: 'target/*.war'
            }
        }
    }
    post {
        always {
            echo 'Cleaning up workspace...'
            cleanWs()
        }
        success {
            echo 'Pipeline completed successfully!'
        }
        failure {
            echo 'Pipeline failed. Check the logs for details.'
        }
    }
}